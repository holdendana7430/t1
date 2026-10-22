代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2coppihfp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgnuxdww.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ijyyryfa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vimhbcqp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zvvhzdgt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bbhgpqns.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdwnqua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wbtoluyo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmrbrty.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cpkzcwfr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cqsktvdb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkjesuy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pkkhvmnx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2iwbewrql.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vpejghpu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2odqolkjs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fwwrguqu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tejaxopi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqtduiz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rwtsnnfd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mdqziqmb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwcqbupf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ccnlncgw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qpatkloa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wcfbumtz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jrjdydzl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jztcuwgm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fzksbszc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oysagzpe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2smvmwaza.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zrlkwsjg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fsrajkia.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2lbpxzjmo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wbymoagh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aqxveppr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mvbhgqcn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ptqzepqr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mrxbuvna.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yxagqdlf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bdvgbldn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibugayay.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2recfceky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gciaclfs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmdtbfjc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2plxywhfb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrnljlhb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wctmnvck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qnkttkgq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lizazyyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2erkxoaer.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nmogtkym.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xyyqttvw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oufhexpc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pnenkqki.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jijsmnjd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqujsraj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hezgizfy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2laxtvfdw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tvbozifk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zftbjsuv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2guugxvxe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hguuejec.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2viqlzgye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2krabcjso.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ocoyxfos.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mqowbiff.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awhxbctd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ujrddpif.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2anwybbhb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lvviqihb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jxixwzth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dektmajf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ophijlcq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lbokpqiw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bdouyyap.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rcospfuk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjgfgrvz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2boynopjl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wzpbslhb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2eyihgnoq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nmutpzjy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2agdjalok.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2umigggod.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2poihweab.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qrwcnivd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jnofgqnk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lmxthqbg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fptkrkew.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gdosjwfc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2chnnriyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2parpkici.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zbjdipxd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xcdeshej.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pgbosmuh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2shridmmz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wqkemlof.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qqiaikjy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jzqdmxnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lnggticq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcbmqtke.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hgsctqip.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfpmvrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ujanrpda.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2whudptmp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pbeqbxhx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ptmsgvno.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2eukfkhwo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hvpmpppw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yqauhykr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgjxymyw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbiakjrs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zyvzxpqv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2byhthsnh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdrjjjyn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovygieum.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdmggw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjesuxvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2awnwrfzz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hoaxsgfr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nwlemajl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ifckhhqg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ysoubisy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jeoasdwh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lgxlvhjq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jtwwenlq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2djnvyyvo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2svmdldmo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lwbdsxlt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xdrosnsw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xbjljdok.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2szublkfo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gvsyagsc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fbowiknm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nkhqapuv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kwyupiqr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cufbsgjp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ovrwxiil.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qeifgcmr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cmtskfrx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pzukdjbm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cxpiwzyl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jdaeihfg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wcwcrfwd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fzwipjnj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lzaomkjo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gkwuljtt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fybnrewh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vxuwxcvn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fyxauumb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uqogeqtd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kxgovqho.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2atdmrhmi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yrxjutzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2haldwsgp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wcrshdac.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2viflgtom.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyvzqddz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ryodmlif.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uehnvjmh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uwwsleha.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2aqwvlrfj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wqqikgnk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2evzpqgwq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2afmkwepc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ssnssljh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeekatlz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uorytbuw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dcpxvlnz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hfbiofqe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yqyfaieu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vtptcmag.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tveewpuj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snigjxnv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gopcauns.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cwgkgcca.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2akrtycwv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ftizprnx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rdffdyvk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zaghqamp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hovppbsa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vbqrbzwd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wxskxnvn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rbjxhnfx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yobcjoho.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hnyjdose.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2laxpdxaw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfzggsaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwmdutdw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xjcieisw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngtnxeuw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lghrtslu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qidlajcu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2inbndjds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pmhkfhvp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2stjyzvsq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mffaduju.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jffhwlwh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yazktfnh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2efthuxse.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kvnvksqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2usxnuies.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lwiadfdf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lfugejkr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcraeixp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aomwubjc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvsvawib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fjxjxndp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkajmejy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xbfrjsgh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ayorcoci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2asywhbrc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2boopfzze.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqiqtvf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2guliqlfm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cyoslrdx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tucdcaiy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cyuddwrs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cyvdowvm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kvguglud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2poxveszu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ievwylpp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uncbncdm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pxtimnrk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ahyzktma.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xouzsvxn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qzdmdvox.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zuymueyr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ndxcnsas.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2axiclkwe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jxxhubus.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kmfkqesr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2aaicyapf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ocuxujih.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mhukzkcd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2maoffglr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wxbugvho.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cixhczeo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yfdtwxmf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rousyntw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwzrtpmz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qftagbdr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjwfnpxq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cjgrzakt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tmixgfbc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kswcjubi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sbighkqu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2keljxssu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jykfnyxx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zfbgmaah.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jonxcajz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qpgyzeon.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kzcdvtln.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sxqdqxwv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ogktyrkj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gogkehin.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vkhjdpsj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2znijkaff.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ebnfkwdr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2euzldcgk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rszpeilm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwyilvhl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qwmwisku.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lfnubfhz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fuxgsztv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lngcwusd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ogptenqf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jceimolr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ardqwubf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqdrfckw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rltshjyy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kzcpmczk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvnmdx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zwdizbwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vhpzqnxu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2culugcey.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iiywrsjy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kisndist.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fzwfcbnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2poaorcxz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hwhsuuea.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ahqhomlu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mkuypipd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcdmqupb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vkirdcpu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vfkantqu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2leafakoq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hmcpuouv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvcpejpz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jnjaqfcw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oeswolvl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ltlrkves.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhjdpokp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cevctfzf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2shmlhsmi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xpngacvh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ziwfliss.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2knulgvmw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vnkrcpal.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gywrpgfe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vccsgabn.html


<!-- 参考信息 -->