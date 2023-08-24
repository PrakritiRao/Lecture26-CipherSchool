# Lecture26-CipherSchool
#include<iostream>
using namespace std;

// we achieve this using something called a "class"
class student{   //class is user-defined data type
	public:
		//also private access specifier
		string name;
		int mids;
		float ends;
		bool pre_abs;
		
		void calculate_marks(){ // these are parameters which must be passed while the function of this class is being called
			float total_marks;
			
			total_marks = mids*0.5 + ends*0.75;
			
			cout<<"The marks of: "<<name<<" is "<<total_marks<<endl;
		}
		
		void totalMarksIncludingProject(int project_marks){
			cout<<mids+ends+project_marks;
		}
		
		void calculate_fail_probability(){
			if(ends <= 10){
				cout<<"yes, this student needs to attend the same class for one more year....";
			}
		}
};
