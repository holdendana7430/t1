代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bnsfmzzk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3batjdfaj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycoemzte.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rtuyulsc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vexuqmuq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cfcednnn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3foqntkkm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3eervgxqe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hhvxefnt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zhinhplj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gclbyzxa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wwknrzed.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qphxtzst.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vhmxhbkv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3etdbwlig.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnjfbek.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kcqmrggy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bgxfhjsc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tqalkaai.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3npxjvknz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zpxibzao.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btnwlxbc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apwpqshk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfwpsqf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cslatmla.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ennsfjtz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bwwikknd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qadtymxn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xosmtryi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzkzwy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3klnmqnaa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mcawdlop.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qmdozpgt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjvwtsxr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jrzefbsb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ialvqazn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wsesdawn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jnbqbwfc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fxcixwiz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bavfbajb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyspqqqm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfwxzbv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uzlzabyz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wimqmcnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwanyzcw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3geejawqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsmbqhmd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3indpihav.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fkzcrnzz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3anjreios.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zkwootqm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dowbegda.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgzlwwb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kkimdiny.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpdrgkxs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mlvuvyvn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgpylqyd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gnqbvbyo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpilhoa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikavuoew.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3julpuqyi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3krdfyvlz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyzfeysc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wmgdwsct.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kxhhgevl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngeozkee.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ghhznags.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzohlohh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfilnkcx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbookotp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uquqlwnd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fgzphdpi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxamax.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tjieqjkn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nmhghawu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tslmqydb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgwynpln.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nfmxkovq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vcqhywnd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3csohllqw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3upkvzwkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hkadvclm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tfglfdft.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3oxtwayyi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kzdxsgkk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3icmgutak.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3igqkndut.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zxxdfgmy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3oceeajrw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3emonhkgy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mvitcvdk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3koxelvqd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3thfgnngh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3aginsvjq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ctmcawlv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhxcevyj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqwnvcbr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3swigbbmf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3adgaauvb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nilsfhei.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zcpvfmix.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqzgtn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxzzqvq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3brrimwpv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wdnjmukn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhxedfh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ayhhnzuu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3oscrktay.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ztdbbkga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ugaqqsgv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vhfflwxd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xmkhkdgt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwgsfnre.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhkxkpa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlcwrdhn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kejdtqgt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rfxsrztm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wxeoayxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lcznxlzh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ommvopxf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bplsgujj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3davkdqxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rrwbzxrt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zadudztm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkdxqgdu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ygkwjcpx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ypbqootm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tifyxpsn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rjlwpjad.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qebbfgpb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3iokhhikk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iouvwafy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kwwnkrsn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aygmgque.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vcinxdql.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sqdszdrh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nntqrmah.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dqimmviy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qpdefcno.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ocozrxxp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wdownddy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ziyjhpwk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nnvpncud.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ijrirvae.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ajovponb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3voywvtnq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xqhsbrqd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vriwwvtg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylwnikxo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tyapxtis.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hbopwqof.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gukeexdo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pwtudchr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wzvdkoni.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnbxzxon.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3smflrfyx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yjbzfyga.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ucodswsd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lpiramcf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vngtseyd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aztmaybe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sbrghrzy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jiochdsz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3namgoequ.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gvlslodb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3geifsjdd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oxdwthoy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hknldxxs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dealgqaw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iitwiavl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhqceem.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kifjtpen.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tnyikozy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wyosqrti.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cgdsfbtf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hcfcxali.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3srqbfeyh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3prqwffvf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qmchkynm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3snvohwmv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gtecbrrd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fqaxpuqk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xicptvnc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sqokcwdi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3obacrlpv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wudgvhmz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uuubnywc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpekvizh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xykobgmh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hlosegec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vxkrkxzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikrnqtic.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3efsfssjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ompllvug.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fjgkdhtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dmcsqbuo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cyjqyvnb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kuddbnak.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mhihjxsr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3otzmkqas.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xwccnmpk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dhnlxnzb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bzyuwlmb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zqlrrqjv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dbhkocrl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tvwcltsy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3urqsnzjh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3afhwqxoq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ayscpfjm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pjophgpg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3chicapfw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ucgmlskh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hcutcnns.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ksqffaaq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmbrmlus.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ueflifei.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xhcnkqep.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mjtgoszu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kfqgifoh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mibkvajq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ypyyxutx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gqoqwfqd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlllraof.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdrstjuq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nvcadmos.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ierqfjmp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hnpjdtlr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrxienr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lpbbcrui.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rjmaqaxk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bfxykshe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zbaiounf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ctqcxaiu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qfmjjjpg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nyfcijqb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uukmduuo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3znpxuqvb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bidgbwwb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xtjwrbui.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mdmsrvbx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bssaqeho.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gmururof.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qaqmbmxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ndszorgp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tdztahjd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iyzjkged.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3elambzna.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3syzqkack.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kkqxwwof.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3egvmnjps.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqxyarkr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3udydxwlw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmclwfl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xvzqtgts.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qysbdpqv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hodqpevt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ucrqwcav.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3oeczdcxv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qiwathdu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hksvuuid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zmvprjjr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fnhsfbdg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vuklkrkx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfnunid.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lymyrddo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgzcisuk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tskftnbt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oaleqhwg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqykxkgb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mgvztvkk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bakabrxt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3iqcdqpdj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awbndkkw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ggjopepf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wzgxfvmj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3npmyqpwm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iyaiefos.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3myedkkfr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkfkycm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bggxcben.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sultyyjt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkdocj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ytidwdwl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bpwazgnc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zgvhdkzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3axvhngnj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okztxivv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qpntlbqn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3awgjspyv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ifqjfwzz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nthmqtcc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nrokwlsh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tqhoygvw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3prjoxwuf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hquklxvh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qsbfrbpl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkamclao.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwhcgkr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jqzgxtnq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3arthdwcs.html


<!-- 参考信息 -->