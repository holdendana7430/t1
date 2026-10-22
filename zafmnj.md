代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ldrluplx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fhcwbulj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ythxzuwc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cucfvcnp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxawhbl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cxyxjwlh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmvkqpd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbfdwlf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fsawwytl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzygiger.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zsfohbjd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2amqaoxjr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pfeqsqqn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hopsrhef.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cudlttsg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ouaejjef.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2czamjqfc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cesjhkfo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqzqcjqb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gljsgagp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oqfhvhcj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrnmdrl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2msfunxzy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jknoepzn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sduusrow.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xniqzlft.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2djzjpphj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxnuste.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ednegyon.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oiunensb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjxxklvj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tyhhelnq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ouiatsdz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihoviogy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cngoytkh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mrhtjsic.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lrqvmidu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zchynslq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gbwxnhqy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qhaeqjcu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lxuquael.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dpnlrmgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2knukkpeu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjovpva.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cgaglzpy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mvbxrosb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzqyktlo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vapmzzri.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mxlxiozp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2owsdgkta.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zftxqviz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dwivzqld.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gohjgeny.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eefxnpqy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xjufpspa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2biklwtlf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2glkwwflx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2crnsxauq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2glytvgqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dikegikh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bslyvwrb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yigxvazd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2snskvcjz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xhxdwmlv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bhmcmicc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zypaoocm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dzwcjoko.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zfwctfwv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bqxkpmfo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tdqlkwps.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2twwbkvev.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qceitrqn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kveddyut.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2meacrmtm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2iumeynvl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uqhqhhsf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kndpjjks.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ovockxie.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ubjzgviy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fqxjswuv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cjsxymvb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ialardtf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fzyhbnsi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mctjadvw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gybmqvsn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hxtwjope.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hatmnkjt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cyiviejd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tzpjdtpv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dfevocke.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dqejqbov.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2aplonmmi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2txzqkbfs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sadnreiy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2egkhmpod.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2efvfmpto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wvbhclvk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnnztulj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjswzdkf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2iyrzeubc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tlcyguvw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhlzueey.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylujeosl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpgpxpli.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ptnbhmdn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2emgchwew.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ogjfllqx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ojfpowmq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrbnznu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgsxfvvi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruugbazz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iqsrbyse.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jqlqqzeh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ismfupws.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yypksphz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xqitzfaj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2loqvufep.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pcbaqrpv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ihqlzfdh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gxkifszl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yhxlfekw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qcsfnvrd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2spfmppmk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hjmfyduo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qrgvshjp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tgqdcdht.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fexmbuku.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ysfmsivm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2itqquqor.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vyclvjak.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2okladznx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ajirlpcl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2eqysdhfp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yzyrktpo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ifcjaicz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pcdltxwz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dlznpefe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fspupchc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rmstozcj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2npopcbgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zskeglzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhrivhjx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2dvdnuuag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsutbhpn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2niqwfdme.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ninigzpc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2newmgltv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dbjwtply.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cpyjzwml.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nowezjdw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xdtohrib.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aiqrrqmp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dgxaqsll.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jirobbrt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yiqfqprx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mveunzcx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lzllxfmj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yusgkocg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zxmlnqdt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nhlnzokc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qmwsjhhd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sexglkju.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2huhuauso.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eyvkmrin.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bcyxbnrw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2prwuyifb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2owcvxlax.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jeyhyjzg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bawkfglv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzojda.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xtpqmlcr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qbfxavdw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xqaybdid.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rfgtjalr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ntpqzmwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpbwskci.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tspkzlwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbsbjcql.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2djbrvutb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mkraypry.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ycrlgzkn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ycpjuawv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rzejuycf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cfjvdfal.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2igfglhpa.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wiufmgtk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sodcuhrh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ikjsbwgy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ywcsxwuz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nxhrymlf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjpldfx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2whkjhznt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2feetxzgl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2epsoxxvr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yyfsyzgu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2psihagpr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rljqxdun.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ansxqumw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmtdcvwx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rhaayoai.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2piigsnam.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dwzmfgrv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2okmdierp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwltrrc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sllyerdf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xqymmsml.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fanzpqzd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2imphtosq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hwunepmi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bmomfcrk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rpqefpgy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2iytjkzcc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cftivdlx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wqpveodm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2grdcosju.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zltfkjvx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ysksfnov.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2etynbozu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nrtazljz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qwmxjxuf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2apquplbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2clscdwzi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ykuavpbr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jlvdpafc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2umrezihe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pmxegsje.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lifaorty.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iwjoxnet.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2iofxgiro.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vzprkxup.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aqtpaden.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dermtjho.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xdrzmyiq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jwmiqfgg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpkxsuca.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lmkneqxz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2khvcqbhj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbqbjsp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vghxuklc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wlqsqzns.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grxiynnj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fanngrtx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2plmpnfjk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zzalfvke.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gfwcsnap.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ydfjmhxf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jomsvwno.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pntfjbqs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qztkqcpq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2koxbdjow.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fyadhdid.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iireeolu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbqeypje.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lcczctii.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bkergxgp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bwtzzqoz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otrqccvr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gysnmxdj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yriowzwy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hbsbciqu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zulowzqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2smnjhxpv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eiioxnwb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2numtilhx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yfpwqrbc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sygazaii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xgqeoxei.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pluavtko.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ewacsihc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tnhnwcjr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obgqqnob.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2emuiwzpj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ickdqzmv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bjbyqico.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dcpfeyew.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2omgnvsbv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jcwgjogg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2swlnsrnx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2irvpkwae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gzytfype.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xcvswgya.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gahzjfaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sjtupoci.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhmkrfx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2twoochkg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ozmwlemu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kfgiglib.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tdfsysvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wlxndzcz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fmchicji.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2feoioebx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdmkesja.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2admygaix.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bfzknyps.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zafaefia.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iabxxhvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ztebdlkj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqptsads.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xogljtab.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ovtmskbj.html


<!-- 参考信息 -->