#include<iostream>
using namespace std;
class calculator{
	public:
		float add(float n1,float n2){
			return n1+n2;
		}
		float subtract(float n1,float n2){
			return n1-n2;
		}
		float multiply(float n1,float n2){
			return n1*n2;
		}
		float division(float n1,float n2){
			return n1/n2;
		}
		
};
int main(){
	calculator calc; 
	float n1,n2;
	int choice;
	int x;
	
	do{
		cout<<"enter first number :";
		cin>>n1;
		cout<<"enter second number :";
		cin>>n2;
		cout<<"which operation do you want to perform ?";
		cout<<"\n1.addition "<<"\n"<<"2.subtraction\n"<<"3.multiply\n"<<"4.division";
		cin>>choice;
		
		switch (choice){
			case 1:cout<<"addition of "<<n1<<" and "<<n2<<" is : "<<calc.add(n1,n2)<<endl;
                    break;
            case 2:cout<<"subtraction of "<<n1<<" and "<<n2<<" is : "<<calc.subtract(n1,n2)<<endl;			
			        break;
			case 3:cout<<"multiplication of "<<n1<<" and "<<n2<<" is : "<<calc.multiply(n1,n2)<<endl;
			        break;
			case 4:cout<<"division of "<<n1<<" by "<<n2<<" is : "<<calc.division(n1,n2)<<endl;
			
			default:
				cout<<"Invalid choice !!!";
				break;
		}
	cout<<"do you want to continue ?(y/n)\n";
	cin>>x;
	}
	while(x=='y'||x=='Y');
	return 0;
}
