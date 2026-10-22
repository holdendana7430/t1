代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2iiniwpfc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ygntgyvx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rtzhjlxm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cdhygbcr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oqehctwi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vuadfpom.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kegprzew.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2aardttmf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dcmnvlge.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hkipbnrm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2njpoecgq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfthpmhi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tyxulyce.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lsxkkkwq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zcdtlcct.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gwthfdjj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2njvofozs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cwiejzyn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nmrtnqzg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2naiutisb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vormzwia.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qovbjrod.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gekhzyib.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dipkyylp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eldpaoai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cppovlzw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gblsmgla.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2utskvjem.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pbqerpfb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ibqhxwun.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2esgmmpif.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ociafxsm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2upwxaheo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wvflgzyd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hnjevbmf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2iqelaesd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yeqsulfn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gykeudzw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ixmmrhmk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oeokwrnr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kgvnnibx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2svczxhsp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cmjdemqg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dlelfigt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfwvjpyl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qtflbgqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmzdxmjy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pfkugssj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kvqqttfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cfsyxdhj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hbzferdn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypmweppc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crdatbgf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yhnytjjq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2txfyipcn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxgmsfaf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpbojjts.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cjwutezv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2deeemmbq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dglpmbzj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxapmnor.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hwjwsvxr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2snsquxio.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tvcduxfn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gzpqrasy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2chmhuewi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jbsylhxb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpgksphc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnvmkai.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ddywwkua.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bmfyhdni.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxpuylr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwdvqiuz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rtlqcwno.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhixdulf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ecgbpsoq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ieicwnya.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwsjqmgh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rkivqsbj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xuablxlo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ibzdhdbu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwjyfmj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uhfepeav.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xknmhizf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2unucblbf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nqpmechq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jypjmfas.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rpdgvqtc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vtztvhiv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oxtvqtkt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2faarcqww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dgpzsgab.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2atjiswud.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tjztmier.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rkrrnsbg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tnbdwgox.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tgjnhltl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rsguucek.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xfabqwwy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rmmbrcjn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vmopvass.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2szlwkhmm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gbvxiuxb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ljzgacui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2repqihoh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2atckvrwa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eswhpcog.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2crziyoar.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rglkmgdz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wuadoqpo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wmdoatzu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2blrpjisv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rccxisco.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fhjyayeo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kawullyy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rbxoycxu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fodazbeh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlsbahjt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uaahvtzg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dfgnogiy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uicatkca.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vmbzfxhq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pgoeyuof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2otaizvii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xplexwwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yldkzkhr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjzrqmx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vqlbfyag.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zpdezbxo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lssnfrjs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2adtozcwv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hwcyxeqd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xlojgequ.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjwspzhx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2umefmdnt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gugvdoey.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xlnweijp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zwewonye.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lpvbjzxj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lfmegdgo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vhbesfqd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gvuwkyzu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rnisflkj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vlbjoxwh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqghyq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vrvnjfml.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ulbkjuln.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2apemgzcy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zvcxfrqz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2arfxljxs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bpareckx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nhjqabym.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2swxavkjl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wzwsyzwx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iprufwdg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vbfearjz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uapgujmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dyltkhwx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jsgvdpkk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fksfqrgu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsfpfkjh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tlbvmhiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kyuezbak.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gecbcoon.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkcacmzm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2unnxsymm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mcclyecg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jdgeyups.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vauqpzve.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqoeciyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zyrrygpy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdndza.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2skgkwuuh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gysboiee.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kpxzumsz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjztxsc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mveijeec.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ekxqiiep.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sqcdgktd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2detmzsxh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qyqqmmjd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2khmxhzbc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ztzvuelh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2srjfbbux.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tkddvhls.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rqsrupgw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2upngtcax.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adxuoery.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gfzzxqqw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bncdpfgu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrlqnmpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjwgkgci.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rrwnwpgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibxlfvyu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cyzicgrw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wadevbei.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2notjdobz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jzxsqrxl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rywqwqnx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2iehnpjnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lfitqygb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fokotfol.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dcecomoz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2axpofhar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2uqxppcss.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqnjyve.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfzywnlo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wvxomaoq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2budzghtf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2clcvomek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pvicyxff.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2umubzjvc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2orrehinu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rcjmsmdg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2thqdmpsu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dikptome.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zekcpilu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eobcflzv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cxixdnmq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aoqcwgmp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2apnksych.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jawgadui.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2onvpykxs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hicjxgto.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pklvbtcj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfzgvgfi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2aapqaqri.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2smajgnbb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yezferym.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2heuegofn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tqtsfoyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pfvxdlnt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xpzgbjoq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pkbrtfno.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2clvzasax.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vywtujem.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2islmntsp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sbhdmrky.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jybpsnoo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkmutesq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yyapgkfc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndcvmrfg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2glgknsck.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbgoargk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fvyotkxo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ecessmvl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fkvqwmmz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fpixdnpq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vmgaximi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2iosxutud.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dfgnmawz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2priokbfk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcixdynz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zccnqcyj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kksqzgdq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hrqajsux.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sufzalbg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xxyupgwa.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ayncdaey.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ddvbirqn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xdsiwodd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2meugrapw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ekfsqigh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2umycwyfa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uatxgcti.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mvwrlowh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oipajgig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ktbevzuo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmfyyzxh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tyzfextp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dieyerlo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vchfcdqa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2drxsmwlh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jymiamlc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tuklsjqy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2idmzhvrk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wntjcdpq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ejferxdn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cxuzqhjf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkftuak.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dxdnsuro.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cgyslxfo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wjkgtcjg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ptqpxtff.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jfhebbnr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wnxhvkvp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tcfszssh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gwkbfitp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nslnclbs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2iwjusjsn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eaufaeix.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2epfacwdi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2obfyljlv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fopxxdpf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tuhzbbjr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vomzxfvo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2venjozjl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2puaxsthj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sroaeiwm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhaybspv.html


<!-- 参考信息 -->