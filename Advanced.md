            Java Advanced Programming 
- Generic : is used for 2 purposes are making our code flexible and get rid of compile time issues.
- Generic class : it mean that you create a class , an only provide the class type when you called it . if you don't call it then no need to provide the type.
- upper bounded wildcard(? extends Number)  : it means that smaller(integer) than number can use it.
- lower bounded wildcard(? super Integer) : it means that equal or greater than integer can use it.
- unbounded(?) : anything


            FunctionalInterface or SAM(Singe Abstract Method) : have only one abstract method.
- in interface althought you have a lot of methods , but among that you have only one abstract method , so it also called that 
interface a SAM.


            Interface Function<T,R>(This is a functional interface and can therefore be used as the assignment 
target for a lambda expression or method reference.)
- Type Parameters:
    - T - the type of the input to the function
    - R - the type of the result of the function
* Function<T,R>: Represents a function that accepts one argument and produces a result.And the abstract method in Function<T,R> is apply();

+ Method Summary
All Methods 
Modifier and Type	                                               Method and Description

default <V> Function<T,V>	                                       andThen(Function<? super R,? extends V> after)
                                                                   Returns a composed function that first applies this function to its input, and then applies the after function to the result.

R	                                                               apply(T t)
                                                                   Applies this function to the given argument.

default <V> Function<V,R>	                                       compose(Function<? super V,? extends T> before)
                                                                   Returns a composed function that first applies the before function to its input, and then applies this function to the result.

static <T> Function<T,T>	                                       identity()
                                                                   Returns a function that always returns its input argument.
Method Detail
- apply
R apply(T t)
Applies this function to the given argument.
Parameters:
t - the function argument
Returns:
the function result

- compose
default <V> Function<V,R> compose(Function<? super V,? extends T> before)
Returns a composed function that first applies the before function to its input, and then applies this function to the result. If evaluation of either function throws an exception, it is relayed to the caller of the composed function.
Type Parameters:
V - the type of input to the before function, and to the composed function
Parameters:
before - the function to apply before this function is applied
Returns:
a composed function that first applies the before function and then applies this function
Throws:
NullPointerException - if before is null
See Also:
andThen(Function)

- andThen
default <V> Function<T,V> andThen(Function<? super R,? extends V> after)
Returns a composed function that first applies this function to its input, and then applies the after function to the result. If evaluation of either function throws an exception, it is relayed to the caller of the composed function.
Type Parameters:
V - the type of output of the after function, and of the composed function
Parameters:
after - the function to apply after this function is applied
Returns:
a composed function that first applies this function and then applies the after function
Throws:
NullPointerException - if after is null
See Also:
compose(Function)

- identity
static <T> Function<T,T> identity()
Returns a function that always returns its input argument.
Type Parameters:
T - the type of the input and output objects to the function
Returns:
a function that always returns its input argument