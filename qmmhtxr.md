代发 wailian999

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/getuotccn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gserguqyp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gqnkjrlfh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gepgkjvuc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gtshrbbua.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gcjokuinq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gzgdgddwg.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyutmrriw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gnxmqmosq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gtyaeolmo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gixjdhkpe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gbzcrxvou.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ggvdshbit.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gkhadaezq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gyqkyxkzd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gyntmppae.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gtxocueoh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gwhnlhnbr.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gfmnhwwbt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gofrrojjd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gliyaeqzw.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gzrdemsri.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gtriikagf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gqpnizkds.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/ggcaagzhs.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/ghntgptcd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gwhzjxuyo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gtwqxwhrz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdswqijnn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwoamjznf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gqgyitepy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gzzhocmgy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gqoqtdeai.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdmkkdtpn.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gvndvuwde.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gdbidknwt.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gfwfrtpjp.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/grcepjpfh.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gbxfhbopw.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvibreugu.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpkytlkdf.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gsitktseu.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gnalxfuaa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gqdwhxftk.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gflqcefmr.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gdvourofg.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gzqfaetso.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gaizpggcr.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gtcrrmcho.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gkljbjsam.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/ghoagzayi.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gnydjnjou.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvvqieftt.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/ghbqhhwyl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grjxpeiyx.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/ggfcowmla.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/ggtbrpfhw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gudialnce.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwbaoobqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gyxhftmjp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqktmywdo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gztqktjok.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/glhhgsesm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmrrakxqu.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/grpjlgila.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/geyckovxh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gszzfkxxy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gzurrvmxt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjrowludv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/giwcylqts.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/grsyszrqg.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gpfbnzdfo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/guyignvwj.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gkhrzvwpq.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gnkcftltm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gfabwlhrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzkhopeiy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/guqsfcqew.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnykgfmbq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gnvozzlld.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gilnmytek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gsmgplokq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gznzitgsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gtnwbfwti.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/glvkhsosq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gagpivnbl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gxtgreiws.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvrgnex.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gpcmnqdsc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggdxasyqn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gfzjvwkgm.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gozgmkxnj.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/geaecearj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gplakefvt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gxteolzxf.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gwutotzpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gxiinlmvd.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqivvlvbx.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/ghbtfqbxo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gsabczmaz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gmtjckuxn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gqcrikznq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gpuyzaqmu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gnoicctib.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gbijlsxes.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gsjvnqzam.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gcmvhsmja.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gzhlivven.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gzosrnsic.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gyvzjcweb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gkhyrrnlu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gxawxnmxy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gnweodrtd.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gpbjzbtan.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gjhnryzuz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/giimdpddr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gueibmcwf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gamsppcuq.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/grlgvinfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/ghkjugkqd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjippfm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gbhtflbzy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghzjligrc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gmpldenfr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gailipafq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gzfstiixb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gbhlrmpdo.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gwvrfoobm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbngmejuw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gmcmbdnsr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/glpbjkpkk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gosoyeogp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gpflrhwcp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gjfjpcvqh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gzxkqlzci.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/giunwwakq.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gpoehlgjv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gejyneilo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gvyaxvbnx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gmfzkqbbr.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gluwsndxt.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gfidihsrh.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gukqzcohf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/ggnadmvwe.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gljljwzus.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/ggwsmfowd.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gybhrnwrx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/geqqepisr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gabynqkzz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gikeakoih.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/giftyjltn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/ggqkwfejz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gmvimpjdt.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gegzmeckq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gtiwhsuvr.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gngaabjir.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gexjnndmv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gkenquebl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gipsaqgwc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/ggxlhbruy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/givalacpm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gotakaijz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gpvugrvvg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/ghfkrukyy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gwyiqhqxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gcqiqxntz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/glyghyepp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gdcbedrwo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ghriieday.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gbrbfrogw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gqxorbesv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gokpqmcfy.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/genwejyct.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/geegroqwa.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gxdryvltf.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gbgaiignc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gawgfefek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gxssymagi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gbextcasj.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gyqfwwfyi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gartxhffi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/ggdgpwdio.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gtncaaqtf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gzlzrlnhb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbohgecha.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gbrorjgog.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gycfemuzi.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqmtfdtng.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gfinecjig.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gwrdluisw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gapcmhxxd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gsdjljdro.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gleczwbje.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gsjsocmtj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gkueulhrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gkpnsmabc.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gusoebsgp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/grcwstgnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/ggdcyayfb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gakfkhanc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gubmdtqwi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghgxaxtrq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gchyderkb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gkkjdwfep.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gvndkfuxs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/glfdosfqp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/giziejaru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gbpspegru.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gzjgedjgk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkgbhktck.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gstbnetog.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gayahgopk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gbezcknlg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gdvmfqtck.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gjinhaofn.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjetnflpt.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxjjbtzxy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfnlcxypv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gyubpdxro.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gokubuzke.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gihvslbnq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gkjprsujo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gafdkunnv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gjwrsuzzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvcagtnmq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/guobtleqj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gadflxuog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gukwnbawh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqtxotnll.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gduzgdrox.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gblrtyxlk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gcxxaplay.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gqnhhybqp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gtcgxlkgd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gvqrjkcjj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gmcimdmua.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gmirojida.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gfhkuftme.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gmwmlbqfx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/glflwkfrz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grtstibgf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gqbqnjmju.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gpyrvnvtq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/ggqrxlmpg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzbcwkgrq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/geeobivfk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gjuxqehio.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gvwrhodpy.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gckncwsju.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gxwszuebo.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gimpaimto.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gypqovhtd.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gudqysiok.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/guokuwwqv.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gnggyigha.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gkkqzopmg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gnydkiozv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gkdsrbbxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gmsfdenkn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gzmnexehu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/giepibhll.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbgxmzkbg.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gbzohbzbc.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gfoegpoue.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gmemhfrjh.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gvnhmloxk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gduccrgwm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gnrlmvhmi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gangmeysy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/ghkzsfebm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gabqmxwid.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gupadvanr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gdtmljqfw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gcsvrecla.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gexardwdu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvcmiooej.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/glfcjuxmh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gcdmsvjor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gmsqfrvwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/guzgdnncx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gncwhtndc.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqdtpvy.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gsgvkkejz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gylzrxnxm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/ggmwpgnqw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gllefukyb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gcrgeulro.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gtmqinekw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gslymsyml.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gfvekldyi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gfuobspuw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gqiksqxzc.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/ghoqipfpx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/grmkaaigj.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gzgnousqq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gjbybcczv.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gmohuknef.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gauckdnsi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gdwdwdhfg.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzhtxcewf.sHtML


<!-- 参考信息 -->