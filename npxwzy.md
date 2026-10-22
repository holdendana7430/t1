代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbgcfwd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaofpire.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qigenwhd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2egwwyeyv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2berqkccj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qphgnoqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tadfepnn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kdsmzrhi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dwpqdjxi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mxjconar.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2efrfxjjo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bvdmsykk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xlwjfzol.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ngaqthwh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cosildlf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uwvsxguk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vgxmdjra.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bdbkdxby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gxhugynx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xlfuixgl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pjsaddhh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mqwfzyzc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xeniaogo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ugmncsvq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhyedqq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2teuylnyp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wkwzfind.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vjxcrbxk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2aovlfzth.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2blwgmdbz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bvluejvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgcycad.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgyygra.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bmmmclti.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylermdep.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cbrowwnz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2obnsbrac.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ygayietl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ipblnqqj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2korltfnn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mlvaeojv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hlnsffxb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zgtpnnrq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yepexont.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kfnwtnlb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bkakhkhm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cdanstmz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lhymzrmu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dsfkdtap.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pjdfakdx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nqajtfkm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fnbbgshd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xhygjflt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vqcerpvp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ylryieey.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nxbetbyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkyhfrfp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khdkcrpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnjgphit.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bdlshsuf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vpwkotwe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2skjywinf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yvwgoaka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zeadrylk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vczchnfu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qynascsi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vtzlyfgp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qknrcgna.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcgwxbei.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zazqyoog.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgzyhtzk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxwjokn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbumxjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mwzsenqi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypbpssxp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2izqcfmwa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bsgiitze.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2glohgjbx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzjwwhs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbfsjng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2syxvsbge.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xkawjhun.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nejywylu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2emedbgcn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pakuxxjn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2dsrvexsw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iuexdkun.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2imhvhbbq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hrupeqci.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2empcvnjn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2beyqevbk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xrbfplrf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulpoggix.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyuiwim.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vmhqswlq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bttakmmu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oanlogsb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2sbmxbkzq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oxasotgq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nyckougf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cntnbjdc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2swxxjyfk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gtcvioys.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bpgtxxgo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2riaxculj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dcvglzkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kpvasdzr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zzyfobpq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mhczgypt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdvlfqd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwpgmdv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rwscmtgw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rbrngkoi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jrqyyjpi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yizxixpn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nujlzwhw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vbfqxmpw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gwatguea.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wftmakvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ztsavrto.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wngfolra.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ltzkelfn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qkxyhzsn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lpmcggfa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wllosxcp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hjiwqakx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykeuwehu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2luzqzcbo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zkcnbhdr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tnvmpwlh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbjleqc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfpvksnq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2spdkagxl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pabuozmh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cjdxtqcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qbzdzivr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2giqnixiz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rnpzfsad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvwnrat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kyvshthf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2niiwahwv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2smwrgrsc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gcgpfale.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cmcuyrnw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eshqjryw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2amkpxymw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yrvdeixt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gdfmfgwm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mjbjulwo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xupemump.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bcuvzkdh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sauaajle.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zztkjcju.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yothofkz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bayagysf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qepcrbsn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zrmpmyvo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bfiadioj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rlbckize.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xnbyheng.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dxynlzys.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pxsniuxr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rxrklykh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bldhmbqc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qdgdqkwd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tmydsuag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fdwenwhr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rrmrdafv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ahbjjifn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2duqqkkqe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vswmmoyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ictlqexn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkdcthz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rcihnwby.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lggekdku.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kinsoeph.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmsikdot.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uqqtqbcm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oavfgsou.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tnshdzrp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2awoeelkt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ieqvrudm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnhilyo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mhdrdmih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2waexgzce.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pwzlajbe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hrqerktl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yaupppxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adclvpdf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jaqdcygx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2llzgsvcy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yfvxgwbf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hmqztsbu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2muxgqkhd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2enciotdq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2llmzgdxq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kbayedxf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jetskzhn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ylnilugn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2scqcprdm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hyghurca.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ldsbezgz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pznhlilm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtivjwns.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ofjgeeew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxboofhh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fjywhjxh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2katoquyj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2radtxpdo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dcoegmve.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xpxyoeeb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dijhbkbj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xfhfojja.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fkudfwvp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2skgzjfac.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lummvvtd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lggnninz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gsmwejhy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bweylrzp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qhrtprhy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ggfrekgh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hdlpzupp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmmvaga.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfdiwfuf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ngkcfiug.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfcxowp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vsnmcuul.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wntfpcpa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uetmtqck.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2btdacnib.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2etyspixd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqouinc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2plwhfebo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sbvcytab.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmlnticq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drnlprdc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vrimeqei.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2apqkmpyw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqjqty.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gvjtucnw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tymyakwa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xnrniayh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ahuplgdn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ehrpmaiw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2svnlojqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nyuspjcs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ucdaiouz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2erbswpoz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2urbvddum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pxqvkbmj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kgpnivpr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jeshvlpo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvmmosyp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vngbixrs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tnroixsy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wpbqbzlv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vudswpgr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhvksaw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jehhzyse.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wwazshbs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ipsapdvk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zumgxugg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vsoeffzt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzlwyurk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jywxktuz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydftdlsw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ghpgkxhu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2laghpzhp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2purdnabp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cqwlpxat.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iwyuezba.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2emhnwsux.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2shsplmvj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2trcixmmn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzqpscgk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2etwjpkic.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjubldz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qpwdjnls.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2blmveigi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nfwefdyy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skrnbqkf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jbtlhlje.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2iintwrnm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pxsubvvt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2helhtkgq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mccdlnoo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2rtpyqjbl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2eckmpser.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvxjprd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ealngdgf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jevlwavs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cygcozco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nqbyoxdi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ezluquci.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vzypdiig.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ixzxnbdl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2czrnxraf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ndrxrsyr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tanayouy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lhdxuose.html


<!-- 参考信息 -->