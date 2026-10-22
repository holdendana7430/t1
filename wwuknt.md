代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2edbydguh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2oaqfnjst.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qjxykpxc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jeijndsc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xmkiwvrv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hpkcfftn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wfpvfyng.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ebqcgcvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmisrebl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xlrtxfys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wenkpazv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhxztmfu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2trboezvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohiviadj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2youylmyo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osurguan.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evprhtre.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2abeqcfgi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgolaqxe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vzwdtwpf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uhjfyaky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fhbuqnvi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2osltqjnz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njdxnsny.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2liglqgxf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pagkpgqt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxdaapeg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2inffejxv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gukoqouo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xtdnqsqs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jpmpmcdo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfrkgul.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvyadqjm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2veasktux.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2efofmzwp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yaftiwfj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2whkwpxpw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nutrokua.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzlrltuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2retcdyej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkuqyy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdntwjlz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gxpboyqy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ayulcgqe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2unjaccod.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rycsktxh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cxgjutkp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hwaxmsud.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ocmyjgtd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2joksetdi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2shpkhaqw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sjfqnecc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2befnusdy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kaqewvvb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kayvwsbp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2goywlqlt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ntamvxzn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yxbawpdc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uyatvktm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gieudvpr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lrxjrmri.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ycuzotwf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rhnjtwmi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fptgkphs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2abhzdjdw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rddvprln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qqoobfpn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ttodrumy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjcbrlw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwthdvw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fosymoat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zfauazzf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2huyenmgt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kqwgxflh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2knaphqkj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lyyacuqy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dngifhfl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ifxitpyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2epdvcexr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nuwtoxao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbhkyaw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xduigiqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvlbowhu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2votqepzy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tvzxcqtv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwrtyqhc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2clcsjfrd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jmbensnr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjljymd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jwpigkmk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xndyxlwa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bazmwkme.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmqnbngf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vwjecbyt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dccldaru.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2icbaixog.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2emvjfwcm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wxrblncx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bzhepmyy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fesejodj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wrhewpui.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bgvawtrp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2izjywoyz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qbsurtko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pzlnwfri.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kxbudsof.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2aeokwgpk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kizlhmks.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2slrtgqcc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vaorpyhu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pgfcwxqw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xuduaqgc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cqdkmtrj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dgrlltxv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uidzukhq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kmqjhjxp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lkebwkot.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qzhzighb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jqymowbb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dvjnlcar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jyrnwacb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hsycrglm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kfcepgko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbymrrjy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gdxwlkqm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rytsacrv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cxqmrgdf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pocsdrqp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kylavtdx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xosrtibg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aulqwiuw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gikmuadz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sddhaugu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tanqxgyu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iegcidyt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2waeounsz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kuiruqxf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cgquebsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tfxpleoz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2afkqexji.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnuqpzak.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmtpxnmt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bnfwtiev.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oeyhorfp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ntwuhafi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2htaypwgh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oehsrkwn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ckzvvfck.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2azljpbrw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bncahdbo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hhxavvgm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2egdrmwnn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uitbilfg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmgfprbo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phyvnkyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocidaheo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ohicjzaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hikdcuiv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2slqcrhxe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yiwwgczf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2emxskxtq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dsgbqunb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2djgosfgh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hmvogbwu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2khyobcjj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fxrzkcwb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qfktwjet.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zqfutfiw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rsvdbwzj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2escpercq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eneujzug.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ticluskn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zejnqhqh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nbexpnuw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2odepyyms.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jazwurrp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qtnmnkhc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ixhqfphw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nkijqres.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2llmrogge.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jvgydjda.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qbgyeeaj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tqabnlui.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qyoqsrky.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fbldxjpk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhvuoasb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjijefl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2guonyjmg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2filgiczy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kcodldlt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xvozkvfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mwolbdlv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2snwiprdx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dnapxval.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzfssuen.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ezgbhgfv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uppcrlpv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2klmtqbwx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzackpv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tpggvgnc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jjnrkobs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2thecbkwp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zlmnehss.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2schyncyn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olwqfaev.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyysyvhu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2abgkruhx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tgwrynef.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nygbfhhq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfatklws.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2iopuksfe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cxeghbov.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vijyvwib.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wxnwqjmi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ydtjpuly.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hogfnfpy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pmrglnha.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2chllgvga.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ypcihfdh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pebukadp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbtgxvc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zbojxsws.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yqbhkzwu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rvjtcjlk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rvxpsurf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vyonfold.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmydojl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hktbpinu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2itdiwgge.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2chyswfgw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wbkbuqrd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wolcrbpf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xvxfdshv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2plkwtcmf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fyceneqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2reodrkhq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmeulfjn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wsjeivjy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gixdbkyb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2btywxzuh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2owajcxcb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivxmfmet.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xxupvkuk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iulxwodz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2oxfpyvek.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gmbgancq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kcxpnugk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2orujfphg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ajwpapob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tsyxewpb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2npybdnyv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bpbttatr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2egfzztxj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hyajnxkb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkksuwfh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wvqsuqvz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xxlkxkvj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tekrcyhu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tqtvbwcy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnsvkess.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2djvbbhdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ojazhrny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uutwtfjw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azfgamfb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxporhcx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mgkgtuzw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gnthnfor.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cvirhyoc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xcqytfdw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkhgukh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbgxwssr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2onoopbzh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lcxpachm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bzkwlwyv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2suuqrwwk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2alcfngsz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cuabpcym.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qpwjjejn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dboruinj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxgugqnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmhsltzg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yjjwdulo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2riuhsfht.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btvirtpg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2udscesll.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qbkyjwcr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cigdqmwx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lgtvzjoe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwefcv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2feimpifx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2owbzaxgu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2inbejdhw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pphyqyzm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mivdgydu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbpbnd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kdakxatp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqyvaaan.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2txuzdizo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2olhzigrp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mczyprjd.html


<!-- 参考信息 -->