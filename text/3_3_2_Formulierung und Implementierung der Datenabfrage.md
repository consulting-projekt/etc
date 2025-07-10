#### embedding modelle

leaderboard:
https://huggingface.co/spaces/mteb/leaderboard
nomic:
https://medium.com/@guptak650/nomic-embeddings-a-cheaper-and-better-way-to-create-embeddings-6590868b438f

##### SentenceTransformer paraphrase-multilingual-MiniLM-L12-v2

- Dimension: 384

##### openai text-embedding-3-small

- Dimension: 1536

##### nomic-embed-text

- Dimension: 768

##### geofox api

def get_point_byquery(client, point, point_cond):
    coordinate = None
    if point_cond:
        res_cond = check_name(client, point_cond)
        coordinate = res_cond['coordinate'] if res_cond else None
    res = check_name(client, point, coordinate=coordinate)
    if res:
        res2 = {}
        res2['location'] = res['coordinate']
        res2['name'] = res['name']
        return res2
    return None


def check_name(client, search_str, coordinate=None,  maxList=5):
    if search_str is None:
        return None

    endpoint = 'checkName'

    sdName = {
        "type": "UNKNOWN",
        "name": search_str,
        "city": "Hamburg",
    }

    if coordinate:
        sdName['coordinate'] = coordinate

    request = {
        "language": "de",
        "version": 59,
        "tariffDetails": True,
        "maxList": maxList,
        "theName": sdName,
        "allowTypeSwitch": True
    }

    res = client.send(endpoint, request)

    if res['returnCode'] == 'OK':
        if res.get('results', None):
            # Extract the first result
            res = res['results'][0]
            return res
    else:
        print(
            f"Error: {res['returnCode']} - {res['errorDevInfo']}, anfrage: {sdName}")

    return None
