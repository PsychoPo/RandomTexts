#include <iostream>
#include <cstdlib>
#include <ctime>

void generator(int size) {
    srand(time(NULL)); //Вводим длинну текста и получаем рандомные слова

    std::string text;

    for (int i = 0, j = 0; i < size; i++) {
        j = rand() % 10 + 1;

        if (j > size - i) j = size - i;
        i += j;

        for (int k = 0; k < j; k++) {
            text += (char)(rand() % 26 + 97);
        }
        text += ' ';
    }
    text[text.size() - 1] = '.';

    std::cout << text << std::endl;
}

int main() {
    int textLength;

    std::cin >> textLength;

    generator(textLength);

    return 0;
}
