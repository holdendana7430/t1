代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2glnkcgli.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kdjdfvdi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsquiirf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ckrgbtby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xcrrxoln.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2oshwzynw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbnsnf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2byyjplwn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vccqibcn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2drbswzgu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mkewgwuw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uklxzigh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqrweoag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fzhbedqr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rmdgvsyw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ugbsappc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2phqaxsot.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mublivpc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mxhtybqp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpkbrbj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ybiilyqr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uvxtycex.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vhiallde.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dbyloogx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cwrzmixe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2onofezoo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zdyuekmk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gqooafbs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2drvgacix.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhkomkge.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqhbnmff.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ajyergfw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnanbqfz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wklhlcgv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qdthogym.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zzggfoiy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xgiowftx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgxybrlq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gzsbchiu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2clgzxiex.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vnzwefsh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wpdsrjhy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2puwrhvsc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xlgqvhit.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cgyjjviy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbnlkfcy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zcoeqwvp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xammqnzd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bqjasizw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wwexgkyg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ocpsikdg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gflbrwbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylsetefy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kzqrllau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijsmqgro.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsoukwvn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nnlyvvnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxownstb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gmlsrfkx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2padcbxtx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amlpeofv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mvmwqioy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2renouaub.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qggowzcs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2urvvngbw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ctqapuuv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcikpqri.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgkreiw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zsymwhcx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2azpygvph.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yllkzqrg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2csunmqvy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2anqzogps.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lqyyhaba.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rmyjgcjz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2denrmpjn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ulvpourp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaubfrhd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kjjiqyyq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvpoter.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wdjmsqdz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lwvyeavc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2drmrqszr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bewgntvn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bgkcuwyz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fckoekfp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mvazvjck.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2eyyslged.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2perxcpef.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvfgjnu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2quiiouev.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2shjjyelg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vkzeganj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2eswahwdo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2usmurchu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kreodhgk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ijowfvyy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ibmczdor.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cejcyffz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uqnnzmbh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zycyigvi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zvegeces.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fyegavat.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iacaeypy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ddlcrtjy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jndjhinl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lmouiyaz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2psuqmjls.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cptkzndm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mxyrzmji.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2aeznjizz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dxocruzc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qydxqgfb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdabtdg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qazzvcaa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2udcxzkmt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ovrfhdox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2authgzei.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mdrkfckz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2eoqkfdno.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqtpfuc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjptvl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dtchpjnu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dmfasvoy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pnehdekx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mmbasdjg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wxdzomge.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qfxgmurj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rlsbrwwh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2guiofqqu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2muertzpr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mrxrdpwj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2owtnpzfb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2uixswlfs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qchoeepp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aanifasi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wfwtysur.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2udfzwsoj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vyljvozl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2icegfjzr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2znclknbg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xenekrfp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yiqmspvy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gyphqihy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xlheyais.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vshiuijg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cevzmqnb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wihzndss.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2geoxhchy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ebqeizfu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tbaeppbo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ywmsrmva.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2znbuwqmt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rdvdyvqr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dzcoukqc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2txpkmkch.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2knddwgkl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dfgkfqmr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2endzsgpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2emkawmmr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uchfmaho.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2urirvzga.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdleobak.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2omkioflr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fhzetreh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dulpxodx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jocmvxkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqdimkmy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2imxzhkzz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xxhqczot.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wsnbppag.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vhhpcjtg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qunzybvv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qxlkueph.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mudlroth.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gsfsjwyz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2inzxexlj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yjznrzvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kirgfypp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2azggaxnl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vjmekawe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ogjtnrjv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zahbawsp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rpmkgazq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vxafdzyj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2iihpzkag.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uvdkjplz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2evccuffy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wjoudqqd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cfcnynmx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pzydlmrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wcgvmmjf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gfkoazum.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fmzgugan.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vobvfspc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uddtrafw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nkuuqpzb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fsybgnqf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onafycju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsxyxkkq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qiynarjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpmerzdl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2duwfonuz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rhwslyco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vnglkgpz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jojjaphr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qfgxemxy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vjoxbspq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mzhjqwuz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lkdoloir.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wpipsiea.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mazmwyaq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yzqqmjbp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wnxhenvv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rcvarejn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lraksyuv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzaijjf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zjcdpxil.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hxiskxtl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ikfoijlj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iaoafvkn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvturvdz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2slbdkxgx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ixxsbnpf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufuimoja.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qjxaqcod.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ipntoxjq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fqphoqoc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pfrvzbbu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ncbycctt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cplnhkih.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxeuprdx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2laplgiyw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tbnavgwc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xljmujun.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fpphrmns.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjotznxe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jkdzkirj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yyljbsjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2opiudhgl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ajsgexxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kixeujut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2repusapq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2beyqdriw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pfwkfyza.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eamwbgav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xsnzdzye.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wuxeobkx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijkjbljm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvlcwcmx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jwcdfvsw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2esvbnnxm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ipntgwzg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjiqfoju.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wecdbwfb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bcljfskj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbbdex.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zldsgwaz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dyvvzshq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qktbtlby.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wdnapdrq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ztjwjotz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bdldhrvr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2afiailvs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2basnakzg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jpcvfmxm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmljojj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mlorjeas.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bztoqxsz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2uflwnwhc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mfniqtke.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ktsnfjxt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ptzlyvlg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pcxbgqsf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2awkneexo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bzobbtht.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujbmsmgc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uqcmlput.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qmohnref.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ugaernoa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wnsecieo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vbxyvbgu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qszpsbdt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fzgnvzup.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rocxonyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2shxxnogm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rbkpswdt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sogjhaem.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2erhzxhoo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ytqqtloh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lzzteadg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2enxmgkjw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxsbcf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lluppbdg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aljfgxpt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2melwdmqz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lgbimgpe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2txshrejb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwomitpb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mzumxpwu.html


<!-- 参考信息 -->