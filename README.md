# SIMPLE-PATTERN-IN-C-
#include <iostream>
using namespace std;

void
pattern1 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= i; j++)
		{
		  cout << "*";
		}
	  cout << endl;
	}
}

void
pattern2 (int n)
{
  for (int i = n; i >= 1; i--)
	{
	  for (int j = i; j > 0; j--)
		{
		  cout << "*";
		}
	  cout << endl;
	}
}

void
pattern3 (int n)
{
  for (int i = n; i >= 1; i--)
	{
	  for (int j = 1; j <= i; j++)
		{
		  cout << "*";
		}
	  cout << endl;
	}
}

void
pattern4 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  for (int k = 1; k <= i; k++)
		{
		  cout << "*";
		}
	  cout << endl;
	}
}

//****digit Pattern****
void
digitpattern1 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= i; j++)
		{
		  cout << i;
		}
	  cout << endl;
	}
}

void
digitpattern2 (int n)
{
  for (int i = n; i >= 1; i--)
	{
	  for (int j = 1; j <= i; j++)
		{
		  cout << (n - i + 1);
		}
	  cout << endl;
	}
}

void
digitpattern3 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  for (int k = 1; k <= i; k++)
		{
		  cout << i;
		}
	  cout << endl;
	}
}

void
digitpattern4 (int n)
{
  for (int i = n; i >= 1; i--)
	{
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  for (int k = 1; k <= i; k++)
		{
		  cout << (n - i + 1);
		}
	  cout << endl;
	}
}

void
digitpattern5 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= (n + 1 - i); j++)
		{
		  cout << j << " ";
		}
	  cout << endl;
	}
}

void
digitpattern6 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= i; j++)
		{
		  if ((i + j) % 2 == 0)
			{
			  cout << 1;
			}
		  else
			{
			  cout << 0;
			}
		}
	  cout << endl;
	}
}

void
printRhombus (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  // Print leading spaces
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  // Print stars
	  for (int j = 1; j <= n; j++)
		{
		  cout << "*";
		}
	  cout << endl;
	}
}

void
digitpattern8 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  for (int j = 1; j <= n; j++)
		{
		  cout << j;
		}
	  cout << endl;
	}
}

void
digitpattern9 (int n)
{
  for (int i = 1; i <= n; i++)
	{
	  for (int j = 1; j <= n - i; j++)
		{
		  cout << " ";
		}
	  for (int j = i; j > 1; j--)
		{
		  cout << j;
		}
	  for (int j = 2; j <= i; j++)
		{
		  cout << j;
		}
	  cout << endl;
	}
}
void pattern5(int n)
{
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<=n-i;j++)
        {
            cout<<" ";
        }
        for(int j=1;j<=(2*i-1);j++)
        {
            cout<<"*";
        }
        cout<<endl;
    }
    for(int i=n;i>=1;i--)
    {
        for(int j=1;j<=n-i;j++)
        {
            cout<<" ";
        }
        for(int j=1;j<=(2*i+1);j++)
        {
            cout<<"*";
        }
        cout<<endl;
    }
}
void pattern6(int n)
{
    for(int i=1;i<=3;i++)
    {
        for(int j=1;j<=n;j++)
        {
            if(((i+j)%4==0) || ((i==2) || (j%4==0)))
            {
                cout<<"*";
            }
            else{
                cout<<" ";
            }
        }
        cout<<endl;
    }
}

int
main ()
{
  int n;
  cout << "Enter the digit: "<<endl;
  cin >> n;

  cout << "Pattern 1" << endl;
  pattern1 (n);
  cout << endl;

  cout << "Pattern 2" << endl;
  pattern2 (n);
  cout << endl;

  cout << "Pattern 3" << endl;
  pattern3 (n);
  cout << endl;

  cout << "Pattern 4" << endl;
  pattern4 (n);
  cout << endl;

  cout << "digitpattern1" << endl;
  digitpattern1 (n);
  cout << endl;

  cout << "digitpattern2" << endl;
  digitpattern2 (n);
  cout << endl;

  cout << "digitpattern3" << endl;
  digitpattern3 (n);
  cout << endl;

  cout << "digitpattern4" << endl;
  digitpattern4 (n);
  cout << endl;
  cout << " digitpattern5" << endl;
  digitpattern5 (n);
  cout << endl;
  cout << " digitpattern6" << endl;
  digitpattern6 (n);
  cout << endl;
  cout << " digitpattern7" << endl;
  printRhombus (n);
  cout << endl;
  cout << " digitpattern8" << endl;
  digitpattern8 (n);
  cout << "digitpattern9" << endl;
  digitpattern9 (n);
  cout << endl;
  cout<<"pattern 5"<<endl;
  pattern5(n);
  cout<<endl;
  cout<<"pattern6"<<endl;
  pattern6(n);
  cout<<endl;
  return 0;
}
