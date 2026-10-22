代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yylsswvt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgeirmge.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2solxcpgx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ugvcbouw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cicbkwtw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2crwfpfxw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzcokaw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ekcmsnxc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tbbrarjo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kxjjraqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwkgjkh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bowoxjkz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zwpkcorz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rdvwgkrl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mylmfevk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdbpzco.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzgrku.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aorjeipz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ogmmispg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2flaoxkts.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ddwgxsga.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxbkmpvz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ahucufwp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eupibapd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ulvthfiy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hwbzxxxr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2isfgcyky.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2itthyrut.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hxtnrmec.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qxhakioi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qzdvpnvy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2umzsvqza.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2otswmkmq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajdykqtu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2evsoaiod.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2emhkfqqk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wjdunepz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2evfykygb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vmfkdnxs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2svnqvndh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjpbczbv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tafclpvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfycllij.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2myuixwhr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lcicweim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ldeirfgn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hrbanmzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2taufvyir.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frgqfrjr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2izetzmmr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2itjdjkxf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbplfrbd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnpcykou.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bnbjdith.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2aqqhsplk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tywvnjcj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wjgidmki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qxdldrgr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvrwbowp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2remqfcvp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xfojsjoc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhejlgto.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wipnmhlj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gijttcln.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kyfmbszk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tupuskht.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qtirqjqh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdxopmy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fvaexyqk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2smsrjalo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jmjikwiv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mpydppmz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wluevozk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yhpooads.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iooztisc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qsqztyme.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gyoaeuwb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zptxpsnn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlszkeqj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vzgimolf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2optofzaa.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rmwcrbdi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uzlazyrj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jaimthfv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2peinykim.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2utyhxoch.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tqafvzsc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kfsknlre.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mgnsjman.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bbilhfql.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rlsvuohr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2baxirxnd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2taybslru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iptydnfg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2aoqzqiup.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwthqcm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cexhpdtp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bfwlofbi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dsvsvcav.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dgtgvrbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jzllflxi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jptbgadp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ttvqqyxj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bgemqdyl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ewgdfqwg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2svcncoab.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ordgumlz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2luhtzcpz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2geuyqrnt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmloqfuz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwyqbey.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vzasookm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2regajmxw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nillnbzu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lqmlorky.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rizxbpnt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kdlxmlsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjdzqajw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jjhajvyx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2twuiayql.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fimcqfye.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rdjknekx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zklzpwjl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2twcskhfo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yjexonmc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vduoejjs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2detwpygp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ndetsyyt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qvolhiwh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ydnqkwhu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tmjuuhkp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yvkxadly.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rfqmibga.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2skefzdhm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tpirnkvk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ggxunkgk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kqjzknff.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2srpvtitp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mkwgkrdp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yzrszkmw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kzjebksb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ritdnsxr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wexgozgz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2krtklnkp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kkjlftqo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yggruvju.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iuoyfzre.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2opaskbhv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wikcnubl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwqcqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ybthdrzo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bbrrworn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2itjkgglw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocildneg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2anfaghfb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vwhbmvqb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eilxbhew.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rnutxyiu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mkuirbwc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nkoxqytj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2osmtagcv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wspygljm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fbkwbcbu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ztkfhpvv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pdkdnxrg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnxfbgq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsucpdr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kacahwru.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2duihpqil.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2trxpmmqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ucizkahw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nukwsiqh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vqxijlbv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrfjezu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dwmecgie.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lbptrfjm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2oepmknzw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2twfilhpi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qwudwjrh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iilhemoj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2exzuucnx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kjznuefq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hctaxqxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqhyvjff.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2srukuyco.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpbofzps.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfpcvulq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmmrikzo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rmxuwkvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlnvdlqu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kbolfdas.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nytahjyw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2icyvjtqk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oegyolpr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2hjfjkmly.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xnnlzquw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2daysuzvk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2aazyhdka.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qpfslaoe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jaszyiyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rtykavgy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cegsxetb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usqrgjac.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2soqsetsz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cbodmycu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mjuwbtia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2iaypgnza.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agdnnowt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2knydjbpk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnatpxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uicxizej.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ngfvydil.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cbvuahnb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnbcwsed.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wpajklpl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2okpfqkos.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jockpcuj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xuffujve.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jloofwju.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2whtzxgdi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jkfgfwmh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zortpbxk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oeqvlsqp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2scvqqrcq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zyqrdosf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wrqlejjc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ykgmvier.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hpncewfh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ilxbxkwv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bgqhpdop.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzcwbiyg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lvtlbuep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2byptscud.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2igiobzlk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pbqedcxo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ertlnywt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmngtnqn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwydtcxc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cbmflnbo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2crsqdbot.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wgfptcvf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlarzrbs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iwdbbucf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2clqjojly.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2epwubtdk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pzjbphgz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2azyswxeh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kdwwemgm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2abqletiy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2skfecozl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nuaigbuj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dcuwvlcx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pzaogjbe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pbqdqepa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxbvbiw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2enclelgu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lljffrvs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yeptxkkn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwjeyrku.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dehcqtij.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rzcsghmd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2osxfwjab.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xscwcofm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2grcdcppi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blaycamv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2aaxhdklf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2klancmtl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2otsxuzba.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpypsskv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ycpylija.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oqkspams.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nddyynjr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qswjxooh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppvtrtlb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zcibusbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhoenry.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mqccgzjd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tdlacggu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mmmepnpu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2likcgjfs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ontzvbpj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2caicknsu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjuvjlsj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nvmsynth.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yscqjpbl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xugwqbnh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wirmylny.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ghzkbwat.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tielqtuy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mkpkuswp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2frclrjuh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bnpwrwga.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nsvlfxaz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2orhjdtii.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hxvcumhn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lznzmtfb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ewsfptgr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2epjqrawy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zpsqccxp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eqqyefna.html


<!-- 参考信息 -->