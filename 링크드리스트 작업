//링크 리스트
//https://www.youtube.com/watch?v=cAZ8CyDY56s&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=6

#include <stdio.h>
#include <stdlib.h>

struct Node {   // 연결 리스트의 노드 구조체
    struct Node* next;    // 다음 노드의 주소를 저장할 포인터
    int data;             // 데이터를 저장할 멤버
};

struct Node* head; // global variabel, can be accessed anywhere

void Insert(int x) {
    struct Node* temp = (struct Node*) malloc(sizeof(struct Node));
    temp->data = x;
    temp->next = head;
    head = temp;
}

void Print() {
    struct Node* temp = head;
    printf("List is: ");
    while (temp != NULL) {
        printf(" %d", temp->data);
        temp = temp->next;
    }
    printf("\n");
}
int main()
{
    head = NULL; // empty variable, can be accessed anywhere
    printf("How many numbers? \n");
    int n, i, x;
    scanf("%d", &n);
    for ( i = 0; i < n; i++) {
        printf("Enter the number \n");
        scanf("%d", &x);
        Insert(x);
        Print(head);
    }
    
    printf("\n\n===End");
}
