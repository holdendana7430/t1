代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cemhaywx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dawwqogg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3srpuvwem.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cuemompt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pgxxtvlv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3knsevsxf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xwqjjiix.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zwumfcvp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mxthlopm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3muvrjyzp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vczfxwwz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyrjlzxl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jffdnfbc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wdjdcnfb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3sjlampsw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ojukspkw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rlqrhmyq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bdsaucve.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ruggdxam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gojifofk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3azsubbzg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbpoory.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rsvipzvs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kfkwvpzh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnfwxor.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bertayli.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gwhymdym.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bqjvorai.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yanwrjkr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uupdvlap.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3upganibl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ztxusjfk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kdhsiinb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qztqwoeq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yuztsdct.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fbrrxurq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tlvjixjl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3abehpdmu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pgckyvxc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3blmgbrem.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fvqltgzc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qmkgkjgr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3iilhrwcz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrsighb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxsbcwmu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zelocwei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peciiczm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcfnhsil.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ycirwmrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xhqkkhfn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxowsyw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlhxnhwm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyleumub.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ibvyhgge.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nauopmcw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rzokznvh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3oioabbdp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3smzcakgh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zszkxino.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anguskwq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eaxggfmg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vbamgehr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnaezrmk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3klrsrgow.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3emfvrebp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rtcbgbkf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ksqwjeem.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhjmqqyw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhmwrbv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pkimyeel.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szxdmsxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ijlgupgn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hkrneyru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sciztevr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3veupqdjw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bxxyurzt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eoqmlzpu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3buepqwts.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hzgxfdjs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bhmptnxl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ddksnxht.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lyhfnlyt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mahsynoz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3owpfxvje.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3giuuqmab.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3frmsxzeb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qzasqeiu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3auykepvh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uzdodkng.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rnrfnkfq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ovujqsan.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yxpvvexx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3glomkwvz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pzbvlvvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fskkqbco.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xyoigqum.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aaamitrq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xgooyvkt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ixrvcyrp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lsebxuhp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fctujxgh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jkvmffvh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nmlikusv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mevsdsgm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3obezlpcc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kfapqbov.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbavstkf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nwegrqgm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3teclpsgu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ahtpsgoo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mtvrffoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gmstruxx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeveldye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rowiysvu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsqtiira.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sathpecg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pgbbhcjj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3prhulyyu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnuervl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3coaqmqnu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oagrcvmd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cqbuhfdk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ewxplfhn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3usakcauy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wwavrmzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxwvylf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qerwcvcs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tizvjhhy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rstatmwe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3obdybiyc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3polbfpil.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vdschohr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mzdyyyqo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xsofnyao.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vdubxvil.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wumddgbi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uouqrbhj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yoafoxkt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kellnnmt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqisuln.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yvsiojat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qlfxjptf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3apsxajia.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xdnjjmuw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uaztcmkl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mqfxdeou.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3amxnrtuw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3sbkjupxk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pnimpfvd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pivemktl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sscuxwpa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kycbozhr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rkwgcrcw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xradlksq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3sekilczi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nmucdhqb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wyfjghoi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znhxouab.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sfamyawh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbbwape.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hmixjvhs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zesohjoq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vguqwshm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ietqjgtg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wchnubvd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ygtzoxln.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xubgczrn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xnkxwgak.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gllzrsbo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3svmkejfv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hrmktvvw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yvnumlfj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eqwqtobf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3acecsyey.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uuxiqefq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3urxmcios.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnwkojeq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rymisuhc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pgejxwhc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ajdajyhw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3whriagjm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3odvutqok.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3brmfphkj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3osepqngy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqpeos.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hjeaoqtt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3urqkbhkk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sqlgrqms.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kqekoxny.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpjupwpc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zgxmffbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adzhbqrm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kbsunbhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqprgeyv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aijoesck.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rtpceaam.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qxpqcgah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iosxtcmh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uanfklgv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lmvrgcfo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dpswfgni.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3obgwtpzf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3acojoztv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ziqzhykc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iytbkhkj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrfqvdc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zphnkapp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3prbmpodr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vdvgqxui.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ukbcnile.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yfswtiql.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abxaiisg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pmyvoyxg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxehuqcu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3itizmzsi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3awrjmyrv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3npdaggjc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3syigwcex.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3clnucguj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wnhfcdlc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssaywffl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3udwiefhr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uxdvsgjf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vdotivrm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3natujfzy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cgugjgkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pybuvapj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3quwaxdik.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqkkmpf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uymvnrga.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vdxxmeap.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hvkqtdjm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rqjunbjq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mvkawsbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fzdkszqw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kgwjfcdw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gypdsdsw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nshbhmjx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3enyauvat.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjygdpcf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vebemyil.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlzuapyr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rkiphecq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kjyixlhd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nskslkqs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpsqgrqp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wiaqndfl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lxcelhaj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3paosqulo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pmpdvqxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezoslasx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jmequwdz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqknagqx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qedwnlkl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3owfetdca.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xwtnjpop.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibdfmsmy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dpdesogo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3inlfkote.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zpoyyfly.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3weidowju.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xzzhfcyl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqtzeeph.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mipjisqo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wdhkdgjv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wqaldhav.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lppjrxen.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3geigsgnw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vnflffym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vywuajfp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3svfrrxgr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gjdtehlv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzxjtqlx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ovgvnsud.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fftkazpp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wrekcbvx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cvnbjpmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jhtkukgo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xxtgdcyt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xcibfnti.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vokyoggn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3twstdywk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3optwnwkh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uqlrrbum.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dehphfvx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yeweoitv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkixculi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ahlzyabm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3iwzdaimn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jbfhxzfp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dhjepwpz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rclaogky.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xqyrgxka.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ghroefwl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3aodnjtef.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mllflyxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mywobzeu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ypbovreb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rsuyopmr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bjplsglz.html


<!-- 参考信息 -->