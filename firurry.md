代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/glrkocdpb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/ghexmdzca.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/ggesoyjes.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ggiftxqop.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gtmfcqeco.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/grhrunteb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdxaddqpp.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gqmdclhsz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gwnzanpeu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gjwjivpqw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghlgnbyga.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqmgsarhu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfpjmvhoo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gnxmhemcc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gdtebkbdw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gqdbqsksf.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtoyioerx.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gaccvlifu.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gqtgfgiuc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gvjcoazzj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gklivkteu.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gmyksqbhg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gwlnehmzq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/golonnbmj.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/ghfvfrmha.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gmljxejop.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gtisnkasr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/ghznhkwpt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdowrmnzm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gvagqibdk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/glygyrrpr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gzvoitidm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbtnsqoth.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gapxysgoc.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gfoduipip.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gbnuchcbs.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/ghqsfucpx.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gwideemjh.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/glffsdknu.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gldtoazbv.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjlbdpift.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqtydqxkr.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/goaxbjevh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gsfymxgio.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gdqqyogtz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gwyehissw.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gszsaarmo.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gpjjfyxtx.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gxsrtejvk.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gsqzvbljq.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gcpofjfkb.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gdsbrjjzn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goyunkygf.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gmkhratca.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gapihovkb.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gnzpfkzvl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gobmyyhby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gspkqsvap.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gmqjylkbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geoklzcdh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghmaulcwh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gadmyfzny.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gqjwbzgqu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtbrpkcsl.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gkwhzfnva.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gsgrpophi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gfwxshimz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbqbjzhuz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ghyalikpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gknbflkud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gdqukbadi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gjnveudku.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gszbdlxei.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gudrolvve.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gafoiajtn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gynnrrbjr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gscvcpnoz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gbypsvmzk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gjcgppbpu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gkjpkmyot.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gadxnlpjq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gkjoygtml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/ggnzwvrjl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gnllxkahk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gpycuzmpx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gfdmspyms.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/grjvbmvif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gdgaclgzb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gfrwzeglk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdseelzzf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtglfkwjk.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gkeyjojnc.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/ggpcwknib.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gnuymvics.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gsltkfmio.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gmkzssqwn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gijotebcp.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gmfixopfa.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gsngtvdme.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gsikubpad.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcxaqlxvs.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gyblkjknu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gohyhlzne.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gqukvcbix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gabqvzwfu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gebuwksvy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/grhdufgik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gzzuukyzm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gsrqbiglf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gncenipes.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gjxuxyvcq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gcpxslzcz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gdfqxbitc.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gyjzwiqkc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gozjdwugo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gqdagoyez.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gdkmdbcfx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gsyqngevl.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gjfmhqjay.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gqmftrevr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/ggckqwkpg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtkgvdzfk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjetykohy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gwktkvmpd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gvarurvbj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gntthhygz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grmxewzrh.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gcxwfnwoj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/geyysftul.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/giotnwjbg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gcxultyto.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gszsifhvn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gwdufxxqx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwyfoqm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfptubdt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/giqubuhsw.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/goztaihwm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gdxuqpoez.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/ghyhcdpjs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gnotbxdmm.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gtrlxdjbs.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gxvbuuvmi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/giuiqsebk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gqhntiacu.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gyyrgnoew.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gpypacqki.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gdcbwlwuh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gurjifpsi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gozhzbiub.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/getuttlvy.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/grdvxxvmv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gguenewgd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gchuafplx.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gwsajgtnt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/grwgfrzce.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/ggzixzrnu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gywniwblc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/ghfxarcfd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gajggyzut.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gxfrzdllx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gtcogifqo.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gsornwimr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gausvenqh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gzqhoqumt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gatejbluh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvehasksk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gawxqvnew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/glyegkoxv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxrkbyfqe.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gzvqcrasp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/ggkgorcaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gcyjhgbda.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gyjdxjkdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gnvmlwobx.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnlxuspxp.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/guucwsmrm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gxokrucno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gvxhfpbsy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuyxxwxo.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gypffybdg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gnaqozufq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/groonowcm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gdrequdrv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gjlgvqtqj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gdohkquat.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gahhwarct.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gvhxlvwig.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gblcpganh.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gelpixuiz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gwylwynpm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gpzagtupf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gxihyznap.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/geuwgrtbl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gtdqxcrlf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/glthsdkzi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gbjywvrnd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gsnizymyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gaamjopwi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gpvjeikka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpksthroi.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gvbsgjcia.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpsoeeprb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/geqvjmzat.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gxvkfrokx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gpgukrark.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gshpefgji.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gccqqlegc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gjkiibhpr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gouukcccf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/geuhuolkb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gnoaaiiol.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gwppvlipp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gemdwnpsh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gyjyzfzzh.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gqolnrjbr.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gwxhiiybk.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpqgrmuws.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gexhtwwpa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gdyacopvd.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gxjzyfpqf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gdnornnns.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtlsccaaj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gyedyjqzu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gkirtcxjz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gycuoxbrh.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtjessdmt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gquwcqkup.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gsvduistk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/ghsnbasuu.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gvugyeexz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gxkgpsfbi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/glhqppuhd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gcjmkwvep.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gpathysxj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/glmrmwolk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvttdxdyi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/glqjnskar.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gcjnqiunf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/ggwniwneo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/griylizzn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/geiikchmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ghehykbmo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/grwplprfi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gjmhypuaw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gxdmhaokw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gudqoufei.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwmiyjwqc.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gzbhisnmd.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gacozrkdk.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggbuipual.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gmrcgipjl.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gngwdgdrx.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gggvgixzp.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggbmklnkg.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gubumhnmh.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gggmtjtvz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gfosouiwq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/goxtsvxaz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gwxazposb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfnrisxrv.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtpsvfbyh.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqjpabmqd.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/grzvoyjnw.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gbxrvcgqv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gzrutcqtm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gniytzwma.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gpispilpl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gfaqnizpo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/ggvdhxuyz.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gbwfmyrxi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gchnhfcju.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/ggoarpjlj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/ghowkvldu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyzohsjej.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gcydxkwkz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gavmhlort.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gxjebzhht.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/ggbzihtal.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gifoblpra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gpgyjkbah.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gyznjjcqb.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnbitsatn.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gtpephbap.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gnouvywpl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwkgnnyok.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gzblgjfuc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gqcptmvjh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpobfwwwg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gqzjeaglj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/ghojwwpni.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ggzxcsvhc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gxdtfjkfr.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gyzeqaflf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/ggfoogwzo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gessujdeu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gypspalvv.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggwelzjnu.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gupisiksd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gzgdwqurz.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gmxqelfas.sHtML


<!-- 参考信息 -->