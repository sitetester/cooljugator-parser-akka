Currently it's parsing common verbs from given language codes. More codes could be added later on and still need to save those verbs in DB.

Data is parsing using Akka actor model. Multiple instances of SAME actor are created (depending upon language codes) and ALL HTTP requests are executed in parallel fashion.

TODO: still in progress to parse `ALL` link for each language (e.g. https://cooljugator.com/en/list/all)

Output shared on https://stackoverflow.com/questions/49882201/creating-multiple-actors-at-once/59800946#59800946  