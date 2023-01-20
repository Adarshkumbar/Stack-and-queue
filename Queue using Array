#include<iostream>
#include<cstdlib>
using namespace std;

#define N 5     // MAX size oF Queue
int Queue[N];
int front=-1,rear=-1;			// Not Pointing to any index
void enqueue(int x)
{
	if(rear==N-1)
	{
		cout<<"\n!!! Queue is Full !!!";
	}
	else if(front==-1 && rear==-1)
	{
		front=rear=0;
		Queue[rear]=x;
	}
	else
	{
		rear++;
		Queue[rear]=x;
	}
}

void dequeue()
{
	if(front==-1 && rear==-1)
	{
		cout<<"\n!!!Underflow!!!";
	}
	else
		if(front==rear)
		{
			cout<<"\nDequeued Emt is "<<Queue[front]<<endl;
			front=rear=-1;
		}
	else
	{
		cout<<"\nDequeued Emt is "<<Queue[front]<<endl;
		front++;
	}
}
void show()
{
	int i;
	cout<<"\nQueue is :";
	if(front==-1 && rear==-1)
	{
		cout<<"\n!!!Empty Queue!!!";
	}
	else
	{
		for(i=front;i<=rear;i++)
		{
			cout<<Queue[i]<<"\t";
		}
	}
}
int main()
{
	int ch;
	do
	{
		cout<<"\n1.Enqueue\t2.Dequeue\t3.Show\t\t4.Stop :";
		cin>>ch;
		switch(ch)
		{
			case 1:cout<<"Enter Val to enqueue:";
					int val;
					cin>>val;
					enqueue(val);
					break;
			case 2:dequeue();
					break;
			case 3:show();
					break;
			case 4:cout<<"\nExiting.......";
					exit(0);
					break;
			default:cout<<"\n !!! Invalid Entry !!!";
		}
	}while(ch!=4);
}
