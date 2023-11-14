# Mini-Project
## ANALYSIS OF THE DETAILS OF INDUSTRY
## Aim:
Analysis of the details of a industry.

## ALGORITHM:

Step:1 Importing necessary packages.

Step:2 Read the data set.

Step:3 Execute the methods.

Step:4 Run the program.

Step:5 Get the output.

## CODE AND OUTPUT:

```python
import pandas as pd
df = pd.read_csv("dataset.csv")
df.head(4)
```

![Screenshot 2023-11-14 111759](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/b1450f73-58a5-4eed-af7f-6f18b12918c6)

```python
df.info()
```

![Screenshot 2023-11-14 111913](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/327ea939-663b-489f-b945-da44f84a4f7d)

```python
df.dropna(how='all').shape
```

![Screenshot 2023-11-14 112003](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/a99055d4-86b2-4125-86f8-bf0ba325fbd0)

```python
exp = [13,23,28,12,5,9,31,26,10,19,22,24,29,4,25,30]
af=pd.DataFrame(exp)
af
```

![Screenshot 2023-11-14 112037](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/9e05fde8-d8d7-4872-865b-1fc0d9d67900)

```python
q1=af.quantile(0.25)
q2=af.quantile(0.5)
q3=af.quantile(0.75)
iqr=q3-q1

low=q1-1.5*iqr
low
```

![Screenshot 2023-11-14 112110](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/2d9d318f-a746-42be-b038-d9281ca1d75b)

```python
high=q1+1.5*iqr
high
```

![Screenshot 2023-11-14 112144](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/74965f3a-88d5-4a8b-88ca-28f5201be2cd)

```python
correlation_matrix = data.corr()
plt.figure(figsize=(8, 6))
sns.heatmap(correlation_matrix, annot=True, cmap="coolwarm")
plt.title("Variable_name")
plt.show()
```

![5](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/9773d9d5-5a54-4320-8959-5e3a22cf33a2)

```python
sns.histplot(x='Variable_name',data=df)
```
![image](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/192bd3ad-a77f-44fa-8728-b7c539c1f400)
```python
plt.figure(figsize=(8, 4))
sns.boxplot(data=data, x='ID', color='lightcoral')
plt.title('Position Boxplot')
plt.xlabel('ID')
plt.show()
```
![1](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/44af0e9b-e316-49b7-b720-7ca7dc96d222)
```python
plt.figure(figsize=(10, 4))
sns.countplot(data=data, x='Desig', palette='Set2')
plt.title('Desig Counts')
plt.xlabel('Desig')
plt.ylabel('Count')
plt.show()
```

![2](https://github.com/lokeshrahulv/Mini-Project/assets/118423842/df39bb3f-8a8c-4a9a-8659-0fc2c76b04d0)

## RESULT:
Hence the program to analyze the data set using data science is applied sucessfully.
