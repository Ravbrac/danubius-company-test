# Danubius Test

## Short questions

- What is GIT? What is it used for and what kind of
situations is it designed to solve/make it easier?

A: GIT is used for version control, a way, developers can share their codes and work on projects together, allowing them to constantly
update both
projects still in progress and finished ones too.

- What is HTTP? What kind of HTTP methods are you
familiar with? What are their characteristics?

A: HTTP is a hypertext protocol, used for performing different internet methods, like reading (GET), creating (POST), updating (PUT) or
deleting (DELETE) certain web contents.

- What is the difference between HTTP and HTTPS?

A: The 'S' stands for 'Secure' in HTTPS, meaning it's a more secure (encrypted) version of the HTTP protocol.

- What do you know about the following HTML tags?
What are their characteristics and when do we use them?
  - `<div>`
  - `<span>`
  - `<p>`
  - `<a href="...">...</a>`

A: `<div>` was the generic dividing tag in HTML before HTML 5, but it's still widely used even today, along with a class attribute usually. 
`<span>` is ment for inline division, `<p>` is stand for 'paragraph', used to divide articles into smaller paragraphs. `<a>` is stands for
'anchor', used for clickable links (unlike the `<link>` tag).

- What do you know about dependency injection?
What is it used for? What is its advantage?

A: dependency injection is used for example in Spring framework to connect a class to other classes which said class depends on, 
for example repository classes to service classes. In Spring, dependency injection is done with the help of annotations.

- Briefly describe a current topic in the IT field
that you are interested in!

## Programming task

Given a table that contains units and multipliers
that belongs to them. The multipliers tell you what
is the number that you need to multiply the value
with if you'd like to calculate the base unit.
The base units for example: liter, meter, etc...
Those that doesn't have a metric prefix.

### Length

| Unit | Value |
|------|-------|
| mm   | 0.001 |
| cm   | 0.01  |
| dm   | 0.1   |
| m    | 1     |
| km   | 1000  |

### Weight

| Unit | Value   |
|------|---------|
| mg   | 0.001   |
| g    | 1       |
| dkg  | 10      |
| kg   | 1000    |
| t    | 1000000 |

### Task

Create a data structure(could be a class but also
any type of combination of primitive types, array,
but also the series of well named variables) which
is suitable to store the values in the table and
makes the implementation of the exercises below easier(You don't have to
implement the actual operations they are just there
as an example).

- List a given type(e.g.: Length) of measurement units.
For example: mm, cm, dm, m, km
- Query of the multipliers.
For example: input -> km, output -> 1000
- Given an actual unit, return the value in the base unit.
For example: input -> "1200 cm", output -> 12

Initialize the datastructure with example inputs.

`java`

public class MeasurementUnit() {
	@Autowired
	private MeasurementService measurementService;
	private double value;
	private double multiplier;
	private String siUnit;
	private UnitType unitType;
	Hashmap<String, double> lengthUnits = new Hashmap<>();
	Hashmap<String, double> weigthUnits = new Hashmap<>();


	Hashmap<String, double> lengthUnits = new Hashmap<>();
	lengthUnits.add("mm", 0.001);
	lengthUnits.add("cm", 0.01);
	lengthUnits.add("dm", 0.1);
	lengthUnits.add("m", 1);
	lengthUnits.add("km", 1000);
	
	lengthUnits.stream
	.forEach(k -> measurementservice.setSIUnit(k))
	
	lengthUnits.stream
	.foreach(v -> measurementService.setMultiplier(v))

	Hashmap<String, double> weigthUnits = new Hashmap<>();
	weigthUnits.add("mg", 0,001);
	weigthUnits.add("g", 1);
	weigthUnits.add("dkg", 10);
	weigthUnits.add("kg", 1000);
	weigthUnits.add("t", 1000000);




