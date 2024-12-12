# Semana-10-Testes-de-software


from numeroromano import converte
import unittest

class TestConverteNumerosRomanos(unittest.TestCase):

    def testeI(self):
        self.assertEqual(converte("I"), 1)

    def testeV(self):
        self.assertEqual(converte("V"), 5)

    def testeII(self):
        self.assertEqual(converte("II"), 2)

    def testeXXII(self):
        self.assertEqual(converte("XXII"), 22)

    def testeIX(self):
        self.assertEqual(converte("IX"), 9)

    def testXXIV(self):
        self.assertEqual(converte("XXIV"), 24)

if __name__ == "__main__":
    
    unittest.main()
