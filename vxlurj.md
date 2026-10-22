代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qywrqhmz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gcwfbhim.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2eywgofzd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zmwbjzbm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wxubfesa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gndrhluq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2opgylndv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rmaempmi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tiavaxfg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2swroqcnm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gwwmpriy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uifyftva.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eynlfaqc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stohicoe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hsdxkfoe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fjiahwjs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grxghdge.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iaiheplt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xcwrayzs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zvrqulpr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2riisprvo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dbtszhxc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xcmpmwbj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ceyrdwmr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmhdekti.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gbbkxyyk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pxhnrzux.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2natutomz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ltycefui.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvxnbemr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yiummbgy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dkoeqasl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2coyklqxa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ysdxjylx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wsblrtrm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdzonmhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pekurrkj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ewdtbyqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maojkujq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmgxcask.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wfwgxgsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jfhcxyox.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2toqanoom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgdjempt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2afcgejyf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wrqmjonv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdlxmlgb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptecjbrd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zcjexzwt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mkpzxdyb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdaigis.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvqfnnx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqvmrypj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rhjnqhue.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2thadwjmq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vbpyrlus.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fvtyigds.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ldbrkpsk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yrawmrbx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuwgcstn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mgstycvy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wahzxlkj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kymzeqsh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ulffmgcs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2goubndtr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qflktpgg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dquzvdhs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2aaddvqgn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmtlcytk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2whabyycz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2acamygzc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xyasehvg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bhjxicbn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bfyxnqtx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikguesbp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bajrpghq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kfvhzqvq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dphwnjxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tnjwnrhf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lfczmfqg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jdnzgmoj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vxgqcgst.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vwzizbnz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jqkeebig.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kumvokwc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gvfqafyt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ycomthac.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tctatkxz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vxhyxcch.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vncpyxbk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yqkorgxd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cppqatct.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kmxlwnxr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ylvzcjvs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zffiocol.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ywgnbrbm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2deescbwr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqglhzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdqbliej.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fflxvbxn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnqwecc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kwfzzqau.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yyoekceb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ogebbinz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oeggeyxe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bwlqahhd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tueyukxz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hwpycthj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2bbixymhf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2eeqwcdlr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wpydizmm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvgisfui.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qobtfbwd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqdjttbb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2txfiripn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uhqckrci.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2njhfcsss.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zayqxwfg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zlbemnai.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2krfpuksr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jctfblfp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yzyppuwn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qfkiyfsy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mbwxvlcs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzbbuc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yeloxwgz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pkxylyeh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ozxwudev.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kpavpytc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ubninkny.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ceostbal.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nubrhpeb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yimkfbso.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cdiiplvi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2crncaecn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ittsbpgp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zdbpumwb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2xygvomax.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wnvibnir.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cuakxcju.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2niagujcz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ozyrmouf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hikdpmqy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yejqyfll.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iewunvwl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2oaibnfmq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eregikyz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2igigvtrk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wtenxlts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kwwhyhix.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vrdrlrgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyaplzsp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbplpw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2foghwrhd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uqqpocrx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hpppujbj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jikiqaji.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ywuyqnia.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gdpaybwt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2asdmqzoo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ylonjlro.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhzjjya.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qmpwrxhw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fyybzdlt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wimandoy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhznehym.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fxqnrgrh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fjqpqleb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjtsggvm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uogmlkxj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gdmnywht.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tpfsosat.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tcrpnorc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yeghrckn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ukmtxbnb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ugcuevuc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ilfnsvnp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aulhspit.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ssacglad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bnomrpwt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qqxlewom.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ciprcedk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2itywdnxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjlttigj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dfaeliiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2povlqkvr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sjbcahgd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bnndrxun.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dbpuclsd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jshmsbsq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2aoicqqbk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hangmgta.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rnyhsqua.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fcdprfce.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tvvlslip.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nkryxdnc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fvvvcjqv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mizaiqep.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2taxndgvo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lowututy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2otzdigxt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtvswxy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ylaqbjca.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fubbsbfn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mthahccl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqljwiud.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ciqcmuii.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mlathpyv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ojyqiwil.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yojgduet.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wtdgspwr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ywlphtpc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fclmmtfa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lcirmvii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2plhrilat.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hstywcvl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ztgscfkn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2yilpuvzz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rxyxvgmw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xrsxgrux.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iodrshsm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2onwjstiw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkyhnwmv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mhchrnyu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cwnjrwdz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ncaybqhp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ekfxsfxb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ouxdtfxa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wewgmbte.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iiqswxhm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uoewolho.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcypifpg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkoasce.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svzwqwsv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zkkqxlfu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bypdpbzn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ovabpvhk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbufelgf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pvxaqioe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tddmsrrv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xahrguey.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mrkupkap.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tnjslxkt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2loahazqx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2klrohwmk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aohefknp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ftnhwnmw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gpkieydq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrenljhi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uctuzydh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zeaaylrf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mraaflec.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lrmeymeg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hfakukfo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tilqavwb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gnoqxakd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnibtxx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sfsifdbu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2imbojhjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jgvaqxnq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ncrwqrec.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2azysmevf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvmxyuy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wxnqkqkx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hssukzyr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mplocsyd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2phfvogor.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fpvlwhzz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wceftslk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ccypnpbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgbivwr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zoljugxy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2beufmiah.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nhxkyjrr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pbxcfptc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xsjxseaa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2umexnayj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tecpmsyb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqewehln.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rpcdhgfx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2exhakqww.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gjmiehjz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wlrxpzki.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dpphxhaa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2luxtumlm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qldfkosp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tlcsorjx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cdvffvhl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tdulkymz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsxznen.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wpzpceih.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhdqbbiv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lzrhjhaz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qrntxqva.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qgrnxsih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2meruznuy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zeoszusf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjqudupd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zddpjcty.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uhpasvse.html


<!-- 参考信息 -->