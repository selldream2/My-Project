### print in monitor window

```
int delayTime = 500;

void setup() {
  // put your setup code here, to run once:
  
  Serial.begin(9600);

}

void loop() {
  // put your main code here, to run repeatedly:

  Serial.println("Hello, Arduino");
  delay(delayTime);

}
```

### combine string and print

```
int delayTime = 500;
String name = "BH Lee";

void setup() {
  // put your setup code here, to run once:
  
  Serial.begin(9600);

}

void loop() {
  // put your main code here, to run repeatedly:

  Serial.print("Hello, Arduino! ");
  Serial.print("I'm ");
  Serial.print(name);
  Serial.print(".");
  Serial.println("");

  delay(delayTime);

}
```

### area calculation

```
int delayTime = 500;

float pi = 3.14;
float radius = 2.;
float area;

void setup() {
  // put your setup code here, to run once:
  
  Serial.begin(9600);

}

void loop() {
  // put your main code here, to run repeatedly:

  area = sq(radius) * pi;

  Serial.print("Circle area with radis = ");
  Serial.print(radius);
  Serial.print(" is ");
  Serial.println(area);

  delay(delayTime);

}
```




