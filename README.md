# Homework_9.1


def popular_words(text, words):
    text_lower = text.lower().split()

    word_count = {}

    for word in words:
        word_count[word] = text_lower.count(word)

    return word_count


assert popular_words(
    'When I was One I had just begun When I was Two I was nearly new',
    ['one', 'two', 'three']
) == {'one': 1, 'two': 1, 'three': 0}, 'Test1'

print("тесты пройдены!")
