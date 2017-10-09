# IS590PR Assignment	3:		Improving	the	WordMath	class - WordMath

Topics	and	skills	involved:
• Modifying	others’	code	and	committing changes	to	a	repository.
• Writing	and	running	Doctests

1. In	calc_operation(),	the	series	of	if	statements	are	mutually	exclusive	possibilities.	Improve	it	by	
properly	using	“elif”	where	it	makes	sense.

2. Notice	the	gray	underline	on	the	calc_operation()	method	name.		Hover	over	it	and	see	the	notice	
“calc_operation()	may	be	static”.		This	occurs	because	it	does	not	reference	any	class	instance
attributes.		Notice	also	that	most	of	the	other	methods	are	already	declared	as	static.		Change	this	one	
accordingly,	and	you’ll	have	to	also	correct	the	way	it	gets	called	elsewhere.

3. Most	of	the	methods	already	have	Doctests,	but	we	need	a	few	more.		Using	the	feature	“Run	Doctests	
in	word_math.py	with	Coverage”	we	can	see	that	it	currently	has	87%	coverage.		Scroll	through	the	
code	edit	window	afterward	and	you	can	tell	from	the	green	and	red	bars	next	to	the	line	numbers,	
which	lines	did	not	get	tested	at	all.		This	example	shows	a	very	common	pattern	to	which	ones	are	not	
being	tested	– it’s	mostly	the	edge	case	or	exceptional	situations	that	are	missing	tests.	So,	add	more	
test	cases	to	take	care	of	this.

4. You	might	also	notice	from	the	test	coverage	that	although	calc_operations()	tries	to	support	
exponentiation,	it	is	not	yet	supported	elsewhere	in	the	code,	so	we	can’t	use	it.		Add	support	and	tests	
for	that	so	it	will	properly	evaluate	expressions	such	as	‘two	exponent	three’	or	‘two	power	of	three’	to	
compute	8.

5. This	WordMath	is	very	limited	in	range.		It	can’t	handle	any	word	numbers	larger	than	“ninety	nine”.		
Following	the	structure	already	in	place,	expand	it	to	handle	numbers	in	the	hundreds	(anything	up	to	
“nine	hundred	ninety	nine”).	
