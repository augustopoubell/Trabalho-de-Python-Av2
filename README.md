# Trabalho-de-Python-Av2
Um trabalho que vale ponto!
Integrantes: 
Augusto Poubell Ribeiro Pinheiro de Souza   202103132881

Evellyn Ramos de Lira   202109410032

Nathan de Medeiros Moreira 202103059171

Maria Eduarda Soares Costa  202203657569  


 Primeiro código do trabalho: 


class Funcionario:
    def __init__(self, nome, idade, salario):
        self.nome = nome
        self.idade = idade
        self.salario = salario

class Atendente(Funcionario):
    def __init__(self, nome, idade, salario, setor):
        super().__init__(nome, idade, salario)
        self.setor = setor
    def atender_paciente(self):
        print("Atendendo paciente")

class PessoalLimpeza(Funcionario):
    def __init__(self, nome, idade, salario, setor):
        super().__init__(nome, idade, salario)
        self.setor = setor
    def limpar_setor(self):
        print("Limpando setor")

class Enfermeiro(Funcionario):
    def __init__(self, nome, idade, salario, coren):
        super().__init__(nome, idade, salario)
        self.coren = coren
    def cuidar_paciente(self):
        print("Cuidando do paciente")

class Medico(Funcionario):
    def __init__(self, nome, idade, salario, crm):
        super().__init__(nome, idade, salario)
        self.crm = crm
    def realizar_atendimento(self):
        pass

class ClinicoGeral(Medico):
    def __init__(self, nome, idade, salario, crm, especialidade):
        super().__init__(nome, idade, salario, crm)
        self.especialidade = especialidade
    def realizar_diagnostico(self):
        print("Realizando diagnóstico")

class Ortopedista(Medico):
    def __init__(self, nome, idade, salario, crm, especialidade):
        super().__init__(nome, idade, salario, crm)
        self.especialidade = especialidade
    def realizar_cirurgia(self):
        print("Realizando cirurgia")

class Pediatra(Medico):
    def __init__(self, nome, idade, salario, crm, especialidade):
        super().__init__(nome, idade, salario, crm)
        self.especialidade = especialidade
    def examinar_crianca(self):
        print("Examinando criança") 



Segundo código do trabalho:  

class Person:
    def __init__(self, name, age, gender):
        self.name = name
        self.age = age
        self.gender = gender
        
class MedicalProfessional(Person):
    def __init__(self, name, age, gender, specialty):
        super().__init__(name, age, gender)
        self.specialty = specialty
        
    def perform_consultation(self, patient):
        print(f'{self.specialty} {self.name} is performing a consultation on {patient.name}.')
        
    def perform_diagnosis(self, patient):
        print(f'{self.specialty} {self.name} is performing a diagnosis on {patient.name}.')
        
    def perform_surgery(self, patient):
        print(f'{self.specialty} {self.name} is performing a surgery on {patient.name}.')
        
class Doctor(MedicalProfessional):
    def __init__(self, name, age, gender, specialty, degree):
        super().__init__(name, age, gender, specialty)
        self.degree = degree
        
    def prescribe_medication(self, patient, medication):
        print(f'{self.specialty} {self.name} is prescribing {medication} to {patient.name}.')
        
class Nurse(Person):
    def __init__(self, name, age, gender, certification):
        super().__init__(name, age, gender)
        self.certification = certification
        
    def take_vital_signs(self, patient):
        print(f'{self.name} is taking vital signs for {patient.name}.')
        
    def administer_medication(self, patient, medication):
        print(f'{self.name} is administering {medication} to {patient.name}.')

Nessa atualização do código, foram incluídas duas classes para enfermeiros: a classe Nurse e seus respectivos métodos take_vital_signs e administer_medication. A classe Nurse herda da classe Person e possui um atributo adicional chamado certification, que representa a certificação do enfermeiro.
Para acessar o código completo, você pode encontrá-lo neste repositório público do GitHub:  https://github.com/augustopoubell/Trabalho-Est-cio-Python/compare/main...augustopoubell-patch-1?quick_pull=1

