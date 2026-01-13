#include<stdio.h>
#include<stdlib.h>
#include <string.h
int count=0;
struct stud
{
long long int ph;
int sem;
char name[15],un[15],brnch[8],
struct stud next;
}*head = NULL, *tail-NULL,*temp NULL, *templ;
void create(long long int n,int s,char na[20],char u[15] char b[5])
{
if (head==NULL)
{
head (struct stud*)malloc(1*sizeof(struct stud));
head->ph=n;
head->sem=s;
strcpy(head->name,na); stropy(head->usn,u); 
strepy(head->brnch,b);
head->next=NULL;
tail=head;
count++;
}
else
{
temp=(struct stud*)malloc(1*sizeof(struct stud));
temp->ph=n;
temp->sem=s;
strcpy(temp->name,na);
strcpy(temp->usn,u);
strcpy(temp->bruch,b);
temp->next=NULL;
tail-next=temp;
tail=temp;
count++;
}
}
}
void display()
{
temp1=head; 
if(temp1== NULL)
{
printf("\nlist is empty\n");
}
else
{
 printf("student details are as follows:\n"); 
while(temp1! NULL)
{
printf("\n"); 
printf("NAME:%s\nUSN:%s\nBRANCH:%s\nSEM:%d\nPHONE NO.:%lld\n",temp1->name, temp1->usn, temp1->brnch,templ->sem,temp1->ph);
printf(" \n");
}
temp1=temp1->next;
}
printf("no. of nodes=%d\n",count);
}
}
void insert_head(long long int n,int s,char na[15],char u[15],char b[8])
{
temp=(struct stud*)malloc(1*sizeof(struct stud));
temp->ph=n;
temp->sem=s;
strcpy(temp->name,na);
strcpy(temp->usn,u);
strcpy(temp->brnch,b);
temp->next=head;
head=temp;
count++;
}
void insert_tail(long long int n, int s,char na[15],char u[15],char b[8])
{
temp=(struct stud*)malloc(1*sizeof(struct stud));
temp->ph=n; 
temp->sem=s;
strcpy(temp-> name,na);
strcpy(temp->usn,u); strcpy(temp->brnch,b);
tail-> next =temp;
temp-> next= NULL;
tail=temp; 
count++;
}
void delete_head()
{
temp1=head; if(temp1==NULL)
{ 
printf("list is empty\n");

}
else
{ 
head=head->next; 
printf("deleted node is:\n");
printf("\n");
printf("NAME:%s\nUSN:%s\nBRANCH:%s\nSEM:%d\nPHONE NO.:%lld\n",templ->name, temp 1->usn,temp1>brnch, temp1->sem,templ->ph);
printf("\n");
free(temp1);
count--;
}
} 
void delete_tail()
{
temp1=head; 
if(temp1==NULL) 
{
printf("list is empty\n"); 
}
while(temp1->next!=tail)
{
temp1=temp1->next;
}
printf("deleted node is:\n");
printf("\n");
printf("NAME:%s\nUSN:%s\nBRANCH:%s\nSEM:%d\nPHONE NO.:%lld\n",tail->name,tail-
>usn,tail brnch,tail->sem,tail>ph);
printf("\n");
free(tail);
tail=temp1;
tail->next=NULL; 
count--;
}
void main()
{
int choice;
long long int ph;
int sem;
chat name[20],usn[15],branch[5];
printf("------MENU\n");
printf("1.create/a2. Insert from head \n3. Insert from tail\n4.Delete from head \n5.Delete from
tail\n6. display/n7.exit\n");
printf("\n");
while(1)
{
printf("enter your choice\n"); 
scanf("%d",&choice).
switch(choice)
{
case 1 :printf("enter the name usn branch sem phno of the student respectively/a"); 
scanf(%s%s%s%d%lld" name,usn,bench&sem,&ph); 
create(ph,sem,name, an bench),
break;
case 2: printi enter the name usn branch sem phno. of the student respectivelyin"); 
scanf("%s%s%s%d%lld",name,usn branch,&sem,&ph); 
insert head(phsem namen,bach);
break;
case 3: printf(" enter the name usn branch sem phno. of the student respectively \n"); scanf("%s%s%s%d%lld",name,usn,branch, &sem,&ph); insert_tail(ph,sem,name,usn,branch); 
break;
case 4 :delete_head();
break;
case 5 :delete_tail();
