代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vqbncpcc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uztkaryz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xhngbjis.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rzgjvohl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zozvvrqa.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xvxfxrtp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qghjgvxk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kmkypvow.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrceoof.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iqrlgray.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lavmvsdg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yolhotuf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cnjuhnky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2smboxtvg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fpomaaev.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2osrtluxj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qlhpdroz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vxsctuiz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2stborijf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qtlqyxto.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2revmbwom.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxtswm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hdoaffvh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvnnyh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zudvehjr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gwvsonbm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ztfuoiek.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aukmmyrk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2upkqzizu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gwmmnhck.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zpxffjaa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hwvxeyzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjwvszie.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tywsdbqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dknarwwe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lzergxvh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2otqywerv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wrslvhfk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpdpnnfn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hozbbvrq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xgeduoiy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lhmzmpyi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2smnrigei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ppazyosd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2baibypjx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2omghqkkt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcquwsy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tsxvaibh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrrhvrj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qollofin.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqqkskmb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hriqntkn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lwiyqkxs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkuotybs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nklysjpn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2alesuvrg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ahjkzrfy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wcanysci.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ujjiogpi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvcinxd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdztklki.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xbzwgpzm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kijjvvwa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ndodtifv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2leywgass.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ajodnbgy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bevosmjl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rpoftdqy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ziuduwby.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awoinfkn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xbhatfdy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wxumjdij.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fqlgdaec.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2oncztekj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ptamzurj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zrbaaegr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ccnanmpz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lxtixsba.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gygplodo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kdyfvsqb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ieqocpoa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2psgajboy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kcjnlzwa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mhnskjtu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yvalbwzf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2eonaurbc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fflguyvu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2uufcltks.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vpqwvyoq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nluvbnvd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2frcksgaw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xqquiwyj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xpckzlvy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ohzoxcoz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fjahfmks.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yesbyckf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2syibkheu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ckjytqhx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ukkxuumh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wawirnah.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bozpxhhu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2edgifobe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iuuzkuli.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gibfdozd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqyrcfhr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vwyzhnmz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hohyfdcr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nawhfwgz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyyavvdj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qadntifz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tbrwunjy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vejgkmkp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qyficefm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xhsbirng.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uozpznej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cotcgqfq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2coxlhebq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2epnssmiq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wekcpmwq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pwydmvwc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2itbqivpf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sgozuuxj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tfytboys.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ldzrkcba.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2paisckah.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ypygdttb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bfrfiwjq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2whknpfzj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xjktcslo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rvptpzoy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xvkfzgxr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2epccaqkb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mattcbcj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2brgheggs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xekzohoj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gunpksci.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rtxpiccx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hwysfraz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2txvkyzhh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2opjgtrfg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rpolwzlg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xzttdhta.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2higaedkf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kxoxylsw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cmvisxue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zjebqigg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2atjhpwvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ytnhkvlu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wndwikjp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ctnolfgz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yhwvmhqe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qpbqvsap.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mprjytuv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2unhdoikh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tcxqnhxz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2chcocfbv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vnptdrsz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcyqcngy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nescqkgf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bvfmtbjp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2sqttrule.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2llzzgjxx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pepxfcls.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cdpncohs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pilrlkyy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btoubhms.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nfillgrv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wfgrvbuq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yzdhtwqx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nbpzuusk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qtorfbte.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrqago.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ulprqqvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2clwvyjzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vtkdsmst.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2oflhjvyn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vywpvwol.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gsqqtlqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2duiheiua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eftqvoip.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kezkusfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkgbuszg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ocyunusl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mppgirss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pfpvylqx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2klfcaenw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dktxoymk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xakwcbyf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bztibwhg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bjijyfgb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2shozlaty.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kejniaoj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qounnyrb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwcmqtq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqtpfosp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjynrdkx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zozdegal.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mxspuzca.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2omjwpkkq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpgaqij.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wknjqsso.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmfcsid.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jznoeghi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cptwrlgf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ezjcavul.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dtluhcir.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2axwioyfx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mmbjdvsl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tswrmeyy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2veospjbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhijjxgr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypfqzulv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2usshdwil.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lcynpanc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aaulgzey.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2khvzazsq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrfjacv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zpbslgko.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2spjjqroh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jjdrszme.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mhyzcodf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2srkfewed.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vnvnngqg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vjtnlshr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ovyznnoe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eclxeqpb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ewilpnzr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2peupiufh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abyplqcq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oxdqtmsv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxurft.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jfwddfic.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ucqhlcht.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlclxlxr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vpuzunxk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuwvlu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xbqblhgu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2amczpalr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nldbinlw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbszqjih.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bobyfnoi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ucbainoh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nenqshyi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mbcyitjg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xqkdsvyb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xjmrfcrn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbwxlc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2eqmnkzab.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2irdmgxwm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ylmdsvlw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yaewpgea.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2oqtyhnmc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qexiclzs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzftjtpq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2niqvwtpq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xvojzbuw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rlgfaviq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pvbutojq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2oeptgoja.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zwkfwgqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkbuqtzv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lwyomfvx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ghxybgyz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bnxlggqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsmansl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2drbvgngw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zmonmvah.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvyyyzv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ekffxcvm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cqnytzkg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2difbnzwy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2flqximjr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iecrylbe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xeaxqirj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkvfcgck.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rqbvzerh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fvwdsngi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2isigfafv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwtdpgrw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ufpvscwu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mzvcclfr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nzwvogsy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zbqiduxp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ljrzpolw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kbhdbbbr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zectpoji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2broeexvw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ccbdchnw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2suowmgwf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rclbmght.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ajwvpaok.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2deakmfes.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bkkineuj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgdhsila.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ciapznlj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhivuy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2epunravr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lvbyiabx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vbonelmq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ouascgnu.html


<!-- 参考信息 -->