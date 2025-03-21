# Databricks

# Description du projet et attendus 
Le ministre de l’Enseignement supérieur cherche un Data Analyste afin d’exploiter leurs data(s)
Le besoin est formulé comment suit
# Partie1 : Load Data
## Question1 :
def getEtudiantsAndProf(path: String):Seq[DataFrame]
Cette fonction lit un fichier JSON et retourne deux DataFrames, un qui contient les informations des étudiants qui ont perçu une bourse excellence et un autre celles des professeurs récompensés

# Partie 2 Agrégation simple
## Question1 :
def SumBourseByNivAndUniv(df:DataFrame):DataFrame
Cette fonction calcule la somme d’argent versée par Niveau d’étude pour chaque université
## Question2 :
def CountBourseUnivEachYear(df:DataFrame):DataFrame
Cette fonctionne calcule le nombre de bourse donné dans une université pour chaquee années

# Partie3 agrégation avec windows partition
## Question1 :
def TopOnBourseForUnivEachYear(df:DataFrame):DataFrame
Donne les informations de l’etudiant qui perçu la somme d’argent la plus importante pour chaque
université lors d’une année
## Question2 :
def DiffBetwMinAndNex(df:DataFrame):DataFrame
Calcule l’écart de bourse pour chaque année entre le plus petit et le suivant (plus proche)

# Partie 4 Agrégation Combinée
## Question 1 :
def CubeUniversiteAndAnnee (df:DataFrame):DataFrame
Fait une agrégation combinée de l’année et université en utilisant le fonction cube

## Question 2 :
a) Réaliser le graphe de la question Question1 en utilisant l’Api SQL
b) Tirez une conclusion

# Partie5 Cross data
## Question 1 :
def CheckProfRecomp(dfEtu:DataFrame, dfProf:DataFrame):DataFrame
La fonction fait la jointure du Dataframe etudiant et celui de prof afin de savoir quel est l’id du prof
récompensé pour chaque étudiant
Si l’étudiant n’a pas de prof récompensé la valeur de l’idProf sera ProfS_No_Recompensés

