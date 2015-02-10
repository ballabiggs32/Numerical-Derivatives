//Numerical-Derivatives
//How to calculate the derivative of a set of data

#include <iostream>
#include <cmath>
using namespace std;

int velocity(int a, int b)
{
  int equals = 0;
  equals = a + b;
  return a;
}

int main ()
{
  ifstream altitude;  //Declare the ifstream
  ofstream out; //Declared the output of the ofstream
  string store;
  altitude.open ("rocket_altitude_data.dat");
  cout << "What is the name of your file output?" << endl;
  cin >> store;
  out.open (store);
  if (altitude.is_open())
  {
    //Not yet correct - for steps 3-5
    double time1 = altitude.nextdata  //not a function, need to read in next data
    double alt1 = //set them to whatever the next piece of data it;
    double time2 = //set them to whatever the next piece of data it;
    double alt2 = //set them to whatever the next piece of data it;
    double time3 = //set them to whatever the next piece of data it;
    double alt3 =//set them to whatever the next piece of data it;
    double v2 = 0;
    while ( getline (altitude,))  //while the file still has data, perform this
    //not sure how to format because not sure what the data file looks like
    {
      v2 = (alt3 - alt1)/(time3 - time1);
      out << "time2 = " << variable of the numeric value << endl;
      out << "alt2 = " << variable of the numeric value << endl;
      out << "v2 = " << vairable of the numeric value v << endl;
      out << time = " << time2 << " alt2 = " << alt2 << " v2 = << v2 << endl;  //alternate method to put all outs on 1 line
      time1 = time2;
      time2 = time3;
      alt1 = alt2;
      alt2 = alt3;
      //Read new time3 and alt3 from the file
    }
    altitude.close();  //closes the input file
    out.close();  //closes the output file
  }
  else cout << "Unable to open file";
  return 0;
}
