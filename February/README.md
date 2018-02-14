## February 8

- Pointers
- Structures

#### Structures 

Ex: 

```cpp
 #include <iostream>
 #include <string>
 using namespace std;
 
 void printMovies(string title, string director, int year, int time);
 
 struct MovieData
 {
 	string title;
 	string director;
 	int yearReleased;
 	int runningTime; //In Minutes
 
 };
 
 int main()
 {	
 	MovieData disney, pixar;
 
 	disney.title = "Toy Story";
 	disney.director = "Juanito";
 	disney.yearReleased = 2012;
 	disney.runningTime = 120;
 
 	pixar.title = "Cars";
 	pixar.director = "Juanito Gonzales";
 	pixar.yearReleased = 2010;
 	pixar.runningTime = 124;
 	
 	printMovies(disney.title, disney.director, disney.yearReleased, disney.runningTime);
 
 	cout << endl;
 	printMovies(pixar.title, pixar.director, pixar.yearReleased, pixar.runningTime);
 
 	system("pause");
 	return 0;
 }
 
 void printMovies(string title, string director, int year, int time)
 {
 	cout << "Title: " << title << endl
 		<< "Director: " << director << endl
 		<< "Year Released: " << year << endl
 		<< "Running Time: " << time << endl;
 }
 
 ```

