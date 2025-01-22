{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "a4761088-a52b-487b-bd20-0492068c2b7d",
   "metadata": {},
   "outputs": [],
   "source": [
    "print(\"kalai is a baad boy\")"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "a820766c-7153-411c-ade7-ec0936a53e53",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter a number:\"))\n",
    "s=0\n",
    "while(n>0):\n",
    "    digit=n%10\n",
    "    s=s+digit\n",
    "    n=n//10\n",
    "print(\"sum of digits is:\",s)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "cf2e2f45-ff2a-40ff-a3b2-760ae9973395",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter a number:\"))\n",
    "p=1\n",
    "while(n>0):\n",
    "    digit=n%10\n",
    "    p=p*digit\n",
    "    n=n//10\n",
    "print(\"product of digits is:\",p)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "53623c46-0c45-4eef-9c7b-3adc5680bb3b",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter a number:\"))\n",
    "p=1\n",
    "for i in str(n):\n",
    "    p=p*int(i)\n",
    "print(\"product of digits is:\",p)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "b901c11e-2c0a-455f-8570-45c9cea11d60",
   "metadata": {},
   "outputs": [],
   "source": [
    "a=0\n",
    "for i in range(1,50):\n",
    "    if(i%2==1):\n",
    "        a=a+i\n",
    "print(\"Sum of odd number is \",a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "15033292-ec6c-466c-b208-b7fbc79e32bf",
   "metadata": {},
   "outputs": [],
   "source": [
    "a=0\n",
    "for i in range(1,50):\n",
    "    if(i%2==0):\n",
    "        a=a+i\n",
    "print(\"Sum of even number is \",a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "74a97353-436c-4914-a9a4-f9b4db438848",
   "metadata": {},
   "outputs": [],
   "source": [
    "a=int(input(\"enter a number\"))\n",
    "s=0\n",
    "for i in range(1,a+1):\n",
    "    s=s+i\n",
    "print(\"n natural numbers\",s)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "f0603265-49cd-417b-a401-55ee271aecd4",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter a number:\"))\n",
    "s=0\n",
    "while(n>0):\n",
    "    rev=n%10\n",
    "    s=s*10+rev\n",
    "    n=n//10\n",
    "print(\"reverse:\",s)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "87859671-5783-4be9-a077-b654795ba822",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter the number\"))\n",
    "a=1\n",
    "for i in range(1,n+1):\n",
    "    a=a*i\n",
    "print(\"factorial\",a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "415409cf-1bbb-4ab8-9bfd-4039bfea4092",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter the number\"))\n",
    "for i in range(1,n+1):\n",
    "    if n%i==0:\n",
    "        +print(i)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "38d42920-bf2f-4f83-8d2a-1323af74d451",
   "metadata": {},
   "outputs": [],
   "source": [
    "def sum_of_digits(n):\n",
    "    s=0\n",
    "    while(n>0):\n",
    "        digit=n%10\n",
    "        s=s+digit\n",
    "        n=n//10\n",
    "    return s\n",
    "n=int(input(\"enter a number\"))\n",
    "print(sum_of_digits(n))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "03a496ae-ba8d-4aa6-bb22-b33246c0e21e",
   "metadata": {},
   "outputs": [],
   "source": [
    "n=int(input(\"enter the number\"))\n",
    "factor_list=[]\n",
    "for i in range(1,n+1):\n",
    "    if n%i==0:\n",
    "        factor_list.append(i)\n",
    "print(factor_list)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "id": "7840e089-de68-4eb8-b07a-51cc0217f6d1",
   "metadata": {},
   "outputs": [
    {
     "name": "stdin",
     "output_type": "stream",
     "text": [
      "enter a number 10\n"
     ]
    },
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[1, 2, 5, 10]\n"
     ]
    }
   ],
   "source": [
    "def factor(n):\n",
    "    factor_list=[]\n",
    "    for i in range(1,n+1):\n",
    "        if n%i==0:\n",
    "            factor_list.append(i)\n",
    "    return(factor_list)\n",
    "n=int(input(\"enter a number\"))\n",
    "print(factor(n))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "23350a82-b152-479e-87c4-a207cf8417c0",
   "metadata": {},
   "outputs": [
    {
     "name": "stdin",
     "output_type": "stream",
     "text": [
      "enter a number 7\n"
     ]
    },
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "True\n"
     ]
    }
   ],
   "source": [
    "def prime(n):\n",
    "    return(factor(n)==[1,n])\n",
    "n=int(input(\"enter a number\"))\n",
    "print(prime(n))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "b18d3799-acf0-4f08-a85f-f3358388f0c7",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python [conda env:base] *",
   "language": "python",
   "name": "conda-base-py"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
