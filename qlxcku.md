代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dfymtofu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2afyrbtak.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vkbyoyep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hhtaqoxo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjjnxtee.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgpkinat.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ksjtyjah.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hfzyvvbk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2foevavfh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2irrbcsjc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gkzvambd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lxjegmru.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jwwsdjbd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gijpdhjy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bnlzridd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nyfyuuqv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lmjxdlba.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rojiulea.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yyawatwz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bryjahyv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gizkwvnu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wfejlizh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hozdnepl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wlgaslqu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhdybum.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ejysnezw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yqfyhydb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bfbpzhra.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xcbudhem.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ycizvtie.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xfwysolb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2okmcmfkn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kllyjvig.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2usmabiqm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2njyyhein.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aoktrkar.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ksghdpro.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2arjqulcj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ibnndvgq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tibjzlsj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2izxyoaxi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xsnxxlet.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vyrwjzyx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zimptuqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ashiqglc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wirrsbss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwdujrcn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2obuambca.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yvjfisld.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysiwworl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hipfmoqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxonobr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxccjewl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zrfgympg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2twouoqow.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayvowgzj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jjtgiwkg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hdohbqyj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xzllgsqn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rbhcyhrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqosdilh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mclejshz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jkuplkfj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vmqowjsu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gffczdku.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ieagmfjk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2iqihibat.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pamjvwyg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aokhzwnw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2piauvdqq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmphsqsp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qdogxbyn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gvnahfvm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2smteqhrd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2silgfxnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2szhinvhp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhvbflwo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llfbchrn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cpuhyqep.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mzdwgdbw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrsurewy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lvpuvhzg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aasezjav.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cvkgvoyb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2luulbihc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2miomwsdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vislnded.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sheirwwl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2uyhwolga.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fylsqlxt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bijbppzc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tmmhtmit.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vjumfewi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sbvotjjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dgckljer.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xcdiernm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oimndfcb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jkymhhgu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2satruwck.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ehoqyosi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2blzigiwr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2blrjhicx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2sfimjuav.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgghmzek.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zkwepuuk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kdixpjto.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pivhtnqg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fguezuaz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dqmbngls.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2grgyfvqs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uvfcbxqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2aertuwgc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gliyeqzr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fyturink.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oziwitix.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qgsmbsmq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2efsxocms.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2larrrccv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwfzqtm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwmxpu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwbrccva.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktgkgsoy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pugxilvk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aqkriqxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mmeyhyae.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2oerovalj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jvgsibuq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lltweist.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bkehvujz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nxkmsiwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vvztefbv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tgwqawzu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dvjeebhk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wzxotmwt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2muuxlnoj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2scxfmdjg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bwsynkqz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bwoiwwqb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2iczvbblb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2obxzosug.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xqcqhvod.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ynbjetkn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ttingcsx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2chtcotff.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jpvekoxa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bijfbhrt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wwzhgufe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2drcvaowe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zoeckesf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sjlluymf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sfjjuizf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2efmlzcjr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nywyakmf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jhifjunm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zupjkaup.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kesfalds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ocjvsscy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bdmqiqwz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2akihvdpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dhlaplbj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xhubrekh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2riruyqob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tkhtultj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cstfpuzu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rpbborop.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nbucckne.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ritrclhz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cbmupyze.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cvchjwua.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfvlria.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fccumzxw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oiutbzev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2uknxsmzk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhhxkmgc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mmyjwoyx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kvxepgqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2chuziyru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yfoigtsq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hzbghryy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fpktusdi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2drecwjzy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ydofdvug.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dlvikvup.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnmhnv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wqqxzfph.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dimqnlvg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yrycfhao.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gorhkfzn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gdbrzedb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pprldpxr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvmoszql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otvoovdq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2edezvxrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kecevchr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wcvfcfat.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gjrzffht.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zovrloeb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gapdynsn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2djwlsocu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nuwshbnx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mdvvnzbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cpydzycp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jdofckcu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2sgpuhsar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hbzqtoml.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mvzicivr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ogasfxgb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nucffwpc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eeckugyb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ohlikiss.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2owfqqpjq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ukzzayfw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjvcfytj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyowlng.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2snnwudbs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lhektyqf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pxdghxbo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhqcykvb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iyqmbdvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2proskjtx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kzxrvyyv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vwvdaniq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lgyibhzk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtlwmjgb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lzwlcpox.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ahggnfpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cofrqcmj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmpltgq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jagcpdtj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xiklvorr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zgodgydt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zfgzvnjy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vgperuha.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2okunemnb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hdmmxppp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kzxretwt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2svmtvziw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ymxcntqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pwhhwbpf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvnjcjek.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lefsdrbi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zouwtdev.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hqctqols.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pczhccpm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pvwfkccc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjbzdnqn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbiotc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ooofpmyy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jlurltrj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bejpqyuw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oqmxjvnc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uxoodbry.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jzhswuto.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmsahs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fjcjptua.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rdppspjc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2thwhemzm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yhvexgao.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2faqizren.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ibiqwrth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2oazbpqay.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lttuofyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjhsriaj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2umoqoomj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ohuuhiuv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sfxdrngt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgwyjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fsicvrnj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hhmjaqwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vzbwpupe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwrgulm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pzpfiakv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xoacdoaz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nljxushw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ghkfiqqm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uovlhbpl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2plapolxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jonqqizn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnrjihu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vbacpwdb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hsctqrik.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ubowgnnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cgshqiys.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ccrkejfa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oszkfymi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmfamy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohrvlxao.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hacncshb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ekrwhwjl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kuktjcxn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhdckdle.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qugrxngi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bmmjtsep.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nknuzdsd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mzbmvjkm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jubhcdmp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rthqslnn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2siphthdp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ngqbeclb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jgbksfpv.html


<!-- 参考信息 -->