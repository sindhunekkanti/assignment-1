# assignment-1
{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "lekhana.ipynb",
      "provenance": [],
      "collapsed_sections": [],
      "authorship_tag": "ABX9TyNNveJXQnYeSXWUttrA8rgc",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/lekhana262/Assignment1/blob/master/lekhana.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "6R2Gjw1Gxm5-",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 168
        },
        "outputId": "61d0b247-2f43-4784-fd8c-41f4ff9fbc25"
      },
      "source": [
        "#simple calculator\n",
        "def add(num1,num2):\n",
        "  return num1+num2\n",
        "def subtract(num1,num2):\n",
        "  return num1-num2\n",
        "def multiply(num1,num2):\n",
        "   return num1*num2\n",
        "def divide (num1,num2):\n",
        "    return num1/num2\n",
        "print(\"select operation\")\n",
        "print(\"1.add\")\n",
        "print(\"2.subtract\")\n",
        "print(\"3.multiple\") \n",
        "print(\"4.divide\") \n",
        "choice=int(input(\"select operations form 1,2,3,4:\"))\n",
        "num1=int(input(\"enter first number: \")) \n",
        "num2=int(input(\"enter second number: \"))\n",
        "if choice==1:\n",
        "        print(num1, \"+\", num2,\"=\",add(num1,num2)) \n",
        "elif choice==2:\n",
        "        print(num1,\"-\",num2,\"=\",sub(num1,num2))\n",
        "elif choice==3:\n",
        "        print(num1,\"*\",num2,\"=\",mul(num1,num2))\n",
        "elif choice==4:\n",
        "        print(num1,\"/\",num2,\"=\",div(num1,num2))\n",
        "else:\n",
        "        print(\"invalid input\")      "
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "select operation\n",
            "1.add\n",
            "2.subtract\n",
            "3.multiple\n",
            "4.divide\n",
            "select operations form 1,2,3,4:1\n",
            "enter first number: 10\n",
            "enter second number: 2\n",
            "10 + 2 = 12\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "UfdVHbLLTa_1",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 101
        },
        "outputId": "b7829099-fe6e-424d-b00f-9fbe2a20842d"
      },
      "source": [
        "#simple interest\n",
        "def simple_interest(p,t,r):\n",
        "    print('the principle is',p)\n",
        "    print('the time period is',t)\n",
        "    print('the rate of interest is',r)\n",
        "    si=(p*t*r)/100\n",
        "    print('the simple interest is',si)\n",
        "    return si\n",
        "simple_interest(9,7,10)    "
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "the principle is 9\n",
            "the time period is 7\n",
            "the rate of interest is 10\n",
            "the simple interest is 6.3\n"
          ],
          "name": "stdout"
        },
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "6.3"
            ]
          },
          "metadata": {
            "tags": []
          },
          "execution_count": 7
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "xFQvEyvvV6_q",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 50
        },
        "outputId": "be504b41-6c16-4af1-9185-48b58c42a487"
      },
      "source": [
        "#area of circle\n",
        "PI=3.142\n",
        "r=float(input(\"enter the radius of circle:\"))\n",
        "area=PI*(r*r);\n",
        "print(\"%2f\" %area)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter the radius of circle:20\n",
            "1256.800000\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "waucbJp4Xm-v",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 84
        },
        "outputId": "20d62723-ed80-4767-f127-0db7f767c554"
      },
      "source": [
        "#area of  triangle\n",
        "a=float(input('enter first side'))\n",
        "b=float(input('enter second side'))\n",
        "c=float(input('enter third side'))\n",
        "s=(a+b+c)/2\n",
        "area=(s*(s-a)*(s-b)*(s-c))**0.5\n",
        "print('the area of the triangle is %0.2f'%area)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter first side4\n",
            "enter second side6\n",
            "enter third side8\n",
            "the area of the triangle is 11.62\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "0AAhp1Q2Y2mH",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 50
        },
        "outputId": "3ff68056-cabc-4324-81d2-ea2b1badb9cc"
      },
      "source": [
        "#celsius to fahrenheit\n",
        "celsius=float(input(\"enter the temperature in celsius: \"))\n",
        "fahrenheit=(celsius*9/5)+32\n",
        "print('%2f celsius is: %0.2f fahrenheit'%(celsius,fahrenheit))"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter the temperature in celsius: 76\n",
            "76.000000 celsius is: 168.80 fahrenheit\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "OXWcj9igZ6bl",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 67
        },
        "outputId": "0eadb1b0-a61b-42fa-b421-9bc456a4b33c"
      },
      "source": [
        "#area of rectangle\n",
        "width=float(input('enter width of a rectangle: '))\n",
        "height=float(input('enter the height of a rectangle: '))\n",
        "area=width*height\n",
        "print(\"area of rectangle is:%2f\"%area)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter width of a rectangle: 6\n",
            "enter the height of a rectangle: 8\n",
            "area of rectangle is:48.000000\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "k_iRvkNmbWbj",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 67
        },
        "outputId": "00502466-9b5c-4dc1-a826-ba67fce0295a"
      },
      "source": [
        "#perimeter of a square\n",
        "s=int(input(\"side: \"))\n",
        "area=s*s\n",
        "perimeter=4*s\n",
        "print(\"area of square : \",area)\n",
        "print(\"perimeter of square: \",perimeter)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "side: 4\n",
            "area of square :  16\n",
            "perimeter of square:  16\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "AlARqNHSctMF",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 50
        },
        "outputId": "5b589678-1989-437e-a890-789b2376d5ea"
      },
      "source": [
        "#circumferences of a circle\n",
        "import math\n",
        "radius=float(input(\"enter the radius of the circle: \"))\n",
        "circumference=2*math.pi*radius\n",
        "print(\"circumference of the circle is :%.2f\" % circumference)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter the radius of the circle: 12\n",
            "circumference of the circle is :75.40\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "hpQldxDjOpka",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 118
        },
        "outputId": "0acd4de2-8bbe-447f-a2da-0f447f214a27"
      },
      "source": [
        "#swapping of two numbers\n",
        "num1=input('enter first number')\n",
        "num2=input('enter second number')\n",
        "print(\"value of num1 before swapping:\",num1)\n",
        "print(\"value of num2 before swapping:\",num2)\n",
        "temp=num1\n",
        "num1=num2\n",
        "num2=temp\n",
        "print(\"value of num1 after swapping:\",num1)\n",
        "print(\"value of num2 after swapping :\",num2)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "enter first number1\n",
            "enter second number2\n",
            "value of num1 before swapping: 1\n",
            "value of num2 before swapping: 2\n",
            "value of num1 after swapping: 2\n",
            "value of num2 after swapping : 1\n"
          ],
          "name": "stdout"
        }
      ]
    }
  ]
}
