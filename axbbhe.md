代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xgrrousp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2obwadwri.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nozfqmog.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nujjvcst.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hpijdmae.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cjnykmiy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2grahiexm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oaswhfki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyqnoklt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xheynvsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uczgqanb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2exskiwfl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pxdnfbxu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sthfxdix.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwuqmqeq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdemduth.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ifvmimyk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngpxwpgk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2acrpygdo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hztxxufr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yiblwdcz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yniifnkd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wueybblo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoapzcsb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqftzggq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jxeslndl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zqaygykf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2csulbois.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ylpjuzos.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2eggocuxg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hzahbcth.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2aagngkqo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fnaobsyo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cucowupq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2topeyxdt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwfksxo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2iocrdupw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ovhxegeu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ojncuvki.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnpwlbf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrbesvjm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cherticv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ngbnshki.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2prthirzb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkhaixsm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzzowhn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yxgycpbl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xwoqsljv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rxoegewx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2awmrysbk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ymszhnvq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tkfzyaex.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cwysdwws.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2efxuqygm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lmwskfkz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pkhdhvjt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yjekrgxx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wskehueq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqmndfl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uclphibi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2icwriyxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2aslwnkgn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cilxusgy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ovrhqall.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xfjrvxoc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wnvqidfq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qgixnqkb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wbwbktmn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbrniqq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gxblvhte.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ubccdldk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hhhdpcxl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gilipvck.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fdtlitpj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jlexnwfs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fdzsecxp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbbsybr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrevfwx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieppltqs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ygtifwem.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zekmyybg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gzipxref.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gkcgugrk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2aadfyqnf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rgcssmrq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmfyaaak.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pcwabdle.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vrtzymam.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fsplmbsn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yycmoaxv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anziiujp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xpvpnwtm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qdxsspex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqqdvf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fmxbamlf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nogpxqzy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uostcwkp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hlmfyfou.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iofwjyqy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vxcnzuvm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mtatlauy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2esjfpmlc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2stytaaap.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xxcaoasx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iaevfryt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jbtymwkb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2oynreuyy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tvtwxbih.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hpuajfpw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jifbzqqg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2luhklzlq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sgmxervx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jyizcykm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iudpmahd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rvrtoish.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2brxmnicz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hnmzzhzn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lddrylnq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ikddwfsm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bqglvxds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2aupqsmjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gbjvnbhu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sldxwqxr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dkfrdpwf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbptgpc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lxzizilq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ydgiizsr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xggichju.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2enqfaehb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gootnfxf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2llsjvmcv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hvgxztoe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tlxkjhpe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2msqfaaab.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wmraanku.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2twelcbuc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gealdecs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfxmzgvf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xeyfrrbd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tdqmoxhu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dbugbjhj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slczjmmk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iobbcqio.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lqhjrugn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2meqvbsnj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lozzqbld.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cqcpxsdy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lebbksat.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2upbxkihj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vbjjwtsz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2camzflnb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cysmjufv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2axnrexfi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qkrfehnw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2myottdkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcqklhyb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sactmwnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjhnwqmz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qeczdlwu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cinaybmj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tycswkdt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mkrrilov.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2udfxomyi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qznglkee.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ibfxygnd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2krltytqr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sczyvldl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ganurxmd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mgipoygr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dxsnkfhi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtwhnneo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ipcveapk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cryoexms.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2poghdlgk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fzdnlukv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qhsyydjv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2usgjzwhm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2maytrufn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tdotthan.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wmrqontk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oxazlvzd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2quunvycu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fptfqquk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cqzeuhzr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2soahanle.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fndkvlph.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cuhkdzac.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqvdcjdt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cgezgcrg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zdjacqrx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgumuadd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cotocptq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dpefzqlp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vevzsuet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xpdcqqjy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kciibbtl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2guliqqxv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pqxgpjdc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xrecfyam.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xxuxnqyz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pamnliyy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kyqkeznu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yohucifl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vzttcnhw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnimotfv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2teceaixq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ddzpaxrt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdlovajr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwdhui.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpwloaif.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2otbjqkea.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gykoqasg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fdizbszu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pnpsztrz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yrrgzorq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pseiuite.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwhczubx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dssqkgjs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ejqyltdk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pxmwdxdn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pnrigcvn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfkqafqf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tnojdasl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wqizelpv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zxedywex.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zxusekcv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bbyqecyh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxvzkek.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2holnsspf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjdpilw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kqdpnwki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wfdcdtpv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxdjgdyq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jubwoakp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bvgoznpy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tehnddjv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tdicsmyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vqgprngl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ghnewmen.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nsdjrykz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xajjosnx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tiznqgkm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xzetbcps.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ryplzkuw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yvmkizwj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uybhqpcf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tgbpfmql.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2irgdzznv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wramaamv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kfwgzjee.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrpprtqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2usojxbkb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ibrxgbqb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zwrysuwu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2iumswnze.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bghqgcek.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tljqdwwx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gpkwvxuw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bxlciwvv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhxgxczy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vjpcajqw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjssuxso.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pvybepqd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2twcuwpnv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rvkhtuyh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vbetrtny.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pponeuku.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2flguibuk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2iajjodok.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2stygmkwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvzwjid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgqeugb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yinyvngu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhxxgli.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojdkuuab.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jevfffhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2goibzhin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2souhxybt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyslhfm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2usddqflx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2exajbzut.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzjqdlzg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xpctyxnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oohgnmrq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2igjhskez.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ctwiupot.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfotunjv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2liruhwwn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lkotozcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qaxhyxjy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2amqppynm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2smkeidhb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ofpcpkno.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2thmzyusb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cyfbmeaq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sjfhrdkk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbihwoa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ydadqvuq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2smouodct.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jnxgqjcr.html


<!-- 参考信息 -->