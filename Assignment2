import 'dart:io';

// Circle Circumference

class Circle {
  double _raDius = 0;
  set radius(double val) {
    _raDius = val;
  }

  double get radius => _raDius;
  double Calculate_Circumference() {
    double CircumFerence = 2 * 3.14 * _raDius;
    return CircumFerence;
  }
}

// Student Data

class Student {
  late String _name;
  late int _age;
  late String _major;
  late double _gpa;
  Student(this._name, this._age, this._major, this._gpa);
  String get name => _name;
  int get age => _age;
  String get major => _major;
  double get gpa => _gpa;
  set name(String val) {
    _name = val;
  }

  set age(int val) {
    _age = val;
  }

  set major(String val) {
    _major = val;
  }

  set gpa(double val) {
    _gpa = val;
  }

  String Grade_Level() {
    if (_age >= 18 && _age <= 21) {
      return 'Freshman';
    } else if (_age >= 22 && _age <= 24) {
      return 'Sophomore';
    } else if (_age >= 25 && _age <= 27) {
      return 'Junior';
    } else if (_age >= 28) {
      return 'Senior';
    } else {
      return 'Not Applicable';
    }
  }
}

// Book Data
class Book {
  late String _title;
  late String _Author;
  late String _Publisher;
  late double _price;

  Book(this._title, this._Author, this._Publisher, this._price);

  String get title => _title;

  String get author => _Author;

  String get publisher => _Publisher;

  double get price => _price;

  set title(String val) {
    this._title = val;
  }

  set author(String val) {
    this._Author = val;
  }

  set publisher(String val) {
    this._Publisher = val;
  }

  set price(double val) {
    this._price = val;
  }

  double Calculate_Discount(double disc) {
    double discount_amt = _price * (disc / 100);
    return _price - discount_amt;
  }
}

// Course Data

class Course {
  late String _name;
  late String _code;
  late String _instructor;
  late int _credits;
  late double _costPer_Credit;

  Course(this._name, this._code, this._instructor, this._credits,
      this._costPer_Credit);

  String get name => _name;
  String get code => _code;
  String get instructor => _instructor;
  int get credits => _credits;
  double get costpercredit => _costPer_Credit;

  set name(String val) => _name = val;
  set code(String val) => _code = val;
  set instructor(String val) => _instructor = val;
  set credits(int val) => _credits = val;
  set costpercredit(double val) => _costPer_Credit = val;

  double calculateTcost() {
    return _credits * _costPer_Credit;
  }
}

// Bank Info

class BankAccount {
  double _balance = 0;
  String _ownername = "";
  BankAccount(this._ownername, this._balance);
  get balance => _balance;
  get owner => _ownername;
}

class Bank {
  late List<BankAccount> _Accounts;
  Bank() {
    _Accounts = [];
  }
  void addAccount(BankAccount val) {
    _Accounts.add(val);
  }

  void removeAccount(BankAccount val) {
    _Accounts.remove(val);
  }

  BankAccount findhighvaluebank() {
    BankAccount Top_Value_Bank = _Accounts[0];
    for (int i = 0; i < _Accounts.length; i++) {
      if (_Accounts[i].balance > Top_Value_Bank.balance) {
        Top_Value_Bank = _Accounts[i];
      }
    }
    return Top_Value_Bank;
  }
}

void main() {
  print("--------Circle Circumference--------");
  Circle cr = Circle();
  cr.radius = 30;
  print(cr.radius);
  print(cr.Calculate_Circumference());

  print("\n\n--------Student Data--------");
  Student student_1 = Student("Hamza", 19, "OOP", 3.5);
  Student student_2 = Student("Kumail", 18, "ICT", 3.5);
  print("--------Student 1--------");
  print("Name: " + student_1.name);
  print("Major: " + student_1.major);
  print("Age: " + student_1.age.toString());
  print("GPA: " + student_1.gpa.toString());
  print("--------Student 2--------");
  print("Name: " + student_2.name);
  print("Major: " + student_2.major);
  print("Age: " + student_2.age.toString());
  print("GPA: " + student_2.gpa.toString());

  print("\n\n--------Book Data--------");
  print("--------Book 1 Data--------");
  // Book_1 = "https://books.google.com.pk/books/about/Clean_Code.html?id=_i6bDeoCQzsC&source=kp_cover&redir_esc=y"
  // Book_2 = "https://books.google.com.pk/books?id=ML9Jzb7SL9EC&source=gbs_similarbooks"
  Book Book_1 = Book("Clean Code: A Handbook of Agile Software Craftsmanship",
      "Robert C. Martin", "Pearson Education", 28.99);
  Book Book_2 = Book("Agile Java¿: Crafting Code with Test-Driven Development",
      "Jeff Langr", "Pearson Education", 9.31);
  print("Title: " + Book_1.title);
  print("Author: " + Book_1.author);
  print("Publisher: " + Book_1.publisher);
  print("Price: " + Book_1.price.toString());
  print("Discounted Price: " + Book_1.Calculate_Discount(20).toString());

  print("\n\n--------Book 2 Data--------");
  print("Title: " + Book_2.title);
  print("Author: " + Book_2.author);
  print("Publisher: " + Book_2.publisher);
  print("Price: " + Book_2.price.toString());
  print("Discounted Price: " + Book_2.Calculate_Discount(20).toString());

  print("\n\n--------Book Data--------");
  Course course = Course(
      "Introduction to Computer Science", "CS101", "Sarwat Iqbal", 3, 100);
  print("Course Name: " + course.name);
  course.costpercredit = 150;
  print("Credit Cost: " + course.costpercredit.toString());
  print("Total Credit Cost: " + course.calculateTcost().toString());

  print("\n\n--------Bank Data--------");
  Bank Account_control = Bank();
  BankAccount Account_1 = BankAccount("Muhammad Hamza", 1056787.43);
  BankAccount Account_2 = BankAccount("Kumail Abbas", 656787.46);
  Account_control.addAccount(Account_1);
  Account_control.addAccount(Account_2);

  print("Detail of High Balance Account");
  print("Owner: " + Account_control.findhighvaluebank().owner);
  print("Balance: " + Account_control.findhighvaluebank().balance.toString());

  print("\n\n--------Palindrome Checker--------");

  stdout.write("Enter Any Text: ");
  String User_Input = stdin.readLineSync()!;
  String reversed = "";
  for (int i = User_Input.length - 1; i >= 0; i--) {
    reversed = reversed + User_Input[i];
  }
  if (User_Input.toLowerCase() == reversed.toLowerCase()) {
    print("Its Palindrome Text");
  } else {
    print("Its not Palindrome Text");
  }
}
