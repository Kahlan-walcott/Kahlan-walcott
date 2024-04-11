def recursive(word_list, word, list_index):
    if len(word_list) <= 0:
        return 0
    if len(word_list) != 0:
        if word == word_list[0]:
            return list_index
        elif word != word_list[0]:
            return recursive(word_list[1:], word, list_index + 1)
        else:
            return 0

