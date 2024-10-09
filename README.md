
 
### Hi there, I'm [Luis Carreño](https://lcarrenoy.github.io) 👋

- Bachelor of Science in Industrial Engineer from [UNI](https://portal.uni.edu.pe/#1), Perú. 
- Languages: Português, English and Spanish
  

**I’m interested in**:
 -  Web Development (Javascript, HTML and CSS)
 -  Programming (R, Python and SQL)
 -  Databases (SQL)
 -  Machine Learning and Artificial Intelligence
 -  Data visualization (Power BI, Tableau and Data Studio)
 -  Finance
  
## Skills:
#### Languages programming and tools:

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white) 
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white).
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white)&nbsp;


   "source": [
        "<a href=\"https://colab.research.google.com/github/ad17171717/YouTube-Tutorials/blob/main/Google%20Colab%20Tutorials/Exporting%20to%20a%20PDF%20Format/Google_Colab_Exporting_to_a_PDF_Format!.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"

{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyMcdXYvI0Jz+n3jsVw8oyxA",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
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
        "<a href=\"https://colab.research.google.com/github/ad17171717/YouTube-Tutorials/blob/main/Google%20Colab%20Tutorials/Exporting%20to%20a%20PDF%20Format/Google_Colab_Exporting_to_a_PDF_Format!.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# **nbconvert**\n",
        "\n",
        "**The `nbconvert` tool allows you to convert a Jupyter `.ipynb` notebook file into another static format such as: HTML, LaTeX, PDF, Markdown and more.**"
      ],
      "metadata": {
        "id": "rcUjvq5MP26_"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "<sup>Source: [Convert Notebooks to other formats](https://nbconvert.readthedocs.io/en/latest/) from nbconvert Documentation</sup>"
      ],
      "metadata": {
        "id": "eN3UVgZpQDqH"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## **Method I - Convert notebook to HTML then print as PDF**"
      ],
      "metadata": {
        "id": "Nc081PyiQDzu"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "!jupyter nbconvert --to html /content/KNN.ipynb"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "QyRG0nsrQLCu",
        "outputId": "a6376269-c3f5-4845-d790-835426e7004b"
      },
      "execution_count": 1,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[NbConvertApp] Converting notebook /content/KNN.ipynb to html\n",
            "[NbConvertApp] Writing 1553619 bytes to /content/KNN.html\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## **Method II - Convert notebook directly as a PDF**"
      ],
      "metadata": {
        "id": "28DB2WQUQLJO"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "!sudo apt-get install texlive-xetex texlive-fonts-recommended texlive-plain-generic"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0nRxT2YRQLSO",
        "outputId": "ab355536-34f0-4daa-b3e6-c48a0e4cf228"
      },
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Reading package lists... Done\n",
            "Building dependency tree       \n",
            "Reading state information... Done\n",
            "texlive-fonts-recommended is already the newest version (2019.20200218-1).\n",
            "texlive-plain-generic is already the newest version (2019.202000218-1).\n",
            "texlive-xetex is already the newest version (2019.20200218-1).\n",
            "0 upgraded, 0 newly installed, 0 to remove and 34 not upgraded.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "!jupyter nbconvert --to pdf /content/KNN.ipynb"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "q2xH3xSgQSR3",
        "outputId": "e4da07de-f08f-452e-ae7b-15ce203edf1f"
      },
      "execution_count": 3,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[NbConvertApp] Converting notebook /content/KNN.ipynb to pdf\n",
            "[NbConvertApp] Support files will be in KNN_files/\n",
            "[NbConvertApp] Making directory ./KNN_files\n",
            "[NbConvertApp] Making directory ./KNN_files\n",
            "[NbConvertApp] Making directory ./KNN_files\n",
            "[NbConvertApp] Making directory ./KNN_files\n",
            "[NbConvertApp] Making directory ./KNN_files\n",
            "[NbConvertApp] Writing 62577 bytes to notebook.tex\n",
            "[NbConvertApp] Building PDF\n",
            "[NbConvertApp] Running xelatex 3 times: ['xelatex', 'notebook.tex', '-quiet']\n",
            "[NbConvertApp] Running bibtex 1 time: ['bibtex', 'notebook']\n",
            "[NbConvertApp] WARNING | bibtex had problems, most likely because there were no citations\n",
            "[NbConvertApp] PDF successfully created\n",
            "[NbConvertApp] Writing 671417 bytes to /content/KNN.pdf\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# **References and Additional Learning**"
      ],
      "metadata": {
        "id": "riGJ53jdRgcG"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## **Websites**\n",
        "\n",
        "- **[Convert Notebooks to other formats](https://nbconvert.readthedocs.io/en/latest/) from nbconvert Documentation**\n",
        "\n",
        "- **[Installing TeX](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex) from nbconvert Documentation**"
      ],
      "metadata": {
        "id": "h6QzfPO9Rixm"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "# **Connect**\n",
        "- **Feel free to connect with Adrian on [YouTube](https://www.youtube.com/channel/UCPuDxI3xb_ryUUMfkm0jsRA), [LinkedIn](https://www.linkedin.com/in/adrian-dolinay-frm-96a289106/), [Twitter](https://twitter.com/DolinayG), [GitHub](https://github.com/ad17171717), [Medium](https://adriandolinay.medium.com/) and [Odysee](https://odysee.com/@adriandolinay:0). Happy coding!**"
      ],
      "metadata": {
        "id": "XIHuE48QR2GH"
      }
    }
  ]
}
