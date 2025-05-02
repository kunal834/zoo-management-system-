# zoo-management-system-
#include<iostream>  
using namespace std;

// zoo management system
class zoo{
    int a ;
    int b ;
    int c ;
   

    public :
    // Constructor to initialize variables
 zoo() : a(0), b(0), c(0) {}


    void cage( void )
   {
       cout<<"the total  cage for the total animals in the zoo is as of now :"<<a<<endl;
       cin>>a ;
}

void animal(void )
{
    cout<<"the total no. of animals in the zoo is as of now :"<<b<<endl;
    cin>>b;
    
}

void zoo_staff(void )
{
    cout<<"the total no. of staff in the zoo is as of now :"<<c<<endl;
    cin>>c ;
}

};

class animalspecies : public zoo{
   int amphibians;
   int reptiles; 
   int birds;
   int mammals ;
   int fishes;
   int insects ;
    
   public:

   // Constructor to initialize variables
 animalspecies() : amphibians(0), reptiles(0), birds(0), mammals(0), fishes(0), insects(0) {}

 
   void amphibianspecies( void )
   {
       cout<<"the total no. of amphibian species in the zoo is as of now :"<<amphibians<<endl;
       cin>>amphibians ;
   }

   void reptilespecies(void)
   {
       cout<<"the total no. of reptile species in the zoo is as of now :"<<reptiles<<endl;
       cin>>reptiles ;
   }
void birdspecies(void){
       cout<<"the total no. of bird species in the zoo is as of now :"<<birds<<endl;
       cin>>birds ;
   }
    
    void mammalsspecies(void)
    {
        cout<<"the total no. of mammal species in the zoo is as of now :"<<mammals<<endl;
        cin>>mammals ;
    }
    
    void fishspecies(void)
    {
        cout<<"the total no. of fish species in the zoo is as of now :"<<fishes<<endl;
        cin>>fishes ;
    }
    
    void insectspecies(void)
    {
        cout<<"the total no. of insect species in the zoo is as of now :"<<insects<<endl;
        cin>>insects ;
    }



};

class zoobudget : public animalspecies{
    int visitors;
    int ticket_price;
    int total_income;


    public:
    // Constructor to initialize variables
 zoobudget() : visitors(0), ticket_price(0), total_income(0) {}

    
    void visitor(void)
    {
        cout<<"the total no. of visitors anually  in the zoo is as of now :"<<visitors<<endl;
        cin>>visitors ;
    }
    
    void ticket(void)
    {
        cout<<"the ticket price for the zoo is as of now :"<<ticket_price<<endl;
        cin>>ticket_price ;
    }
    
    void income(void)
    {
        cout<<"the total income from the zoo is as of now :"<<total_income<<endl;
        cin>>total_income ;
    }
};

class maintainance  : public zoobudget{
    int food;
    int staff_salary;
    int infrastructure_cost;

    public:
     // Constructor to initialize variables
  maintainance() : food(0), staff_salary(0), infrastructure_cost(0) {}
    
    void foodcost(void)
    {
        cout<<"the total cost of food for the animals in the zoo is as of now :"<<food<<endl;
        cin>>food ;
    }
    
    void staffsalary(void)
    {
        cout<<"the total salary of the staff in the zoo is as of now :"<<staff_salary<<endl;
        cin>>staff_salary ;
    }
    
    void maintainancecost(void)
    {
        cout<<"the total maintainance cost of the zoo is as of now :"<<infrastructure_cost<<endl;
        cin>>infrastructure_cost ;
    }
};


    

int main(){

    cout<<"------------------------"<<endl;
    cout<<" zoo management system "<<endl;
    cout<<"------------------------"<<endl;


    cout<<"-------------------------"<<endl;
    int x;
    int y;
    cout<<"the charge sheet anually for the zoo x"<<x<<"to"<<y<<endl;
    cin>>x>>y;

    cout<<"-------------------------"<<endl;

    zoo m;
    m.cage();
    m.animal();
    m.zoo_staff();

    animalspecies as;
    as.amphibianspecies();
    as.reptilespecies();
    as.birdspecies();
    as.mammalsspecies();
    as.fishspecies();
    as.insectspecies();

    zoobudget b;
    b.visitor();
    b.ticket();
    b.income();
    

    maintainance m1;
    m1.foodcost();
    m1.staffsalary();
    m1.maintainancecost();

   

  
    return 0;
}
