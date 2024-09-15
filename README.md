// C++ code
//
int counter;

int counter2;

int counter3;

void setup()
{
  pinMode(7, OUTPUT);
  pinMode(1, OUTPUT);
  pinMode(3, OUTPUT);
  pinMode(4, OUTPUT);
  pinMode(2, OUTPUT);
  pinMode(8, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(6, OUTPUT);
}

void loop()
{
  digitalWrite(7, HIGH);
  digitalWrite(1, HIGH);
  digitalWrite(3, HIGH);
  delay(5000); // Wait for 5000 millisecond(s)
  digitalWrite(7, LOW);
  for (counter = 0; counter < 4; ++counter) {
    digitalWrite(4, HIGH);
    delay(500); // Wait for 500 millisecond(s)
    digitalWrite(4, LOW);
    delay(500); // Wait for 500 millisecond(s)
  }
  digitalWrite(1, LOW);
  digitalWrite(3, LOW);
  digitalWrite(2, HIGH);
  digitalWrite(3, HIGH);
  digitalWrite(8, HIGH);
  delay(5000); // Wait for 5000 millisecond(s)
  digitalWrite(8, LOW);
  for (counter2 = 0; counter2 < 4; ++counter2) {
    digitalWrite(5, HIGH);
    delay(500); // Wait for 500 millisecond(s)
    digitalWrite(5, LOW);
    delay(500); // Wait for 500 millisecond(s)
  }
  digitalWrite(2, LOW);
  digitalWrite(3, LOW);
  digitalWrite(9, HIGH);
  digitalWrite(1, HIGH);
  digitalWrite(2, HIGH);
  delay(5000); // Wait for 5000 millisecond(s)
  digitalWrite(9, LOW);
  for (counter3 = 0; counter3 < 4; ++counter3) {
    digitalWrite(6, HIGH);
    delay(500); // Wait for 500 millisecond(s)
    digitalWrite(6, LOW);
    delay(500); // Wait for 500 millisecond(s)
  }
  digitalWrite(2, LOW);
  digitalWrite(1, LOW);
}
