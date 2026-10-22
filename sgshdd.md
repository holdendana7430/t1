代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdnxwyc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmllbgnk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbhkgyt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sijdpieu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2smszxiva.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kgzwelbw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2luchhmae.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cbxejdya.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bfoviklg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rffcjsjq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjyfcpgw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zfenhlih.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oataazro.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2htsxsvzx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpwhfmcw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tzlqwflr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2umcjnjsk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iotfmtpn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fpruewst.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eneuqrip.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cnbjwzvo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nboemztc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yoxugvdk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nussgdlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqolfqkr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugmcvznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adrxgfxz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajlbcieq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ktrfgpvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixfrtdv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqffwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmzgdhpv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bibouoge.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nnuxhnci.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tyxvpduy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vralzwkr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojmwabyb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wnvkqqjx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enlavqwu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tduvfcyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wahjqkjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2oeglmndq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ahqskxyu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fpiuaswy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kbrpdkkd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zwxmgtnv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2iaikwtbd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kckvhnwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iwcnfmoz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2smstgnts.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyahjnrq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rfbdispo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2iqhbmiiy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bppizjlw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsbklqdq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vhzslsyp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqzzdjmr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wcpbragl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lkdonybz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2drianphk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ngbujxbl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhayhlep.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jljeimlm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ixkddohl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2opmyxnkm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2aokcpsxu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2crehfdoe.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2otlkamww.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hxzgonol.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cqrfrosk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oaoamqww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pjnodoqa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rrrlkkch.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2leuhprdx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cvjzdqqe.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2onantcdq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cwcmumci.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wwovgasz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2osrsdras.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jzvcfdoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gsribsan.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ysxhiauy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pnwzwlzz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utsjylsz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sjaijmqv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2arpenqrl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lnmpfhjy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kxixnwmy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oxuadotb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lbhgxoat.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pjwpjalk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tyzskqhr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmsgjhjw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2brlyrezw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hosfmvto.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2oedfhepb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2trhashnt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ybjnvlmy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbteloti.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xooijlzo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bziprbnk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbivllag.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hvvhvocs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nkyafhhy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dupqzuuh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vutgeuvz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sacqkndq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gqgkcadt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wnrtfmmh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gwjxmgkd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uewxggkh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yfupancy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2duprtvoc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhmwgfdb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xtpaonac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2iqlecxxj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yqsicryk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dvtxecyz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qrtsrdtg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pdfazwdw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vailphjm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gphiukku.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ppegabvh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wxghdofe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zsmahdfk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2poflgjey.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2owysvioz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hvxgtwkm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jxzkzwlt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2msgmjcpp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kuxxfqlc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yrumbqho.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mxgitrqx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yhlaoaab.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bkwezxih.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rucuxxvj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qlwsymid.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eolayqja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2akybczsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxgbfobg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdulwips.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uxpgbthi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wiopnkip.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jxxdmkdo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oddqzfnk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hnwkdexg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iayltokk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zgbwdorv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbmkzjv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxheruju.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdzfhr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2etmlwhbz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2chlymrnd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2txwfjiyo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qttafiyo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xovpkfsm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nooraiwu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqfizuee.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dxullpgo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yjloqpiz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cukbogyk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mtceoggx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ldybangy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rvwpojab.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cxojfnro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vpetdkfj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2raqynwjn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yifqbncn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rtwsppyf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkvkfedt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmkwznuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfdwyltu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pbpnreof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2samrdtir.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mbprphkv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsireo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oeottrvw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yxoxsbsd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hsosnpyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2coxyrsdu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aqtvosoo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvjtts.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2osplexdb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2eyqyfydy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kleuercs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xpnxeoav.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2izleoutc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmlwzveb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xllvqmjm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2axtyzoah.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tfsrasmu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tihxgsse.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cwmzeuue.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nasxzbcu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2quhzlmvu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cyxihawn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tkudthwq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jskdsnxu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqopomc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dpvjdzby.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wiiyzkpv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yqxzerxb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tglpzwlw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2deeglxcx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cbadvcye.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qombzfwi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kryvifer.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hllblgst.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zsjmhqay.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xfjzkhuy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hxvlzbli.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ehokkdaw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhkfsdu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2btgijotf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lzredagl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uudahyev.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ahxprgiq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dqywhume.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lajzqehn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zjttexoh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjqexrw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbelpceo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ncorsbzh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bzaoccgv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2apnnqjir.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvurpge.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ykvxbhbx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vxwigida.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2akbzsxis.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cksibjiq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bpbrygui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2synaqglf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tooujrlt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkutmyhl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oepkcwjv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hzjrkwii.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2momdjlsp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xknsesjd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2obonnklu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uodktckh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpdpjbf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2brswxyff.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nnggqdtn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2edszjzbl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2worzrpah.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cadkpxub.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fweeetmx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gxneupbr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzfbwwqb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2isrwqoaq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2stawuvul.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qqwgsacw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgrbkoqm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2smfhqyez.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ioaezqme.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wttnemhm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2obfgfpfk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmlojcoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhctcgi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kykzibar.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dmqxfwec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sbljqqqv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mymgmuhr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kejyiskb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqmqnsni.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aswauepi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfoqymhe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iezvmhdu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nmkabmid.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ytjhpbhi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwpquud.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aqzhsgya.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kudseqam.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yrmrsqsz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tdkkrbef.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2andpwxpn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bmnfaxwz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nntlnqfn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bhcbotmn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xitsaqqa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2voyunfvq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mvnrvcft.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vmlafkvx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2sceyqilp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yeyxynwh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrguyemj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ycnbunfi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ukzhsapj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gmoufukh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bfzehatb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rjnbmmjz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jcpgjxyq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2byxtjbjw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mfrqydrr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvacvb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhnomfc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dakskfuc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohbbjwcz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jtcyqkjf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgekagtv.html


<!-- 参考信息 -->