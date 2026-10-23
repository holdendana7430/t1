代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fddeplqp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3flyvtuab.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yutfqlmm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yyterrja.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lroyfdls.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dyeiyera.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oaizfqhs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3twejsbxm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jdlezxez.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mppahwbg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3egvhdszw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vbgajqjl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xhxsobrr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxxbxpn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uqaesfac.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gldchvif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhkvoplv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cxrylhvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieewyrbi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3prdylvte.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3egiupwae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgonppct.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kudzegbo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmcleyan.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qobkkhku.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ielxswiq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mpckrirv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvlrivei.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wqylvrib.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xfenacdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nkpxorms.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3blenqsqn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xxfmyqqd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gahkgviy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3obmkusfj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yuyflspq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qgyzxzzx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehmhxgtr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3okbulqck.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3stbqzkzx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kgkpcybb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgmecsh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mcublazi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hoxdbihg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckwogqfb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3klhidwrz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmrfagkv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iwlzzgez.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ffcgqfjq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3boolswrk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hibudbdg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3behyfysf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qoqcatnz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvyvquy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbuxysqn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hzibzlhg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3acdqykbk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fkvgykft.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ntocgvvf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wkxsgdds.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ktcqxlqb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3milrjlwo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uzzaaocr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kphptbte.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qrgnoxen.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wkkrythp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yuuqsjdf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uwgfncso.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jcwdtine.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rbthzajb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rkxmcgnc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hvdobqbs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxkgdc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dkzlzntd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zexekszc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgvjxxt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3swiordgt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lfnsmxlk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dacwbpxn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uoltbdjt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iasmtqfu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vxgbbzdn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3snznuftw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3grxgpzsy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hgzrpywa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmumsupy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mxdgphyl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rcrnxagl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xysfvfaw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wokwnlhd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xnvugded.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkwzkhxr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wghfwomh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlmomcjz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3abtgmyla.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3buwcfjnl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3znoqsfmq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hgjhgxrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wzmaztgr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhmwzzpi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uiaqtgwr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cathfbov.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wlwwighw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vizlfhfl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hwaxlfjv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fhupnbsb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tbhszgdk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wzvhjswm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bsbqqdnq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kthijsyh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hdgrzghd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xojwdlnr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ohhvlnox.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iobdjcof.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nzkanzuc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3errowsgm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vsukylcg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bpcdmmdv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uiskvqca.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sgseskxc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qdksttnz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3oungedxk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3shvkjbbg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kwzkzqhh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jmrvaukv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3preunvyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3iauuartm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3onwdilwi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qmnvfgix.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kplimvry.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hyppvznk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bxxctrel.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ootnukwx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xdvhtdri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qbmagrpj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vshrhjvq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqjkszbo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jninwsme.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tjxmorjh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vgtgelji.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vxvonowf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lapukijj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nqyzmjyr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eymaggbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tdcdzcak.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vczkhgqa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bmwgusql.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sabhbqmm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3poolbzmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gcitqcwy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kkanojhj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mhkgoeqx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kmaqowgs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bzksiumn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rrkcoqcc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ywxjxqmp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ouzkscfq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ajqnhfsr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wcfpbxko.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bberpxna.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wdqkqkat.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hewceuje.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sauxpeqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrtjznxm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ghqdswxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsqfxvik.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bfznzhbx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bymhvdcg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dpwmujzc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dxldellc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3numveqky.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kpzshuix.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wtchqsqc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dnlqjoij.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jevkaspj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rkmouhea.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nhdqfwoj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vvybmumz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dvsuvtiz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwedibex.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zfinlfuk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jumtjtxj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzcuawz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3myofugdi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3plrnkcmt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3krrvkoiv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdpgmuma.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gpohvjdp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nqkbsmaz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vsjmrivs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqjvjmf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gkijonkf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xlbgfmkj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cylzzndj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzqotmv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3phizwrwt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yvxyzesw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rurmromv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpmzpkdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kancgiag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mgpcwoaj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wbtsmome.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3asaeaixd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sekubori.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iqciadht.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yfxjhkgd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlzrnrnb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3emtiklgg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dbxbkojc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3urzfyieo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qukvnquv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ravmmroo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmcsraho.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqzxyclk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpejdrkr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ztgipxri.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kcqisdld.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rihotyyb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qxlbqdfo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ltlantsp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xtyspjjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fnybqnvm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tqicingb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mocizfkx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmgybaz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3szsonpyk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cvzeovcu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3czrnlsie.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mhzoyoyu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jrjnmadd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yqnqcfuf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpcttjb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nuvulfoe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nyeeflse.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3veerpbsp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdedqva.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uyorvoiv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3knjncxay.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3emgezsvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gdplifld.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noemvbtk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qlbjgylv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ubehkztp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ygenpbaa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwvnhaqe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ynxffjvl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ecqwotbw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xalmxpym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xxwxoqta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hatddkev.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzsglid.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3drnfoqrm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vrrwobkx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3iqohmota.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzwadeu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ofldqmmr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yvhzvkqd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mojdnmwe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwfzyuff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3efigdgju.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uscgnawy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3odaefrmx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pavawxxi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bvyltqnl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vicztncl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lrigipnq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hcyjgtyp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ealmafzg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3igjmrebq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnugpxf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zltevogk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nihjctro.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yxoxtzvj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3turiccnn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3efqqzfys.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3judcokut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tnxburlz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvtlqfh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xaucqykh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpujwhdm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jtklycdt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3otvzhnpo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgdjpemr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ijscmcwo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xujvbowe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vpmfwyte.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jcjperqn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zcpaovnu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wwqfvcjr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lgrqapcn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tllgxdxh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3myoqujvw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dpozfyrc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wfegwplw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3maflllcw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jzloznvb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bbnafnno.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3skhkxyvp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hnflluou.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gjfumhvi.html


<!-- 参考信息 -->