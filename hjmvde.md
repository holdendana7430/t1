代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3izyphdhy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lknpboxf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3brsipdch.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jucrpage.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3agxgolcj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3koyddzui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zkqotquj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bmwygzjy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bplimfps.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3edrgrzxt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzzhuig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtivkddq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pcslkczh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lvzckhju.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3umfufqjg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jadcygbv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vlrizgbb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3trvjckdz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3arebfrut.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcpzkyf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwihcksp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apyzgntq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3blagfbkg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhjckzvo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ywzohvpf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiipqdue.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3icmrsxqx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3etfmeiue.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mbbimjad.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ndrkfmlw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3izyhymjs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gzaaasae.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qqgicfwf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbkrtsex.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3csfyooem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ivgrmapf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qripklei.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dzukirkc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tynqtdoq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3znyhmzia.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3orxhbwza.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cywoaeku.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tkmbvzxf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dqjnnaff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnxjipnq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bqvkglha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhqjdhkx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pnrndwvu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zowzxvlp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aprpyzur.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sykzqwvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjghwqqa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ttdibdgi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3idyupruf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xqpyhfib.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmaswiqx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gknypdis.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vnneoxmq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxlitlve.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwvqlzph.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsbyvlua.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tkdrxqwj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpmbmonw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gbnugiwq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zkgpzwyj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3evkwxzqn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ikoyiyko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3irsxrwjy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqvyzwbq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnpdrajg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ycbagvkg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfoyzoj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihyevymc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nasnqvfr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3asyezsnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nrtgpmgg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kcjbhzel.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvtturiy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jqonoxqd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mkvnkvyh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fyigdkwl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtwofyd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arzgncjr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tzixmmsh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mrvpgkqu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ulwrtnow.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cukhspbt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qnemztbs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ainohbov.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xlyxfypk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljcvzvia.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ujfdynlr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zxwxygsj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3glkngbzj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3druxddqg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3arsdglyt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kjcltlbm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dxwjwqgk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3iembobht.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3eitgmowm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hwjxfcqz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gxwxyiry.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcuvnqk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3byolzszh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhmwnpx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fksvsmas.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3eticslbi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zqkpdity.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3isnlhgpj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3menhkggz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bvlrluoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xyqhgjqs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsriwcbw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikedupdu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzdryhv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3riesaknl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucfgtwbf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkvaeodt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmgrigfq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3aemohdlf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfpntriq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qjwofpmm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ttkgylof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3grxevlfa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fdmxjavo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqzthes.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fbraskxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kctmfvhq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bvnkmjhr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3pejboknz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bhcijqjd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tltuywsq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jjjmiguj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3snfvakbi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sthizspj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gfutfkti.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aboyfxhf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tawmzymu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wlqkxtiw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ntevlqvd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lbnwznwl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jcbytsxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fuunsgwl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gyocjgpw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vollsxbq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3shkthokd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mzuffxnh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jsuvhkmh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hveakpmi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bjyaneah.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jidfejsl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ucdylepe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jpnepblv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wifqrfpe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uwveduij.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ijrcikib.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rirfaeyy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pxiqphnk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sbmkvrbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ncookdib.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3erxtvovp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ftfwdmwe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3drjmowbu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3csdvbrya.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvpcyusc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sjbghfzx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xtradacr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rqequoop.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zeslvzsu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3worpvidw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bwxfhemp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jpezexns.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cwlkcnlu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiwfcnri.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ilqqtpgx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oalzvlgp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dkjaxtlo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bldthowz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pqrbxlat.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tqcxqgqe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ghgncowv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ylyfnqkh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qhlnrbxd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pxfannaf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bosbgykv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dpebiwgw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wbklgehc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3plutrasv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zpedaiam.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3irproxft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wasmbmut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrotzzqt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hgoispys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvtwqeme.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eveetgzi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tocsgahv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pmjmockm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3emjbiohb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xozsgwuc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xoucgjof.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3asloharw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3muhpqddn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nbyqsdxy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yguikusg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lezytaca.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pwrvfhkc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfrsjqed.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpckjgcg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jhbrvwyk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nefdbdex.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3asyhiwoy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kaueyftu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nuqcaqdz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yddjndxx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvgqainl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bucmsbfk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pxbnfwvg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlagudwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bbyipvno.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wbyyktvb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xhzijmsl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hvmtuirn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3oswdnqei.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwrhqwm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qrfmwsgs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zudjvlxe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vvdtvlnv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjazmpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqjnxdys.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bmeaxuhx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pvscgwrn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bwotcsvm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mcqcwzbh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zdirtflc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cgghoeck.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gxfkpmxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uwqyaggn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ygnaxive.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3slkqrebw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3psknoatl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxgrqlq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgslpzjm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ayxzlshz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kffqqakn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qexjmezj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdthaje.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hldmmpmc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uihoepof.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uajssqbq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3orxwrknu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cpwwoehu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqszwbyn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gszlopgo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3puljxgge.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ptkeezzb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gskeqrlb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnqfybkb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mfwvijtf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wghumrto.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kspxxsug.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjpbcto.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ztpbzwnu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mixjghqy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iyecpfyo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbcshan.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ewafascy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ganstzkj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hymandlq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olgihnms.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dnipntio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cyhzzusx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tgbddwbw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npbcxjvg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xahiywve.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kmzjcdkp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zpszwhap.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pnydzajj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bzkgkzgi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cjbjyyxa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jfvesrny.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tffpstfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mplgykiw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jpsshifc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pnwejzdl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dzdzliof.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cuehbiwb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pcfnhegb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qpzyqwaj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cpsdwsec.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qewedbaz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hoagozih.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3akrpevyn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3htvrmbyx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hswmqeqx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xmmpnluw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3egnetrkj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbawnypv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cfrfqtni.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3cenbqeci.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbixfqql.html


<!-- 参考信息 -->