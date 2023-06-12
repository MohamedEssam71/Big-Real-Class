# OOP-Assignment-2

# Big-Real-Class
This is a big Real data type in C++.



It is required to build a class `BigReal`. An object of this class represents a real number of arbitrary length. The public interface of your class will be as follows. For functions where the default implementation of C++ is enough and works fine, you do not need to re-implement them. Break your code into a header file, implementation file, and application file.

## Class Interface

```cpp
class BigReal {
private:
  // ...

public:
  BigReal(double realNumber = 0.0); // Default constructor
  BigReal(string realNumber);
  BigReal(BigDecimalInt bigInteger);
  BigReal(const BigReal& other); // Copy constructor
  BigReal(BigReal&& other); // Move constructor

  BigReal& operator=(BigReal& other); // Assignment operator
  BigReal& operator=(BigReal&& other); // Move assignment 

  BigReal operator+(BigReal& other);
  BigReal operator-(BigReal& other);

  bool operator<(BigReal anotherReal); 
  bool operator>(BigReal anotherReal); 
  bool operator==(BigReal anotherReal); 

  int size(); 
  int sign(); 

  friend ostream& operator<<(ostream& out, BigReal num);
  friend istream& operator>>(istream& out, BigReal num);
};
```

## Team members
| Name | ID |
|------|----|
| Mohamed Essam Mahmoud Osman | 20210346 |
| Salah Eddin Mohamed Salah | 20210187 | 
| Abdelrahman Gamal Ali | 20210233 |
