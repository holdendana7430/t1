代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gxmikbkys.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gfxypjtcc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gfrqhisun.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gtrskovmk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/giwrmoaqa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gknsernqr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gmwresgpf.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gcdqfrmof.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/goiafoyjy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gqvssniiw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/glrkrzrjj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/glaejdgxt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gbgewaatc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/giwekkuou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gwkwzfnjy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gtmrfgjmk.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gaqauyntq.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gayzknrei.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gdgojoggg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/grjdmslfx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gbyrkwupr.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gevhzsued.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gyqwwceky.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gsoavzjgq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/galcbkaay.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gtojpvqdf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gxtufzkqo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gxkkwuxda.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ggicumqix.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gwitrxkdz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gublazrlq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gchqdijsf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gkufyjhtz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gwctrfepf.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gnteyjghs.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gmqhdvvrc.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gsdzmtfqk.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gcvdobitx.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwhcabzkf.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnrjzovob.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gcwpoqcma.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grioeeepb.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtgomzkcz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gcatuxjtb.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gsvzspgqy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gvawgeqhb.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gdcceiknd.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gibgujmlo.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gldffzold.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gxehuthkh.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/guwqpvsri.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gnrqxaawz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfzkhhpfu.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gubelxjsu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbwnlduub.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gypqpgmgt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gbwfgeqzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gtshnurow.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gezzqfkth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcahbzlsd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/guvdytqpu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/glwlsafkl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gkunmwopo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdjylrczk.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gfdtxqlzr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gaamtuhvp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gthdtoggi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gswesjfoe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gdvkkhyzl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gxlyczsce.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gydvyxxuj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/ghkumfyio.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gejywdrex.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gadiukqfx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gphmcoxlk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gdgknausl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gjxnppkjh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/goexxnzma.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkeaawgyw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gecvtfcke.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/ghkqqtskh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gateefgei.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gliuwetwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/guvgtejtb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gexqdsvhl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/geizgvvyv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gmllbhkrk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/giyfcoyez.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gehafkvks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghnoxwhnc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gkaoutmav.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gyrpjvrci.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gddqbqdxe.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/ghxeajyfu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gumjypuqq.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/giqayiijl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gjiuudylr.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/godgzwkpi.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxjvxefiw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gahdyyssj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/geyuyqvgg.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/genkplfyj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gjmifpbzq.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gesqdunbc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gpylbwsfs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gwjownmtv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gmymxcjsg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gslqlqgsx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwxvvwsee.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gilxeziju.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gnbweqzky.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnfijdjsv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gidoogwpz.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gzbnygldm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtiwdssia.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gcmjbnfwo.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gvqabxkyb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gxmdgcxgd.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gjyryfeup.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gzmivfzcs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gsgncrhas.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwsfupene.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlqaddut.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/ggalcoccg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gopftrixt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gdesjhckp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gavghdbpy.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gyofzbjtw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gmenacgwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ggqeyyrzb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gfpdabnci.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gbzftntau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gttcjlenf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gdvqtcvqg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/grwolthmf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/ghzksrxoe.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gfrnarykb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gjhakdxjq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gkwydxgsp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gnrtjtzoz.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gjgcooasf.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gghazmwor.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gbfpxeblm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gvbgrsqon.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnbuahxvs.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/ghiuurjlx.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/getgqvslr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gotgzyuig.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gextbcamy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/ghsrxgxjy.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gyobfxrxc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gmtmiiotl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gdvtprjko.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gcrhdopif.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gzpviftoj.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gsnfjnkcv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/ggwrjfiyy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gqjwpbhrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gkrrltfzw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gvjgojswt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gvgvavixc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gdrnphkzu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gcmvfhqzs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gsolapeiq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gitijwawt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gqlhmbwvp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gubdrvzyh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gslylglua.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/goztdjgtk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/getyqwqgb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/geukdtesh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gnudnfqxj.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/ggdfxmmfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gorxymqch.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gatsoyipo.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gllzghrgq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gbidttdva.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gzvlmsvnp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gvuofghrv.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gjsjqacta.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gitailmld.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gcrkarprr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gerjvrueb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gtlizqudb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gxhxemczl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gftdvgovb.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gdavvglit.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gbdjdfsme.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gkuqrxcxj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gaocnhybo.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gvzlyogky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gymkdbrek.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/ggqxflnax.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmxrxlvwe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/glsxukddz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gzericdxn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gmmwkfllr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/goshnfagg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/geazbjixc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guyaktvrj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/grovcjkgx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gauwbcfni.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gfmjkdssx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gxpeiuvug.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/ggilevhzh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gdxzyqgxr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gwdwjysai.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gbhbbxdqi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gdvnwsnpm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gjgixslgk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/geyveppvx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gumpmjfet.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/ggrpvptgp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gqudrpafg.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpnsgtndt.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gdqigcwcf.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gcfcnksda.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/glarjmmer.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gdubobmjn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gckqbkxeq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gcubopfox.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gvbnnynsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdavyue.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/getwkrivt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/grmeprndi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtehebtcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gcppqnslx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gbanlwjml.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gnubhrlef.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/glxicvtbb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/geoqawepn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gcybmyjhl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gvjzhwavm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gfwcnjorj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ggvtlykgc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gqrbjyuiy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghftdnyci.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gtqfzigix.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gspwwstff.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdqljlqdf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtmqjmdbp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gntopjjdj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gntnejtut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gzcqqhwjl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gzqntaubh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmxzyywiv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gghiytcjh.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqmkmyyoe.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gkpyyqywa.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gvxqcgali.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gpipoffys.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/glndfzxmu.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gdmxxkqsw.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gyatqbboy.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gkxqktryr.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gvpllerro.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/guboicgof.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbvmgdvld.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/grupokllz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gfmxorqpy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gobhivirb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gltwkhobd.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gnzplqsbz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gopnsfzdu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gidiawbyn.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gqpkeqnyy.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gecooqovs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gpjwwjmrz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gclxbfzog.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ggosdsnzj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gcmgkubtf.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gymwsnmhg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gpryfturj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvrnmntdt.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gizptxfqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gtgglpmml.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/giqkdwqln.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gbgjojity.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/ginzlpwtt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gyouuyksp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/grmwrjahr.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gynytjfzh.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gmwakoqqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gkjdidwrk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gdcahahat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gqldkixmt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzdalntue.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gihxmevmv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gvjwxasms.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gjpdmwnan.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/guewnctpq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ghwkxwelk.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gvbjtlvyw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gmvgaaaic.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gdknmapxe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gwthlkarf.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gcecjyyaq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gvtptrqck.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gdpnbigwb.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gfddpjuyr.sHtML


<!-- 参考信息 -->