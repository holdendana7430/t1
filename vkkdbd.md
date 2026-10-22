代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2socqsisi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiiqezga.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bgqlavae.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odeznorg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2icvupnvy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mexxszob.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vxrnnavt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gyncuafp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szqvxgny.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tbsgqbqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcubragv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bozzxmrk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2krwpbuny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iedgjzjb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2klwrpwdg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrpwpqde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oafrdkbm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lhteckqu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tksnwmhl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zdvdbhkn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2clgaksgv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kkotimkq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qikrlkiy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdsamhd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkoaegin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ggmwhbwk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2chagrbah.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2detwiqlt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pksyhrtk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jvnbrnox.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yikcnsox.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnytoqng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2esljempf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkugtgtm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypnqsyoy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsjeuzu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dimhljkc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2clswlgbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mldofsmv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ozcjfajx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jcfjdnix.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzxvbmgx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jvblumfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dspgdpqz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mqaxpveg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2klquqryz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qiwoulgk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gilcnyoz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kkkfcflb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qikhicfj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kebmofdg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2adypadns.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2nwccpjqh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ykxxcqvz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2opurgnxz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kketuojs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tzsfqodq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yydtadso.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2njppypzp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yrytgrqs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyhkesbi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vpdfmxdt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2apkrpzfg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kqftvjrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2puunlwlc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yxdeprur.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ujrepuhv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bgwajqga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2owmwhvcb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jifuzuhy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2omwyrkdb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lomreprb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bzxpkapg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bpqrpgfj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2krxnhkfv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2llanzgds.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsqjkvpe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntyjlcxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awykbikg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hsekaaon.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sjqyzxwo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ksmmcovg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rvumisel.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tivsfsaa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2useuuwkt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pcimfvxy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xfsynegy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2epykptqc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjryfkho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nupcbffk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmtgxsy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfefbeov.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypldfuph.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2orvabfhs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xywjxwmv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2voyfyzsh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ekbshnif.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xppgnelc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pimgccce.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zifwtdru.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lssnocmq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2woeojkhy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vbfsffec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2japboukc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tasomnae.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2axmtvwpj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ircxwvrp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bponhcsg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2plqnmcnl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpfunwm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcrslc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2pikenbsr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zbpbxcoo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bqslcpqs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fjtcwzvv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zpxmmubr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iqyysdsp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2esorazdw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtkpumxp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kwcarxod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fbtzuksv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yybukfwh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ssehrezz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2chfbfnoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfztrxur.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fjotkzji.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ifedmvha.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pjeefwgv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2blidxqnz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2miivrqlt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2izpvtnln.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2plxnhbhm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixogoea.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dtqmxcti.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbfebvv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qbfplwif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ggfnrsxi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2obdplpgh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hivxgnzj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2makpecbf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2virftnqd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pdxbzqgs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rdzmgven.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bxsfuxzr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ostxytgv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zimiucck.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cbwjxzlo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zyjhwxbv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bdzmwafh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qipfsrxq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ffbpmfwi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2docczgzc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rrhwpxjt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2olbslppp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ituefuls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stycuvwv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ftqhnwqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwoxjras.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cxcakzxo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2myyccyxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vtidsshz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qomecbsq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ngdwbmbj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dozaznnu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fustllqb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnregadp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jyakgeyu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xmpuisza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yaxqawll.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wkhlhmro.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ohvxbkul.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jorgezwq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jweaxiwd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jqujdtkt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nbcijnsp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tgduqkci.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxyxrqnc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2juhnpdre.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xiumtuds.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lrfdggrq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hugfnfxh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ejkdpipp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xsxdmjho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ygbmvccg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fhwdhevj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rsonivkj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ditjprbo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jikthspd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fzmehvrt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ttonzxef.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xxiitwjr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxnbaia.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2whvywumy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mbvclpft.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lillpabr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gjvbgvmc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2udhhfbfr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qnpvjnrt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2urfqjbre.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eyfmcpns.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jkgnouoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lfqircav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dpakbcyl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yfwhevko.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjmsmpcm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmrgvwed.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cuccyuky.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ybnprrxh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2iwcrmieq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2shzkonyl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nhetktui.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2txufirwe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ifeuuacl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mkvwnhgv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bqlfyyai.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lxyghxgy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcytube.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pihjstkg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jmilejem.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2njgeoxxl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nuvosywj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2czaxvmaz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zsazaznf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjmwydi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2teyilukz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yhigyure.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zlznrjuh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2olupmffe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2axkagvuf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iztznnak.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kaunqikc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ftrxxfhb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlncyebd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kbnstuck.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2whnswjzz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ljaihvmz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyunblf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2atxdbnjp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gsxmgngi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ywytdcph.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjcmbja.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdddnine.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uhauxvtl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2blewwvbt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jyshisfq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bbjafybk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2glnrxlbr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2igtpnett.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oxoxeptw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tnyapwxm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gavxkgme.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kwhimsjb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mdvjztzc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zlwubmwk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrfpoeyj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2idowwkbj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gxnjvwny.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hioguqxw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2njulwwai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2elcanmbs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ewaqksor.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmgznvxm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ertgflhi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fcygodgf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xmgqxiqe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wxajnrvd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gifzepkc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cjfmpjzf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zwdbuuaw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqektzup.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezibyejc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2geznqfbe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hrzvpyqa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbvtcprw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2crindova.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cmxkdnme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ecanrbtu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rqrowmbe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2txoxvefx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exqqbivh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyqoedlw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ieiushbr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pkaakkfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwpctmhw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wdyktijz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xycthziq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgtrxafo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vcyoqqin.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wrxexxch.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vepdepvh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wfxzhtsi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vhwubyhq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmkyry.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ofvykgok.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2syvdnwhi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rzvqlhlu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obfagqio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dhhydecb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wozhubho.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2keprjjxs.html


<!-- 参考信息 -->