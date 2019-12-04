#include <iostream>
#include <string>
#include <algorithm>
using namespace std;

class Organizations {
private:
	string name;
	string office;
	string index;
	string telephone;
	string fax;
	string schet;
	string bank;
	int number_workers;

public:
	// Имя организации
	bool set_name(string org_name)
	{
		if (!(any_of(org_name.begin(), org_name.end(), ::isdigit)))
		{
			name = org_name;
			return true;
		}
		else
		{
			return false;
		}

	}
	// Получение имени
	string get_name()
	{
		return name;
	}
	// Адрес оргинизации
	void set_office(string org_office)
	{
		office = org_office;
	}
	// Получение адреса орг...
	string get_office()
	{
		return office;
	}
	// Индекс
	bool set_index(string org_index)
	{
		if (org_index.length() == 6)
		{
			index = org_index;
			return true;
		}
		else
			return false;
	}
	// Получение индекса
	string get_index()
	{
		return index;
	}
	// Телефон
	void set_telephone(string org_telephone)
	{
		telephone = org_telephone;
	}
	// Получение телефона
	string get_telephone()
	{
		return telephone;
	}
	// Факс
	void set_fax(string org_fax)
	{
		fax = org_fax;
	}
	// Получение факса
	string get_fax()
	{
		return fax;
	}
	// Счёт
	void set_schet(string org_schet)
	{
		schet = org_schet;
	}
	// Получение счёта
	string get_schet()
	{
		return schet;
	}
	// Имя банка
	void set_bank(string org_bank)
	{
		bank = org_bank;
	}
	// Получение имени банка
	string get_bank()
	{
		return bank;
	}

	//Число сотрудников банка
	void set_number_workers(int number)
	{
		number_workers = number;
	}

	//Получение числа сотрудников
	int get_number_workers()
	{
		return number_workers;
	}


};

void Menu()
{
	cout << "1.Ввести организацию: " << endl;
	cout << "2.Вывести организацию на экран: " << endl;
}


int main()
{
	setlocale(LC_ALL, "Rus");

	Organizations organization;

	string name;
	string office;
	string index;
	string telephone;
	string fax;
	string schet;
	string bank;
	int number_workers;

	for (int i = 0;; i++)
	{
		Menu();

		short N = 0;
		cin >> N;
		switch (N)
		{
			// Интерфейс ввода пользователя
		case 1:
			cout << "Название организации: ";
			cin >> name;

			if (!organization.set_name(name))
			{
				cout << "Error" << endl;
				cin >> name;
			}

			cout << "Адрес(город,ул., дом):  ";
			cin >> office;

			cout << "Индекс: ";
			cin >> index;
			if (!organization.set_index(index))
			{
				cout << "Error" << endl;
				cin >> index;
			}


			cout << "Телефон: ";
			cin >> telephone;


			cout << "Факс: ";
			cin >> fax;


			cout << "Зарплата: ";
			cin >> schet;


			cout << "Название банка: ";
			cin >> bank;


			cout << "Число сотрудников: ";
			cin >> number_workers;


			organization.set_office(office);
			organization.set_index(index);
			organization.set_telephone(telephone);
			organization.set_fax(fax);
			organization.set_schet(schet);
			organization.set_bank(bank);
			organization.set_number_workers(number_workers);
			break;
		case 2:

			// Вывод данных
			cout << "Название организации: " << organization.get_name() << endl;

			cout << "Почтовый адрес: " << organization.get_office() << endl;

			cout << "Индекс: " << organization.get_index() << endl;

			cout << "Телефон: " << organization.get_telephone() << endl;

			cout << "Факс: " << organization.get_fax() << endl;

			cout << "Зарплата: " << organization.get_schet() << endl;

			cout << "Банк: " << organization.get_bank() << endl;

			cout << "Число сотрудников:" << organization.get_number_workers() << endl;
			break;

		default:
			cout << "Выберете пункт из меню..." << endl;
		}
	}

	system("pause");
	return 0;
}
