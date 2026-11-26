#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
    int choice, n, i;
    char str1[100], str2[100], ch, sub[50];

    do {
        printf("\n---- STRING OPERATIONS ----\n");
        printf("1. Find Length of a String\n");
        printf("2. Concatenate Two Strings\n");
        printf("3. Copy a String\n");
        printf("4. Compare Two Strings\n");
        printf("5. Find character (strchr)\n");
        printf("6. Find substring (strstr)\n");
        printf("7. Tokenize string (strtok)\n");
        printf("8. Convert to uppercase\n");
        printf("9. Convert to lowercase\n");
        printf("10. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);
        getchar();   // consume leftover newline

        switch (choice) {
            case 1:
                printf("Enter a string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                printf("Length = %zu\n", strlen(str1));
                break;

            case 2:
                printf("Enter first string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                printf("Enter second string: ");
                fgets(str2, 100, stdin);
                str2[strcspn(str2, "\n")] = '\0';
                strncat(str1, str2, 99 - strlen(str1));
                printf("Concatenated String = %s\n", str1);
                break;

            case 3:
                printf("Enter a string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                strcpy(str2, str1);
                printf("Copied = %s\n", str2);
                break;

            case 4:
                printf("Enter first string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                printf("Enter second string: ");
                fgets(str2, 100, stdin);
                str2[strcspn(str2, "\n")] = '\0';
                n = strcmp(str1, str2);
                if (n == 0)
                    printf("Strings are equal\n");
                else if (n < 0)
                    printf("String 1 is less than string 2\n");
                else
                    printf("String 1 is greater than string 2\n");
                break;

            case 5:
                printf("Enter string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                printf("Enter character to find: ");
                scanf("%c", &ch);
                getchar();
                if (strchr(str1, ch) != NULL)
                    printf("Character found in string\n");
                else
                    printf("Character not found in string\n");
                break;

            case 6:
                printf("Enter main string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                printf("Enter substring: ");
                fgets(sub, 50, stdin);
                sub[strcspn(sub, "\n")] = '\0';
                if (strstr(str1, sub) != NULL)
                    printf("Substring found\n");
                else
                    printf("Substring not found\n");
                break;

            case 7:
                printf("Enter string with commas to tokenize: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                {
                    char *token = strtok(str1, ",");
                    while (token != NULL) {
                        printf("%s\n", token);
                        token = strtok(NULL, ",");
                    }
                }
                break;

            case 8:
                printf("Enter string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                for (i = 0; str1[i]; i++)
                    str1[i] = toupper((unsigned char)str1[i]);
                printf("Uppercase string: %s\n", str1);
                break;

            case 9:
                printf("Enter string: ");
                fgets(str1, 100, stdin);
                str1[strcspn(str1, "\n")] = '\0';
                for (i = 0; str1[i]; i++)
                    str1[i] = tolower((unsigned char)str1[i]);
                printf("Lowercase string: %s\n", str1);
                break;

            case 10:
                printf("Exiting.\n");
                break;

            default:
                printf("Invalid choice\n");
        }
    } while (choice != 10);

    return 0;
}
