# Effective-Modern-Cpp

A summary of [Scott Meyers' classic "Effective Modern C++"](./Scott%20Meyers-Effective%20Modern%20C++_%2042%20Specific%20Ways%20to%20Improve%20Your%20Use%20of%20C++11%20and%20C++14-O'Reilly%20Media%20(2014).pdf)

## Table Of Contents <a name="top"></a>
1. [The Book](#the-book)
2. [Objective](#objective)
3. [Summary](#summary)
    - 3.1. [1. Deducing Types](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#1-deducing-types)
        - 3.1.1. [Item 1:  Understand template type deduction.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-1-understand-template-type-deduction)
            - [Sample Code](./Item01_Understand_template_type_deduction/CMakeLists.txt)
        - 3.1.2. [Item 2:  Understand auto type deduction.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-2-understand-auto-type-deduction)
            - [Sample Code](./Item02_Understand_auto_type_deduction/CMakeLists.txt)
        - 3.1.3. [Item 3:  Understand decltype.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-3-understand-decltype)
            - [Sample Code](./Item03_Understand_decltype/CMakeLists.txt)
        - 3.1.4. [Item 4:  Know how to view deduced types.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-4-know-how-to-view-deduced-types)
            - [Sample Code](./Item04_Know_how_to_view_deduced_types/CMakeLists.txt)
    - 3.2. [2. auto](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#2-auto)
        - 3.2.1. [Item 5:  Prefer auto to explicit type declarations.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-5--prefer-auto-to-explicit-type-declarations)
            - [Sample Code](./Item05_Prefer_auto_to_explicit_type_declarations/CMakeLists.txt)
        - 3.2.2. [Item 6:  Use the explicitly typed initializer idiom when auto deduces undesired types.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-6--use-the-explicitly-typed-initializer-idiom-when-auto-deduces-undesired-types)
            - [Sample Code](./Item06_Use_the_explicitly_typed_initializer_idiom_when_auto_deduces_undesired_types/CMakeLists.txt)
    - 3.3. [3. Moving to Modern C++](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#3-moving-to-modern-c)
        - 3.3.1. [Item 7:  Distinguish between () and {} when creating objects.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-7--distinguish-between--and--when-creating-objects)
            - [Sample Code](https://github.com/sm2774us/modern_cpp/blob/main/effective_modern_cpp_oreilly_book/Item07_Distinguish_between()_and_%7B%7D_when_creating_objects/CMakeLists.txt)
        - 3.3.2. [Item 8: Prefer nullptr to 0 and NULL.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-8-prefer-nullptr-to-0-and-null)
            - [Sample Code](./Item08_Prefer_nullptr_to_0_and_NULL/CMakeLists.txt)
        - 3.3.3. [Item 9:  Prefer alias declarations to typedefs.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-9--prefer-alias-declarations-to-typedefs)
            - [Sample Code](./Item09_Prefer_alias_declarations_to_typedefs/CMakeLists.txt)
        - 3.3.4. [Item 10:  Prefer scoped enums to unscoped enums.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-10--prefer-scoped-enums-to-unscoped-enums)
            - [Sample Code](./Item10_Prefer_scoped_enums_to_unscoped_enums/CMakeLists.txt)
        - 3.3.5. [Item 11:  Prefer deleted functions to private undefined ones.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-11--prefer-deleted-functions-to-private-undefined-ones)
            - [Sample Code](./Item11_Prefer_deleted_functions_to_private_undefined_ones/CMakeLists.txt)
        - 3.3.6. [Item 12:  Declare overriding functions override.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-12--declare-overriding-functions-override)
            - [Sample Code](./Item12_Declare_overriding_functions_override/CMakeLists.txt)
        - 3.3.7. [Item 13:  Prefer const_iterators to iterators.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-13--prefer-const_iterators-to-iterators)
            - [Sample Code](./Item13_Prefer_const_iterators_to_iterators/CMakeLists.txt)
        - 3.3.8. [Item 14:  Declare functions noexcept if they won’t emit exceptions.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-14--declare-functions-noexcept-if-they-wont-emit-exceptions)
            - [Sample Code](./Item14_Declare_functions_noexcept_if_they_wont_emit_exceptions/CMakeLists.txt)        
        - 3.3.9. [Item 15:  Use constexpr whenever possible.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-15--use-constexpr-whenever-possible)
            - [Sample Code](./Item15_Use_constexpr_whenever_possible/CMakeLists.txt)
        - 3.3.10. [Item 16:  Make const member functions thread safe.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-16--make-const-member-functions-thread-safe)
            - [Sample Code](./Item16_Make_const_member_functions_thread-safe/CMakeLists.txt)
        - 3.3.11. [Item 17:  Understand special member function generation.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-17--understand-special-member-function-generation)
            - [Sample Code](./Item17_Understand_special_member_function_generation/CMakeLists.txt)
    - 3.4. [4. Smart Pointers](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#4-smart-pointers)
        - 3.4.1. [Item 18:  Use std::unique_ptr for exclusive-ownership resource management.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-18--use-stdunique_ptr-for-exclusive-ownership-resource-management)
            - [Sample Code](./Item18_Use_std_unique_ptr_for_exclusive-ownership_resource_management/CMakeLists.txt)        
        - 3.4.2. [Item 19:  Use std::shared_ptr for shared-ownership resource management.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-19--use-stdshared_ptr-for-shared-ownership-resource-management)
            - [Sample Code](./Item19_Use_std_shared_ptr_for_shared-ownership_resource_management/CMakeLists.txt)        
        - 3.4.3. [Item 20:  Use std::weak_ptr for std::shared_ptr-like pointers that can dangle.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-20--use-stdweak_ptr-for-stdshared_ptr-like-pointers-that-can-dangle)
            - [Sample Code](./Item20_Use_std_weak_ptr_for_std_shared_ptr-like_pointers_that_can_dangle/CMakeLists.txt)        
        - 3.4.4. [Item 21:  Prefer std::make_unique and std::make_shared to direct use of new.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-21--prefer-stdmake_unique-and-stdmake_shared-to-direct-use-of-new)
            - [Sample Code](./Item21_Prefer_std_make_unique_and_std_make_shared_to_direct_use_of_new/CMakeLists.txt)        
        - 3.4.5. [Item 22:  When using the Pimpl Idiom, define special member functions in the implementation file.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-22--when-using-the-pimpl-idiom-define-special-member-functions-in-the-implementation-file)
            - [Sample Code](./Item22_When_using_the_Pimpl_Idiom_define_special_member_functions_in_the_implementation_file/CMakeLists.txt)        
    - 3.5. [5. Rvalue References, Move Semantics, and Perfect Forwarding](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#5-rvalue-references-move-semantics-and-perfect-forwarding)
        - 3.5.1. [Item 23:  Understand std::move and std::forward.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-23--understand-stdmove-and-stdforward)
            - [Sample Code](./Item23_Understand_std_move_and_std_forward/CMakeLists.txt)
        - 3.5.2. [Item 24:  Distinguish universal references from rvalue references.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-24--distinguish-universal-references-from-rvalue-references)
            - [Sample Code](./Item24_Distinguish_universal_references_from_rvalue_references/CMakeLists.txt)        
        - 3.5.3. [Item 25:  Use std::move on rvalue references, std::forward on universal references.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-25--use-stdmove-on-rvalue-references-stdforward-on-universal-references)
            - [Sample Code](./Item25_Use_std_move_on_rvalue_references_std_forward_on_universal_references/CMakeLists.txt)        
        - 3.5.4. [Item 26:  Avoid overloading on universal references.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-26--avoid-overloading-on-universal-references)
            - [Sample Code](./Item26_Avoid_overloading_on_universal_references/CMakeLists.txt)        
        - 3.5.5. [Item 27:  Familiarize yourself with alternatives to overloading on universal references.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-27--familiarize-yourself-with-alternatives-to-overloading-on-universal-references)
            - [Sample Code](./Item27_Familiarize_yourself_with_alternatives_to_overloading_on_universal_references/CMakeLists.txt)        
        - 3.5.6. [Item 28:  Understand reference collapsing.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-28--understand-reference-collapsing)
            - [Sample Code](./Item28_Understand_reference_collapsing/CMakeLists.txt)        
        - 3.5.7. [Item 29:  Assume that move operations are not present, not cheap, and not used.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-29--assume-that-move-operations-are-not-present-not-cheap-and-not-used)
            - [Sample Code](./Item29_Assume_that_move_operations_are_not_present_not_cheap_and_not_used/CMakeLists.txt)        
        - 3.5.8. [Item 30:  Familiarize yourself with perfect forwarding failure cases.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-30--familiarize-yourself-with-perfect-forwarding-failure-cases)
            - [Sample Code](./Item30_Familiarize_yourself_with_perfect_forwarding_failure_cases/CMakeLists.txt)        
    - 3.6. [6. Lambda Expressions](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#6-lambda-expressions)
        - 3.6.1. [Item 31:  Avoid default capture modes.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-31--avoid-default-capture-modes)
            - [Sample Code](./Item31_Avoid_default_capture_modes/CMakeLists.txt)        
        - 3.6.2. [Item 32:  Use init capture to move objects into closures.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-32--use-init-capture-to-move-objects-into-closures)
            - [Sample Code](./Item32_Use_init_capture_to_move_objects_into_closures/CMakeLists.txt)        
        - 3.6.3. [Item 33:  Use decltype on auto&& parameters to std::forward them.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-33--use-decltype-on-auto-parameters-to-stdforward-them)
            - [Sample Code](./Item33_Use_decltype_on_autorr_parameters_to_std_forward_them/CMakeLists.txt)        
        - 3.6.4. [Item 34:  Prefer lambdas to std::bind.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-34--prefer-lambdas-to-stdbind)
            - [Sample Code](./Item34_Prefer_lambdas_to_std_bind/CMakeLists.txt)        
    - 3.7. [7. The Concurrency API](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#7-the-concurrency-api)
        - 3.7.1. [Item 35:  Prefer task-based programming to thread-based.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-35--prefer-task-based-programming-to-thread-based)
            - [Sample Code](./Item35_Prefer_task-based_programming_to_thread-based/CMakeLists.txt)        
        - 3.7.2. [Item 36:  Specify std::launch::async if asynchronicity is essential.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-36--specify-stdlaunchasync-if-asynchronicity-is-essential)
            - [Sample Code](./Item36_Specify_std_launch_async_if_asynchronicity_is_essential/CMakeLists.txt)        
        - 3.7.3. [Item 37:  Make std::threads unjoinable on all paths.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-37--make-stdthreads-unjoinable-on-all-paths)
            - [Sample Code](./Item37_Make_std_threads_unjoinable_on_all_paths/CMakeLists.txt)        
        - 3.7.4. [Item 38:  Be aware of varying thread handle destructor behavior.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-38--be-aware-of-varying-thread-handle-destructor-behavior)
        - 3.7.5. [Item 39:  Consider void futures for one-shot event communication.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-39--consider-void-futures-for-one-shot-event-communication)
            - [Sample Code](./Item39)        
        - 3.7.6. [Item 40:  Use std::atomic for concurrency, volatile for special memory.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-40--use-stdatomic-for-concurrency-volatile-for-special-memory)
    - 3.8. [8. Tweaks](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#8-tweaks)
        - 3.8.1. [Item 41:  Consider pass by value for copyable parameters that are cheap to move and always copied.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-41--consider-pass-by-value-for-copyable-parameters-that-are-cheap-to-move-and-always-copied)
        - 3.8.2. [Item 42:  Consider emplacement instead of insertion.](https://github.com/sm2774us/modern_cpp/tree/main/effective_modern_cpp_oreilly_book#item-42--consider-emplacement-instead-of-insertion)
4. [Disclaimer](#disclaimer)

### The Book

[Scott Meyers' classic "Effective Modern C++" - The BOOK in PDF format](./Scott%20Meyers-Effective%20Modern%20C++_%2042%20Specific%20Ways%20to%20Improve%20Your%20Use%20of%20C++11%20and%20C++14-O'Reilly%20Media%20(2014).pdf)

### Objective

The book is awesome and should be read by every C++ developer. I'd like to put a summary here so that every developer can revise it before they go to bed.

### Summary

#### 1. Deducing Types

##### Item 1:  Understand template type deduction.
  
  * During  template  type  deduction, arguments that are references are treated as non-references, i.e., their reference-ness is ignored.
  
  * When deducing types for universal reference parameters, lvalue arguments get special treatment.
  
  * When deducing types for by-value parameters, const and/or volatile arguments are treated as non-const and non-volatile.
  
  * During template type deduction, arguments that are array or function names decay to pointers, unless they’re used to initialize references.

##### Item 2:  Understand auto type deduction.

  * auto type deduction is usually the same as template type deduction, but auto type deduction assumes that a braced initializer represents a  std::initializer_list, and template type deduction doesn’t.

  * auto in a function return type or a lambda parameter implies template type deduction, not auto type deduction

##### Item 3:  Understand decltype.

  * decltype almost always yields the type of a variable or expression without any modifications.

  * For lvalue expressions of type T other than names, decltype always reports a type of T&.

  * C++14 supports decltype(auto), which, like auto, deduces a type from its initializer, but it performs the type deduction using the decltype rules.

##### Item 4:  Know how to view deduced types.
  
  * Deduced types can often be seen using IDE editors, compiler error messages, and the Boost TypeIndex library.

  * The results of some tools may be neither helpful nor accurate, so an understanding of C++’s type deduction rules remains essential.

#### 2. auto

##### Item 5:  Prefer auto to explicit type declarations.

  * auto variables must be initialized, are generally immune to type mismatches that can lead to portability or efficiency problems, can ease the process of refactoring, and typically require less typing than variables with explicitly specified types.

  * auto-typed variables are subject to the pitfalls described in ### Items 2 and 6.

##### Item 6:  Use the explicitly typed initializer idiom when auto deduces undesired types.

  * “Invisible” proxy types can cause auto to deduce the “wrong” type for an initializing expression.

  * The explicitly typed initializer idiom forces auto to deduce the type you want it to have.

#### 3. Moving to Modern C++

##### Item 7:  Distinguish between () and {} when creating objects.

  * Braced initialization is the most widely usable initialization syntax, it prevents narrowing conversions, and it’s immune to C++’s most vexing parse.

  * During constructor overload resolution, braced initializers are matched to std::initializer_list parameters if at all possible, even if other constructors offer seemingly better matches.

  * An example of where the choice between parentheses and braces can make a significant difference is creating a std::vector\<numeric type\> with two arguments.

  * Choosing between parentheses and braces for object creation inside templates can be challenging.

##### Item 8: Prefer nullptr to 0 and NULL.

  * Prefer nullptr to 0 and NULL.

  * Avoid overloading on integral and pointer types.

##### Item 9:  Prefer alias declarations to typedefs.

  * typedefs don’t support templatization, but alias declarations do.
  
  * Alias templates avoid the “::type” suffix and, in templates, the “typename” prefix often required to refer to typedefs.
  
  * C++14 offers alias templates for all the C++11 type traits transformations
  
##### Item 10:  Prefer scoped enums to unscoped enums.

  * C++98-style enums are now known as unscoped enums.

  * Enumerators of scoped enums are visible only within the enum. They convert to other types only with a cast.

  * Both scoped and unscoped enums support specification of the underlying type. The default underlying type for scoped enums is int. Unscoped enums have no default underlying type.

  * Scoped enums may always be forward-declared. Unscoped enums may be forward-declared only if their declaration specifies an underlying type.

##### Item 11:  Prefer deleted functions to private undefined ones.

  *  Prefer deleted functions to private undefined ones.
  
  *  Any function may be deleted, including non-member functions and template instantiations.

##### Item 12:  Declare overriding functions override.

  *  Declare overriding functions override.

  *  Member function reference qualifiers make it possible to treat lvalue and rvalue objects (*this) differently.
  
##### Item 13:  Prefer const_iterators to iterators.

  *  Prefer const_iterators to iterators.

  *  In maximally generic code, prefer non-member versions of begin, end, rbegin, etc., over their member function counterparts.
  
##### Item 14:  Declare functions noexcept if they won’t emit exceptions.

  *  noexcept is part of a function’s interface, and that means that callers may depend on it.

  *  noexcept functions are more optimizable than non-noexcept functions.

  *  noexcept is particularly valuable for the move operations, swap, memory deallocation functions, and destructors.

  *  Most functions are exception-neutral rather than noexcept.

##### Item 15:  Use constexpr whenever possible.

  *  constexpr objects are const and are initialized with values known during
compilation.

  *  constexpr functions can produce compile-time results when called with arguments whose values are known during compilation.

  *  constexpr objects and functions may be used in a wider range of contexts than non-constexpr objects and functions.

  *  constexpr is part of an object’s or function’s interface.

##### Item 16:  Make const member functions thread safe.

  *  Make const member functions thread safe unless you’re certain they’ll never be used in a concurrent context.

  *  Use of std::atomic variables may offer better performance than a mutex, but they’re suited for manipulation of only a single variable or memory location.

##### Item 17:  Understand special member function generation.

  *  The special member functions are those compilers may generate on their own: default constructor, destructor, copy operations, and move operations.

  *  Move operations are generated only for classes lacking explicitly declared move operations, copy operations, and a destructor.

  *  The copy constructor is generated only for classes lacking an explicitly declared copy constructor, and it’s deleted if a move operation is declared. The copy assignment operator is generated only for classes lacking an explicitly declared copy assignment operator, and it’s deleted if a move operation is declared. Generation of the copy operations in classes with an explicitly declared destructor is deprecated.

  *  Member function templates never suppress generation of special member functions.
  
#### 4. Smart Pointers

##### Item 18:  Use std::unique_ptr for exclusive-ownership resource management.
- `std::unique_ptr` is a small, fast, move-only smart pointer for managing
  resources with exclusive-ownership semantics.
- By default, resource destruction takes place via delete, but custom deleters
  can be specified.  Stateful deleters and function pointers as deleters
  increase the size of `std::unique_ptr` objects.
- Converting a `std::unique_ptr` to a `std::shared_ptr` is easy.
- `unique_ptr` is a move-only type
- also applied to the Pimpl Idiom [Item 22](#item-22-when-using-the-pimpl-idiom-define-special-member-functions-in-the-implementation-file)
- And also `std::unique_ptr<T[]>`
  * About the only situation I can conceive of when a would make sense would be when you’re using a C-like API that returns a raw pointer to a heap array that you assume ownership of -> `std::unique_ptr<T[]>`
- `std::shared_ptr<Investment> sp = makeInvestment( arguments );`

```cpp
class Investment {
public:
  virtual ~Investment();
};
class Stock:
public Investment { ... };
class Bond:
public Investment { ... };
class RealEstate:
public Investment { ... };

template<typename... Ts> std::unique_ptr<Investment> makeInvestment(Ts&&... params);

{
	auto pInvestment = // pInvestment is of type 
		makeInvestment( arguments ); // std::unique_ptr<Investment>
}// destroy *pInvestment
```

```cpp
auto delInvmt = [](Investment* pInvestment)
                {
                  makeLogEntry(pInvestment);
                  delete pInvestment;
                };

template<typename... Ts>
std::unique_ptr<Investment, decltype(delInvmt)> // If it is C++14, the return value can be auto, and the definition of delInvmt can also be placed in the makeInvestment function.
makeInvestment(Ts&&... params) {
	std::unique_ptr<Investment, decltype(delInvmt)> pInv(nullptr, delInvmt);
  if ( /* a Stock object should be created */ ){
		pInv.reset(new Stock(std::forward<Ts>(params)...)); 
  }
  else if ( /* a Bond object should be created */ ){
		pInv.reset(new Bond(std::forward<Ts>(params)...)); 
  }
  else if ( /* a RealEstate object should be created */ ){
		pInv.reset(new RealEstate(std::forward<Ts>(params)...)); 
  }
  return pInv;
}
```

Code Details:
- `std::forward`: In order to solve the perfect-forward problem of parameters in a function template that uses rvalue reference parameters. [Item 25](#item-25-use-stdmove-on-rvalue-references-stdforward-on-universal-references), [reference](https://blog.csdn.net/zhangsj1007/article/details/81149719?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-6.edu_weight&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-6.edu_weight).
- `unique_ptr` can return a value as a function
- It is not possible to assign a bare pointer to a `unique_ptr` directly, which is standard usage `reset(new)`
- After the introduction of deleter, the size of the `unique_ptr` changes:
  1 word -> 2 word in the case of function pointers, and in the case of function objects, it depends on the state inside the function

##### Item 19:  Use std::shared_ptr for shared-ownership resource management.

dynamically allocated control blocks, arbitrarily large deleters and allocators, virtual function machinery, and atomic reference count manipulations

[The use of shared_ptr](https://blog.csdn.net/qq_33266987/article/details/78784852), [a shared_ptr usage technique that I don't understand.](https://gist.github.com/BruceChen7/8cccb33ea6fbc73a0651c4bce3166806)

As with garbage collection, clients need not concern themselves with managing the life‐ time of pointed-to objects, but as with destructors, the timing of the objects’ destruction is deterministic.

The impact of reference count:

  - `std::shared_ptr`'s are twice the size of a raw pointer
  - Memory for the reference count must be dynamically allocated unless `std::make_shared` is used
  - Increments and decrements of the reference count must be atomic

=> move assignment is faster than copy assignment

![`std::shared_ptr<T>`](./assets/shared-ptr.png)

For custom deleters, the difference with `unique_ptr` is that deleters do not affect the type of `shared_ptr`

  - This makes it easier for functions to pass parameters and put them in the same container
  - Always two words size:

```cpp
```

About the rules of control block

  - std::make_shared (see Item 21) always creates a control block
  - A control block is created when a std::shared_ptr is constructed from a unique-ownership pointer (i.e., a std::unique_ptr or std::auto_ptr).
  - When a std::shared_ptr constructor is called with a raw pointer, it creates a control block

=>

  - Creating two shared_ptr with the same bare pointer is an undefined behavior
    * Correct Spelling:

```cpp
```

Similarly, don't create a shared_ptr with this pointer

  - Correct writing: The Curiously Recurring Template Pattern (CRTP)
  - Note: `shared_from_this()` must be called after the object spawns `shared_ptr`
    * In order to prevent the process of an object that does not have a `shared_ptr`, ctors is often set to private
    * `shared_from_this()` cannot be called in the constructor, and it has not been handed over to shared_ptr at the time of construction

```cpp
class Widget: public std::enable_shared_from_this<Widget> {
public:
  // factory function that perfect-forwards args to a private ctor
	template<typename... Ts>
	static std::shared_ptr<Widget> create(Ts&&... params);
	void process(){
    processedWidgets.emplace_back(shared_from_this());
  }
private:
  Widget Widget();
  Widget(Widget &&other);
  Widget(const Widget &other);
  TCPConnection() = delete;
};
```

Warn:

  - `std::vector<std::shared_ptr<A>> a_vec(n, std::make_shared<A>());`.
  - This usage is wrong, and it will assign the same smart pointer to the elements inside, and the correct way to write it is as follows:

```cpp
std::vector<std::shared_ptr<A>> a(size);
std::for_each(std::begin(a), std::end(a),[](std::shared_ptr<A> &ptr) {
                    ptr = std::make_shared<A>();
```

  - `shared_ptr` there is no version of the array. It is always recommended to use `std::vector`
  - `shared_ptr` can't loop pointing, it will never deconstruct memory leaks

##### Item 20:  Use std::weak_ptr for std::shared_ptr-like pointers that can dangle.

`weak_ptr` indicates whether the shared_ptr is dangle, but it cannot be directly dereferenced, and an atomic operation (lock) is required to connect the judgment and the value

  - Potential use cases of `std::weak_ptr` for include caching, observer lists, and the prevention of `std::shared_ptr` cycles.

```cpp
auto spw = std::make_shared<Widget>();
std::weak_ptr<Widget> wpw(spw);
spw = nullptr;
if (wpw.expired()) ...
auto spw2 = wpw.lock();
std::shared_ptr<Widget> spw3(wpw); // if wpw's expired, throw std::bad_weak_ptr
```

Application: read/write cache to automatically delete objects that are no longer in use

```cpp
std::unique_ptr<const Widget> loadWidget(WidgetID id);
```

=>

```cpp
std::shared_ptr<const Widget> fastLoadWidget(WidgetID id) {
	static std::unordered_map<WidgetID, std::weak_ptr<const Widget>> cache;
	auto objPtr = cache[id].lock();
  if (!objPtr) {
    objPtr = loadWidget(id);
    cache[id] = objPtr;
	}
  return objPtr;
}

//Optimize space: delete unused weak_ptr in cache
```

##### Item 21:  Prefer std::make_unique and std::make_shared to direct use of new.

[`make_unique`](https://en.cppreference.com/w/cpp/memory/unique_ptr/make_unique)

C++14 does not have `make_unique`

  - Parameters can only be unbounded arrays: `std::unique_ptr<Vec3[]> v3 = std::make_unique<Vec3[]>(5);`

```cpp
// C++14 make_unique
namespace detail {
template<class>
constexpr bool is_unbounded_array_v = false;
template<class T>
constexpr bool is_unbounded_array_v<T[]> = true;
 
template<class>
constexpr bool is_bounded_array_v = false;
template<class T, std::size_t N>
constexpr bool is_bounded_array_v<T[N]> = true;
} // namespace detail
 
template<class T, class... Args>
std::enable_if_t<!std::is_array<T>::value, std::unique_ptr<T>>
make_unique(Args&&... args)
{
    return std::unique_ptr<T>(new T(std::forward<Args>(args)...));
}
 
template<class T>
std::enable_if_t<detail::is_unbounded_array_v<T>, std::unique_ptr<T>>
make_unique(std::size_t n)
{
    return std::unique_ptr<T>(new std::remove_extent_t<T>[n]());
}
 
template<class T, class... Args>
std::enable_if_t<detail::is_bounded_array_v<T>> make_unique(Args&&...) = delete;
```

```cpp
std::allocate_shared
auto spw1(std::make_shared<Widget>()); //auto can be used
```

__`make_shared` advantages__

  - If not, there is a potential risk of memory leakage, which is related to abnormal security
    * If computePriority throws an exception in the middle of the new shared_ptr, the memory is leaked
```cpp
processWidget(std::shared_ptr<Widget>(new Widget), computePriority());
```
  - `make_shared` More efficient, allocating memory for objects and control blocks at once

__`make_shared` disadvantages__

  - deleter
  - The perfect forwarding code of make_shared is used instead; you can only use new, unless you refer to [Item 2](#item-2-understand-auto-type-deduction)
```cpp
// create std::initializer_list
auto initList = { 10, 20 };
// create std::vector using std::initializer_list ctor
auto spv = std::make_shared<std::vector<int>>(initList);
```
  - using make functions to create objects of types with class-specific versions of operator new and operator delete is typically a poor idea. Because you can only new/delete the memory length of the object instead of adding a control block.
  - In the `shared_ptr` scenario, all related `weak_ptr` must be destroyed before the memory of the pointer control block is released

For the above reasons, I want to use new

```cpp
std::shared_ptr<Widget> spw(new Widget, cusDel);
processWidget(std::move(spw), computePriority()); // both efficient and exception safe
```

##### Item 22:  When using the Pimpl Idiom, define special member functions in the implementation file.

Design pattern: Reduce the compilation of the client (only include .h files).

`widget.h`

```cpp
class Widget {
public:
	Widget(); 
	~Widget(); 
	...
private:
  struct Impl;
  Impl *pImpl;
};
```

`widget.cpp`

```cpp
#include "widget.h" 
#include "gadget.h" 
#include <string> 
#include <vector>
struct Widget::Impl {
  std::string name;
  std::vector<double> data;
  Gadget g1, g2, g3;
};
Widget::Widget() : pImpl(new Impl) {}
Widget::~Widget() { delete pImpl; }
```

__New version with `unique_ptr`__

  - Don't generate destructors in .h files

`widget.h`

```cpp
class Widget {
public:
	Widget(); 
  ~Widget();
  Widget(Widget&& rhs);
  Widget& operator=(Widget&& rhs);
private:
  struct Impl;
  std::unique_ptr<Impl> pImpl;
};
```

`widget.cpp`

```cpp
#include "widget.h" 
#include "gadget.h" 
#include <string> 
#include <vector>
struct Widget::Impl {
  std::string name;
  std::vector<double> data;
  Gadget g1, g2, g3;
};
Widget::Widget(): pImpl(std::make_unique<Impl>()) {}
Widget::~Widget() = default;
Widget::Widget(Widget&& rhs) = default;
Widget& Widget::operator=(Widget&& rhs) = default;
Widget::Widget(const Widget& rhs)
: pImpl(std::make_unique<Impl>(*rhs.pImpl)) {}
Widget& Widget::operator=(const Widget& rhs)
{
	*pImpl = *rhs.pImpl;
  return *this;
}
```

If it's `shared_ptr`, you don't need to do anything, essentially because the `unique_ptr` deleter implicitly generates some functions in the type definition for more efficient runtime behavior

#### 5. Rvalue References, Move Semantics, and Perfect Forwarding

- Rvalue references => Move Semantics and Perfect Forwarding

- It’s especially important to bear in mind that a parameter is always an lvalue, even if its type is an rvalue reference

##### Item 23:  Understand std::move and std::forward.

- `std::move` doesn’t move anything.
- `std::forward` doesn’t forward anything.
- `std::move` unconditionally casts its argument to an rvalue, while,
- `std::forward` performs this cast only if a particular condition is fulfilled.

```cpp
template<typename T>
decltype(auto) move(T&& param) {
  using ReturnType = remove_reference_t<T>&&;
  return static_cast<ReturnType>(param);
} // C++14
// remove_reference is because Item 1 => T may be inferred as an lvalue reference
```

First, don’t declare objects const if you want to be able to move from them. Move requests on const objects are silently transformed into copy operations.

Second, `std::move` not only doesn’t actually move anything, it doesn’t even guarantee that the object it’s casting will be eligible to be moved. The only thing you know for sure about the result of applying `std::move` to an object is that it’s an rvalue.

```cpp
void process(const Widget& lvalArg);
void process(Widget&& rvalArg);
template<typename T>
void logAndProcess(T&& param) {
	auto now = std::chrono::system_clock::now();
  makeLogEntry("Calling 'process'", now);
	process(std::forward<T>(param));
}

Widget w;
logAndProcess(w);                  // call with lvalue
logAndProcess(std::move(w));       // call with rvalue
```

`std::forward` is a __conditional__ cast, it casts to an rvalue only if its argument was initialized with an rvalue. For principles, please refer to [Item 28](#item-28-understand-reference-collapsing).

##### Item 24:  Distinguish universal references from rvalue references.

`T&&` is not necessarily rvalue references, call them universal references. Initialization with an rvalue is an rvalue reference, and initialization with an lvalue is an lvalue reference.

The scenario is as follows:

  - Template:
```cpp
template<typename T>
void f(T&& param); // param is a universal reference
```
  - auto: `auto&& var2 = var1; // var2 is a universal reference`

Universal reference scenarios have limitations:

  - It must be `T&&`, and it will not work with `const`
  - There must be type deduction, e.g. 's caller explicitly specifies the type, type deduction, and `push_back`, `emplace_back`

```cpp
template<class T, class Allocator = allocator<T>>  // from C++
class vector {                                     // Standards
public:
	void push_back(T&& x);
	...
};
template<class T, class Allocator = allocator<T>>  
class vector {
public:
	template <class... Args>
	void emplace_back(Args&&... args); ...
};
```

Application of universal reference:

```cpp
auto timeFuncInvocation = [](auto&& func, auto&&... params){
  start timer;
  std::forward<decltype(func)>(func)( std::forward<decltype(params)>(params)... );
  stop timer and record elapsed time;
};
```

##### Item 25:  Use std::move on rvalue references, std::forward on universal references.

The motivation for `std::forward` is conditionally cast

Perfect forwarding is often used with [variadic templates](http://en.cppreference.com/w/cpp/language/parameter_pack) to wrap calls to functions with an arbitrary number of arguments. For example, [`std::make_unique`](http://en.cppreference.com/w/cpp/memory/unique_ptr/make_unique) and [`std::make_shared`](http://en.cppreference.com/w/cpp/memory/shared_ptr/make_shared) both use perfect forwarding to forward their arguments to the constructor of the wrapped type.

One of the motivations for Universal reference is to replace "simultaneous overload lvalue, rvalue references", the disadvantages of which are: 1) potential overhead for certain scenarios, 2) code volume, and 3) scalability, the extension of multiparameter functions

```cpp
Matrix // by-value return 
operator+(Matrix&& lhs, const Matrix& rhs) {
	lhs += rhs;
  return std::move(lhs);
}

template<typename T>
Fraction reduceAndCopy(T&& frac) {
	frac.reduce();
	return std::forward<T>(frac);
}
```

Never apply `std::move` or `std::forward` to local objects if they would otherwise be eligible for the return value optimization.

  - copy elision
  - Requirements for RVO to be in force
    * The type is consistent
    * the local object is what’s being returned, such as it cannot be a referenced type or function parameter
      * unnamed (named->NRVO)
  - Reason why move is never necessary: __​​"if the conditions for the RVO are met, but compilers choose not to perform copy elision, the object being returned must be treated as an rvalue."__

##### Item 26:  Avoid overloading on universal references.

- Overloading on universal references almost always leads to the universal reference overload being called more frequently than expected.
- Perfect-forwarding constructors are especially problematic, because they’re typically better matches than copy constructors for non-const lvalues, and they can hijack derived class calls to base class copy and move constructors.
  * Even if compilers generate the relevant constructor for item 17, there are still cases where the priority is lower than overloaded universal references

##### Item 27:  Familiarize yourself with alternatives to overloading on universal references.

- Abandon overloading
- Pass by const `T&`
- Pass by value

```cpp
class Person {
 public:
	explicit Person(std::string n) : name(std::move(n)) {}
  explicit Person(int idx) : name(nameFromIdx(idx)) {}
  ...
private:
  std::string name;
};
```

- Use Tag dispatch

```cpp
std::multiset<std::string> names;      // global data structure
template<typename T>                   // make log entry and add
void logAndAdd(T&& name)               // name to data structure
{
	auto now = std::chrono::system_clock::now();
  log(now, "logAndAdd");
  names.emplace(std::forward<T>(name));
}

=====>
  
template<typename T>
void logAndAdd(T&& name)
{
	logAndAddImpl(
		std::forward<T>(name),
		std::is_integral<typename std::remove_reference<T>::type>()
	); 
}

template<typename T>
void logAndAddImpl(T&& name, std::false_type) {
	auto now = std::chrono::system_clock::now();
  log(now, "logAndAdd");
  names.emplace(std::forward<T>(name));
}
// std::false_type(compile value) 而非 false(runtime value)

void logAndAddImpl(int idx, std::true_type) {
  logAndAdd(nameFromIdx(idx));
}
```

- Constraining templates that take universal references

```cpp
class Person {
 public:
	template<typename T,
					 typename = typename std::enable_if<condition>::type>
	explicit Person(T&& n);
  
=>

class Person {
 public:
	template<typename T,
					 typename = typename std::enable_if<
												!std::is_same<Person,
																			typename std::decay<T>::type
																		 >::value
               				>::type
	>
  explicit Person(T&& n);
	...
};
```

=>

`is_same` -> `is_base_of` => Further solve the problem of derived classes in [Item 26](#item-26-avoid-overloading-on-universal-references)
  
=>
  
c++14: typename -> `_t` suffix
  
=>

```cpp  
class Person {
 public:
	template<
		typename T,
		typename = std::enable_if_t<
			!std::is_base_of<Person, std::decay_t<T>>::value
			&&
			!std::is_integral<std::remove_reference_t<T>>::value
		>
	>
explicit Person(T&& n)
: name(std::forward<T>(n)) 
{
  // assert that a std::string can be created from a T object
	static_assert(
		std::is_constructible<std::string, T>::value, 
    "Parameter n can't be used to construct a std::string"
	);
  ...
}
explicit Person(int idx) : name(nameFromIdx(idx)) 
{... }
...
 private:
  std::string name;
};
```

- Disadvantages：perfect forwarding has failure cases ([Item 30](#item-30-familiarize-yourself-with-perfect-forwarding-failure-cases)) and baffling error messages

##### Item 28:  Understand reference collapsing.

> If either reference is an lvalue reference, the result is an lvalue reference. Otherwise (i.e., if both are rvalue references) the result is an `rvalue` reference.
>

Four contexts

  - template instantiation
  - auto type generation
  - the generation and use of typedefs and alias declarations ([Item 9](#item-9-prefer-alias-declarations-to-typedefs))
  - `decltype` ([Item 3](#item-3-understand-decltype))

=> the implementation of `std::forward`

```cpp
template<typename T>
T&& forward(typename
							remove_reference<T>::type& param)
{
	return static_cast<T&&>(param);
}
```

=>Review auto&&

=>

```cpp
template<typename T>
class Widget {
 public:
  typedef T&& RvalueRefToT;
  ...
};
```

##### Item 29:  Assume that move operations are not present, not cheap, and not used.

not cheap

  - move `std::array` runs in linear time
  - `std::string` with SSO optimization, small strings are stored in the buffer inside the object, and moves are not faster

not usable

  - The context in which the moving would take place requires a move operation that emits no exceptions, but that operation isn’t declared `noexcept`

##### Item 30:  Familiarize yourself with perfect forwarding failure cases.

The meaning of perfect forwarding => __passing type information, only for references__

```cpp
template<typename... Ts>
void fwd(Ts&&... params) {
  f(std::forward<Ts>(params)...)
}
```

Application of [Item 42](#item-42-consider-emplacement-instead-of-insertion) (`std::make_unique`), and, [Item 21](#item-21-prefer-stdmake_unique-and-stdmake_shared-to-direct-use-of-new) (`emplace`)

The intrinsic reason for failure cases is that f and fwd don't do things the same

  - Braced initializers: f has the ability to do the conversion, while fwd fails type inference
  - 0 or NULL as null pointers
  - Declaration-only integral __static const__ data members
    * At the hardware level, pointers and references have similar meanings

```cpp
class Widget {
 public:
	static const std::size_t MinVals = 28; // MinVals' declaration
	...
};


std::vector<int> widgetData; widgetData.reserve(Widget::MinVals); // use of MinVals

f(Widget::MinVals); // fine, treated as "f(28)"
fwd(Widget::MinVals); // error! shouldn't link

const std::size_t Widget::MinVals; // in Widget's .cpp file, remember to specify it only once
```

  - Overloaded function names and template names
    * Essentially, FWD doesn't have the ability to infer function information

```cpp
using ProcessFuncType = int (*)(int);
ProcessFuncType processValPtr = processVal;
fwd(processValPtr);
fwd(static_cast<ProcessFuncType>(workOnVal));
```

  - Bitfields
    * Pointers to bitfields don't exist.

```cpp
struct IPv4Header {
  std::uint32_t version:4,
                IHL:4,
                DSCP:6,
                ECN:2,
                totalLength:16;
  ...
};
void f(std::size_t sz); // function to call
IPv4Header h;
f(h.totalLength); // fine
fwd(h.totalLength); // error

// copy bitfield value; see Item 6 for info on init. form 
auto length = static_cast<std::uint16_t>(h.totalLength);
fwd(length); // forward the copy
```

#### 6. Lambda Expressions

Scenario:

  - STL algorithms, custom deleters, condition variables in threading API ([Item 39](#item-39-consider-void-futures-for-one-shot-event-communication))
  - callback functions, interface adaptation functions, context-specific functions for one-off calls

Conception:

  - Compilation: lambda expressions, closure class
      * A __closure class__ is a class from which a closure is instantiated. Each lambda causes compilers to generate a unique closure class. The statements inside a lambda become executable instructions in the member functions of its closure class.
  - Runtime: closure
      * A __closure__ is the runtime object created by a lambda. Depending on the capture mode, closures hold copies of or references to the captured data.

Note
  - The `mutable` specification enables the body of a lambda expression to modify variables that are captured by value.
    * [ref](https://learn.microsoft.com/en-us/cpp/cpp/lambda-expressions-in-cpp?view=msvc-170)


##### Item 31:  Avoid default capture modes.

There are two default capture modes in C++11: by-reference and by-value. Default by-reference capture can lead to dangling references. Default by-value capture lures you into thinking you’re immune to that problem (you’re not), and it lulls you into thinking your closures are self-contained (they may not be).

```cpp
using FilterContainer =
  std::vector<std::function<bool(int)>>;
FilterContainer filters;
void addDivisorFilter(){
  auto calc1 = computeSomeValue1();
  auto calc2 = computeSomeValue2();
  auto divisor = computeDivisor(calc1, calc2);
  filters.emplace_back(
  	[&](int value) { return value % divisor == 0; }
  ); 
}

template<typename C>
void workWithContainer(const C& container)
{
  auto calc1 = computeSomeValue1();
  auto calc2 = computeSomeValue2();
  auto divisor = computeDivisor(calc1, calc2);
  using ContElemT = typename C::value_type;
  using std::begin;
  using std::end;
  if (std::all_of(
  			begin(container), end(container),
    		[&](const ContElemT& value)
  			{ return value % divisor == 0; })
  	) {
  	...
  } else {
    ...
  }
}

// C++14
if (std::all_of(begin(container), end(container),
								[&](const auto& value)
                { return value % divisor == 0; }))
```

The size of objects generated by auto is smaller, less than fixed size in closure `std::function`

Captures apply only to non-static local variables (including parameters) visible in the scope where the lambda is created.

  - default by-value capture essentially captures Widget's `this` pointer => unintentionally captures `this`

```cpp
class Widget {
 public:
	...
  void addFilter() const;

 private:
	int divisor;
};
void Widget::addFilter() const {
	filters.emplace_back(
		[=](int value) { return value % divisor == 0; }
	);
}
```

===>
  
```cpp
void Widget::addFilter() const {
	filters.emplace_back( // C++14:
		[divisor = divisor](int value) // copy divisor to closure 
    { return value % divisor == 0; } // use the copy
	);
}
```

An additional drawback to default by-value captures is that they can suggest that the corresponding closures are self-contained and insulated from changes to data outside the closures. In general, that’s not true, because lambdas may be dependent not just on local variables and parameters (which may be captured), but also on objects with __static storage duration__.

```cpp
void addDivisorFilter() {
  static auto calc1 = computeSomeValue1();
  static auto calc2 = computeSomeValue2();
	static auto divisor = computeDivisor(calc1, calc2);
	filters.emplace_back(
		[=](int value)
		{ return value % divisor == 0; }
	);
  ++divisor;
}
//Although lambda expression is written by-value, it actually captures reference.
```

##### Item 32:  Use init capture to move objects into closures.

generalized lambda capture, which can capture the result of an expression

e.g. for move-only object like or std::unique_ptrstd::future

Using an init capture makes it possible for you to specify

  - __the name of a data member__ in the closure class generated from the lambda and
  - __an expression__ initializing that data member.

```cpp
auto pw = std::make_unique<Widget>();
...
auto func = [pw = std::move(pw)]
						{ return pw->isValidated()
										 && pw->isArchived(); };
```

If you implement it in C++11:

  - moving the object to be captured into a function object produced by an `std::bind`
  - giving the lambda a reference to the “captured” object.
    * `std::bind` -> a bind object
    * the lifetime of the bind object is the same as that of the closure

```cpp
// C++14
std::vector<double> data;
...
auto func = [data = std::move(data)] { /* uses of data */ };

// C++11
std::vector<double> data;
...
auto func =
  std::bind(
		[](const std::vector<double>& data)
	  { /* uses of data */ }, 
  std::move(data)
);

auto func =
  std::bind(
		[](std::vector<double>& data) mutable
	  { /* uses of data */ }, 
  std::move(data)
);
```

##### Item 33:  Use decltype on auto&& parameters to std::forward them.

- generic lambdas
  * Definition: lambdas that use auto in their parameter specifications
  * Implementation: operator() in the lambda’s closure class is a template.

```cpp
auto f = [](auto x){ return func(normalize(x)); };
class SomeCompilerGeneratedClassName {
 public:
	template<typename T>
	auto operator()(T x) const
	{ return func(normalize(x)); }
	...
}

//Use reference collapse --->
auto f = [](auto&& x){ return func(normalize(std::forward<decltype(param)>(x))); };

auto f =
  [](auto&&... param){ 
  	return func(normalize(std::forward<decltype(param)...>(x)));
	};
```

##### Item 34:  Prefer lambdas to std::bind.

  - Lambdas are more readable, more expressive, and may be more efficient than using `std::bind`.

  - In C++11 only, `std::bind` may be useful for implementing move capture or for binding objects with templatized function call operators.

lambdas are more readable

lambdas are faster (in some cases, function pointer called through is less likely to be inlined) than `std::bind`

```cpp
// typedef for a point in time (see Item 9 for syntax)
using Time = std::chrono::steady_clock::time_point;
// see Item 10 for "enum class"
enum class Sound { Beep, Siren, Whistle };
// typedef for a length of time
using Duration = std::chrono::steady_clock::duration;

// at time t, make sound s for duration d
void setAlarm(Time t, Sound s, Duration d);

auto setSoundL =
[](Sound s) {
	// make std::chrono components available w/o qualification
	using namespace std::chrono;
  setAlarm(steady_clock::now() + hours(1),
           s,
           seconds(30));
};

// Wrong writing: steady_clock::now() is not called when setAlarm is called (but in std::bind)

using namespace std::chrono;
using namespace std::literals;
using namespace std::placeholders;
auto setSoundB =
  std::bind(setAlarm,
						steady_clock::now() + 1h, // incorrect!
            _1,
						30s);

--->

auto setSoundB =
	std::bind(setAlarm,
						std::bind(std::plus<>(), steady_clock::now(), 1h),
            _1,
						30s);
// C++11: std::plus<steady_clock::time_point>()

// --->

// If overload setAlarm
void setAlarm(Time t, Sound s, Duration d, Volume v);

using SetAlarm3ParamType = void(*)(Time t, Sound s, Duration d);
auto setSoundB =
	std::bind(static_cast<SetAlarm3ParamType>(setAlarm),
						std::bind(std::plus<>(),
                      steady_clock::now(),
											1h),
            _1,
						30s);
```

```cpp
// C++14
auto betweenL =
     [lowVal, highVal]
     (const auto& val)                          
     { return lowVal <= val && val <= highVal; };

using namespace std::placeholders;
auto betweenB =
	std::bind(std::logical_and<>(), // C++14
						std::bind(std::less_equal<>(), lowVal, _1),
            std::bind(std::less_equal<>(), _1, highVal));

// C++11
auto betweenL =
     [lowVal, highVal]
     (int val)                          
     { return lowVal <= val && val <= highVal; };

using namespace std::placeholders;
auto betweenB =
	std::bind(std::logical_and<bool>(), // C++14
						std::bind(std::less_equal<int>(), lowVal, _1),
            std::bind(std::less_equal<int>(), _1, highVal));
```

  - `std::bind`: implicitly stored by value
    * `std::bind` stores values, and all arguments passed to bind objects are passed by reference
    * can store refs: `auto compressRateB = std::bind(compress, std::ref(w), _1);`
  - Lambdas: explicitly
```cpp
enum class CompLevel { Low, Normal, High };
Widget compress(const Widget& w,
                CompLevel lev);
```

  - Scenarios where `std::bind` has advantages (all in C++11)
    * Move capture ([Item 32](#item-32-use-init-capture-to-move-objects-into-closures))
    * Polymorphic function objects

```cpp
class PolyWidget {
public:
 template<typename T>
	void operator()(const T& param);
  ...
};

PolyWidget pw;
auto boundPW = std::bind(pw, _1);
boundPW(1930);
boundPW(nullptr);
boundPW("Rosebud");

// C++14 lambda
auto boundPW = [pw](const auto& param) // C++14
							 { pw(param); };
```

#### 7. The Concurrency API

futures: or `std::future` and `std::shared_future`

##### Item 35:  Prefer task-based programming to thread-based.

```cpp
// thread-based
int doAsyncWork();
std::thread t(doAsyncWork);
// task-based
auto fut = std::async(doAsyncWork);
```

  - Advantages: Return value, exception tolerance, departure from the concept of thread
  - thread
    * __Hardware threads__ are the threads that actually perform computation. Contemporary machine architectures offer one or more hardware threads per CPU core.
    * __Software threads__ (also known as OS threads or system threads) are the threads that the operating system manages across all processes and schedules for execution on hardware threads. It’s typically possible to create more software threads than hardware threads, because when a software thread is blocked (e.g., on I/O or waiting for a mutex or condition variable), throughput can be improved by executing other, unblocked, threads.
    * limited resource: oversubscription -> (even if the function is `noexcept` attribute) results in `std::system_error`
    * oversubscription: too many threads -> results in costly context switching, and cache inconsistency
    * `std::thread`'s are objects in a C++ process that act as handles to underlying software threads. Some std::thread objects represent “null” handles, i.e., correspond to no software thread, because they’re in a default-constructed state (hence have no function to execute), have been moved from (the moved-to then acts as the handle to the underlying software thread), have been joined (the function they were to run has finished), or have been detached (the connection between them and their underlying software thread has been severed).
  - Task model breaks away from the concept of thread -> No need to do thread management yourself, leave it to the runtime scheduler
    * With global information, arrange __"run it on the thread needing the result"__
    * improve load balancing across hardware cores through work-stealing algorithms
  - Some situations where using threads directly may be appropriate
    * You need access to the API of the underlying threading implementation.
      - __native_handle__
    * You need to and are able to optimize thread usage for your application.
    * You need to implement threading technology beyond the C++ concurrency API

##### Item 36:  Specify std::launch::async if asynchronicity is essential.

  - `std::launch::async`: on a different thread
    * GUI thread
  - `std::launch::deferred`: deferred until get or wait is invoked
  - `default = std::launch::async | std::launch::deferred`
    * It is not possible to confirm whether the threads are parallel or unified; it may not be possible to predict whether to execute or not
    * [Async Tasks in C++11: Not Quite There Yet](https://bartoszmilewski.com/2011/10/10/async-tasks-in-c11-not-quite-there-yet/)
      - Interact with TLS
      - affects wait-based loops using timeout

```cpp
using namespace std::literals;
void f() {
	std::this_thread::sleep_for(1s);
}
auto fut = std::async(f);
while (fut.wait_for(100ms) != std::future_status::ready){
	...
  // loop until f has finished running...
  // which may never happen!
  // fut.wait_for will always return std::future_status::deferred
}
```

==>

```cpp
auto fut = std::async(f);
if (fut.wait_for(0s) == std::future_status::deferred) {
	// use wait or get on fut to call f synchronously
  ...
} else { // task isn't deferred
	while (fut.wait_for(100ms) != std::future_status::ready) {
    ...
  }
  ...
}
```

```cpp
//C++11
template<typename F, typename... Ts>
inline
std::future<typename std::result_of<F(Ts...)>::type>
reallyAsync(F&& f, Ts&&... params) {
  return std::async(std::launch::async,
										std::forward<F>(f),
                    std::forward<Ts>(params)...);
}

//C++14
template<typename F, typename... Ts>
inline auto reallyAsync(F&& f, Ts&&... params) {
  return std::async(std::launch::async,
										std::forward<F>(f),
                    std::forward<Ts>(params)...);
}
```

##### Item 37:  Make std::threads unjoinable on all paths.

  - Joinable `std::thread`
    * Blocked or waiting to be scheduled
    * have run to completion
  - Unjoinable `std::thread`
    * Default-constructed std::threads
    * `std::thread` objects that have been moved from.
    * std::threads that have been joined.
    * std::threads that have been detached.

```cpp
constexpr auto tenMillion = 10000000;  
// C++ 14: tenMillion = 10'000'000
bool doWork(std::function<bool(int)> filter,
	          int maxVal = tenMillion) {
	std::vector<int> goodVals;
	std::thread t([&filter, maxVal, &goodVals] {
									for (auto i = 0; i <= maxVal; ++i){
                    if (filter(i)) goodVals.push_back(i);
                  }
	  						});
  // use handle to set t's priority
  // Recommend: start t suspended
  auto nh = t.native_handle();
  ...
  if (conditionsAreSatisfied()) {
    t.join();
    performComputation(goodVals);
    return true;
	}
	return false;
}
```

Destruction of a joinable thread causes program termination: The following two designs are unreasonable

  - An implicit join:
    * Potential performance issues
    * [Item 39](#item-39-consider-void-futures-for-one-shot-event-communication): a hung program ---> interruptible threads ---> [Anthony Williams’ C++ Concurrency in Action (Manning Publications, 2012)](../cpp_concurrency_in_action/C++%20Concurrency%20in%20Action.pdf), [section 9.2](../cpp_concurrency_in_action/src/ch09/listing_9.2.cpp).
  - An implicit detach: worse design, local variables are destroyed

=> Design RAII object

  - Declare objects last in lists of data members.

```cpp
class ThreadRAII {
 public:
	enum class DtorAction { join, detach };
	ThreadRAII(std::thread&& t, DtorAction a)
	: action(a), t(std::move(t)) {}
	~ThreadRAII() {
		if (t.joinable()) {
			if (action == DtorAction::join) {
        t.join();
			} else {
        t.detach();
			}
		}
  }
  ThreadRAII(ThreadRAII&&) = default;
  ThreadRAII& operator=(ThreadRAII&&) = default;
  
  std::thread& get() { return t; }
 
 private:
  DtorAction action;
  std::thread t;
};
```

##### Item 38:  Be aware of varying thread handle destructor behavior.

Both objects and future objects can be thought of as handles to system threads `std::thread`
  - a future is one end of a communications channel through which a callee transmits a result to a caller
    * Where does the information exist? ---> callee's promise, caller's future won't work ---> shared state
  - Future destructors normally just destroy the future’s data members.
  - The final future referring to a shared state for a non-deferred task launched via blocks until the task completes -> `std::async`
    * deferred task <--- an implicit join
    * Another way to generate a shared state: `std::packaged_task`

```cpp
int calcValue();
std::packaged_task<int()> pt(calcValue);
auto fut = pt.get_future();

std::thread t(std::move(pt));

{
  std::packaged_task<int()> pt(calcValue);
	auto fut = pt.get_future();
	std::thread t(std::move(pt));
  ...
}
```

##### Item 39:  Consider void futures for one-shot event communication.

```cpp
std::condition_variable cv;
std::mutex m;

// detect event, tell reacting task
cv.notify_one();

/////////

... //prepare to react
{
  std::unique_lock<std::mutex> lk(m);
  cv.wait(lk); // wait for notify
  ... // react to event
}
...
```

Problems with Reacting code:

  - Potentially unnecessary mutex
  - If the detecting task notifies the condvar before the reacting task waits, the reacting task will hang.
  - The wait statement fails to account for spurious wakeups.

```cpp
---> cv.wait(lk, []{ return whether the event has occurred; });
```

<=>

```cpp
while (!pred()) {
    wait(lock);
}
```

Another option

  - The disadvantage is that polling in the reacting task <--- not truly blocked

```cpp
std::atomic<bool> flag(false);

flag = true;

...
while (!flag);
...
```

Combination schemes

```cpp
// detector
std::condition_variable cv;
std::mutex m;
bool flag(false);
...
{
	std::lock_guard<std::mutex> g(m);
	flag = true;
}
cv.notify_one();

// reactor
...
{
  std::unique_lock<std::mutex> lk(m);
  cv.wait(lk, [] { return flag; });
}
...
```

The combination scheme is correct, but not concise

=> having the reacting task wait on a future that’s set by the detecting task (void future)

```cpp
std::promise<void> p;

// detector
...
p.set_value();

// reactor
...
p.get_future().wait();
...
```

  - Advantages: no waste of resources, no spurious wakeups, no mutex

  - Disadvantages: incur heap-based allocation and deallocation, limited to one-shot mechanism

e.g.

```cpp
std::promise<void> p;
void react();

void detect()
{
  std::thread t([] {
									p.get_future().wait();
									react();
  							});
  ...
  p.set_value();
  ...
  t.join();
}
```

=>

```cpp
std::promise<void> p;
void react();

void detect()
{
  ThreadRAII tr(
    std::thread t([] {
                    p.get_future().wait();
                    react();
                  }),
    ThreadRAII::DtorAction::join    // risky!
  );
  
  ... // thread inside tr is suspended here.
      // if an exception emitted --> ThreadRAII never returns
  
  p.set_value(); // unsuspend thread inside tr
  ...
}
```

Expand multiple threads

```cpp
std::promise<void> p;
void react();

void detect()
{
  auto sf = p.get_future().share();
  std::vector<std::thread> vt;
  
  for (int i = 0; i < threadsToRun; i++) {
    vt.emplace_back([sf]{ sf.wait();
                        	react(); });
  }
  ...
  p.set_value();
  ...
    
  for (auto& t : vt) {
    t.join();
  }
}
```

[Folly::future](https://kitup.com/facebook/fake/blap/main/fake/docs/futures.mt)

```cpp
std::vector<folly::Promise<Input>> pros(inputs.size());
std::vector<folly::Future<Output>> futs;
for (auto& p : pros) {
  auto f = p.getFuture().thenValue([func1](Input input){
      return folly::makeFuture<Output>(func1(input));
    })
    .thenValue([func2](Output output)) {
        return folly::makeFuture<Output>(func2(output));
    }
    .thenValue([func2](Output output)) {
        return folly::makeFuture<Output>(func2(output));
    };
  futs.push_back(std::move(f));
}
auto allf = folly::collectAll(futs);
auto it = ...;
for (auto& p : pros) {
  p.setValue(*it);
  ++it;
}
assert(allf.isReady());
auto& results = allf.value();
```

##### Item 40:  Use std::atomic for concurrency, volatile for special memory.

`std::atomic` is for data accessed from multiple threads without using mutexes. It’s a tool for writing concurrent software.

  - what’s atomic is nothing more than the read of an `std::atomic`
  - read-modify-write (RMW) operations
  - Data race is an undefined behavior => variables may have any value
  - Can be used to satisfy critical ordering requirement (using sequential consistency)

```cpp
std::atomic<bool> valAvailable(false);
auto imptValue = computeImportantValue();
valAvailable = true;
```

  - the copy operations for are deleted std::atomic
    * The hardware does not support read x and write y in a single atomic operation
    * Move operations aren't explicitly declared
  - `load` and `store`

```cpp
std::atomic<int> y(x.load());

y.store(x.load());

x.fetch_add(1, std::memory_order_release);
```

  - `exchange`
    * The return value is the old value
  - `std::atomic_thread_fence(std::memory_order_release);`

```cpp
//Global
std::string computation(int);
void print( std::string );
 
std::atomic<int> arr[3] = { -1, -1, -1 };
std::string data[1000]; //non-atomic data
 
// Thread A, compute 3 values
void ThreadA( int v0, int v1, int v2 )
{
//assert( 0 <= v0, v1, v2 < 1000 );
data[v0] = computation(v0);
data[v1] = computation(v1);
data[v2] = computation(v2);
std::atomic_thread_fence(std::memory_order_release);
std::atomic_store_explicit(&arr[0], v0, std::memory_order_relaxed);
std::atomic_store_explicit(&arr[1], v1, std::memory_order_relaxed);
std::atomic_store_explicit(&arr[2], v2, std::memory_order_relaxed);
}
 
// Thread B, prints between 0 and 3 values already computed.
void ThreadB()
{
int v0 = std::atomic_load_explicit(&arr[0], std::memory_order_relaxed);
int v1 = std::atomic_load_explicit(&arr[1], std::memory_order_relaxed);
int v2 = std::atomic_load_explicit(&arr[2], std::memory_order_relaxed);
std::atomic_thread_fence(std::memory_order_acquire);
// v0, v1, v2 might turn out to be -1, some or all of them.
// otherwise it is safe to read the non-atomic data because of the fences:
if( v0 != -1 ) { print( data[v0] ); }
if( v1 != -1 ) { print( data[v1] ); }
if( v2 != -1 ) { print( data[v2] ); }
}
```

```cpp
std::atomic_thread_fence(std::memory_order_release);
version_.fetch_add(1);
```

`volatile` is for memory where reads and writes should not be optimized away. It’s a tool for working with special memory.

  - The `volatile` keyword essentially prevents the compiler from doing constant optimization
  - no guarantee of operation atomicity and insufficient restrictions on code reordering
  - In a nutshell, it’s for telling compilers that they’re dealing with memory that doesn’t behave normally
  - special memory
    * Memory-mapped I/O, interacting with peripherals
  - seemingly redundant loads and dead stores must be preserved when dealing with special memory

Two features are shared: `volatile` and `std::atomic<int>`

#### 8. Tweaks

##### Item 41:  Consider pass by value for copyable parameters that are cheap to move and always copied.

```cpp
class Widget {
 public:
	void addName(std::string newName) { 	
    names.push_back(std::move(newName));
  }
	...
};
```

Discussion of the meaning of copyable in the title:

```cpp
void setPtr(std::unique_ptr<std::string>&& ptr) {
  p = std::move(ptr);
}
```

The assignment scenario is different from the construction case:

  - applies to any parameter type that holds values in dynamically allocated memory

```cpp
class Password {
 public:
	void changeTo(const std::string& newPwd) {
    text = newPwd; // can reuse text's memory if text.capacity() >= new Pwd.size()
  }
}
```

that pass by value is susceptiable to the slicing problem

```cpp
class Widget { ... };
class SpecialWidget: public Widget { ... };
void processWidget(Widget w); // suffers from slicing problem
SpecialWidget sw;
processWidget(sw);
```

##### Item 42:  Consider emplacement instead of insertion.                       

Instead of:

`insert`, `push_front`, `push_back`, `std::forward_list::insert_after`

Prefer:

`place`, `emplace_front`, `emplace_back`, `std::forward_list::emplace_after`

  - Of all containers, `insert` only, is not supported `std::forward_list` and `std::array`
  - [`emplace_hint`](https://en.cppreference.com/w/cpp/container/map/emplace_hint)

`emplace_back` uses perfect forwarding (limitations -> [Item 30](#item-30-familiarize-yourself-with-perfect-forwarding-failure-cases))

a heuristic that can help you identify situations where emplacement functions are most likely to be worthwhile

  - The value being added is constructed into the container, not assigned.
    * Node-based containers virtually always use construction to add new values, and most standard containers are node-based. The only ones that aren’t are , , and . ( isn’t, either, but it doesn’t support insertion or emplacement, so it’s not relevant here.)`std::vector` `std::deque` `std::string` `std::array`
  - The argument type(s) being passed differ from the type held by the container.
  - The container is unlikely to reject the new value as a duplicate.

two other issues

  - `shared_ptr` + `push_back` Exceptional security
    * Fundamentally, the effectiveness of resource-managing classes like and is predicated on resources (such as raw pointers from new) being __immediately__ passed to constructors for resource-managing objects. The fact that functions like and automate this is one of the reasons they’re so important.`std::shared_ptr` `std::unique_ptr` `std::make_shared` `std::make_unique`

```cpp
std::list<std::shared_ptr<Widget>> ptrs;
void killWidget(Widget* pWidget);
ptrs.push_back(std::shared_ptr<Widget>(new Widget, killWidget));
ptrs.push_back({ new Widget, killWidget });

ptrs.emplace_back(new Widget, killWidget); // Exception security issues
```

=>

```cpp
std::shared_ptr<Widget> spw(new Widget, killWidget);
ptrs.push_back(std::move(spw));
```

  - interaction with constructors explicit
    * `emplace_back` is not considered an implicit conversion request
    * Thinking deeply, direct initialization is permitted to use explicit constructors

```cpp
std::vector<std::regex> regexes;
regexes.emplace_back(nullptr); // why is it valid?
regexes.push_back(nullptr); // compile error
--->
std::regex upperCaseWord("[A-Z]+"); // std::regex constructor takeing a const char* pointer is explicit

std::regex r1 = nullptr; // compile error
std::regex r2(nullptr); // compiles
````

<div align="right"><a href="#top" target="_blacnk"><img src="https://img.shields.io/badge/Back To Top-orange?style=for-the-badge&logo=expo&logoColor=white" /></a></div>

### Disclaimer

I do not own the copyright of the repository and the copyright belongs to Scott Meyers. The repository is only for personal use.

<div align="right"><a href="#top" target="_blacnk"><img src="https://img.shields.io/badge/Back To Top-orange?style=for-the-badge&logo=expo&logoColor=white" /></a></div>
