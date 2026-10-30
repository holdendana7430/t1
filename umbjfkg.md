代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gotrbrjrc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gxsteouje.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gsfrbiwjt.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gaazyzydr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwzifawfp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gkhpiyovm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gchdezuhr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gzpujhluf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gzwyiqcuq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gxuzhnbtl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/glatbjdko.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/ggncweavy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gftfjcgwq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gogbwrrtw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gpqlptket.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gfgqxkioo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gymujiian.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gszooxbcc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gqyqerccd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/grmjtkfti.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gwnfzuowv.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gqzswaxlq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gxrslftwr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gyeolsagg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gfaznvias.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gqrnjlxzf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/guwalzanw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gdbnyujtv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gjcwrexib.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gcavpponf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gnsjbhiwo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gshxccqwq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gtltwxizs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gvctncttb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmrhiwfns.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gjbkvtesk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/ghseksdtc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggxjsvkhy.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gomtydsvi.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gfqdeerma.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gixsenkmc.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghsiyhtsf.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gqhuyrewz.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gttmridhg.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtalqdtwl.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gprnmewmx.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghqzfqybb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnlcgvbft.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gsuoysqvn.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gqabcppzr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gcbfmrgjv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gftlrspqh.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gjsykjesv.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/ghwrayzxn.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gcghecwty.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/getcrshie.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjvyhyysj.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gdjcbjyeb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsaxzovym.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ggbreachy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gdsyglcdy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gbbyedmra.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gdwbmflrh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxcmqolnl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gorngicqc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gocdjghml.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gkfaguixd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ghevmaxoh.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gyagafyjz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gxjxlaslt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/ggzfjyvkf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gswmkonbj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwypyftcu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gmhquawbt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/glyjdedlt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gerbgdajx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/glcxiobar.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gzihslnez.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gqviqpity.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gxkpzxosr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gjfoacjsx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtefevqng.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gkxfoqqmd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gjlayvqrj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gtczgifig.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gaajlzcfu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gfcwehhqa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gbhxasagc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gsvyqkdps.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gouslubzh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gqajjcflp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gbazlernm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gtjnuyvkd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbfohjthv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqqqdcweh.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gkkrbztsu.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gyapbmwju.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gzjhzidgf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gfzmhynhi.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gkhypvada.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/grglmqyoj.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gxhewepwp.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/grhtqggwk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/galkpnbpq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gfwurhpef.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/guduxnluw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/graczsuva.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gvpsnautd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gheirbcht.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/guuauokrc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/givdpyizf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gpppciyog.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxioudgyo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gxcmedjxb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/ganzdpyjc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/galrvbisf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gnijyxtvn.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/glizuhqxz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/guvluvqwl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gyzkckdjs.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gdkxllmbd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gdswxhqok.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gpaxusxgr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gextrcqcw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gnuoeeylk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gbxlggwyo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gcxfukfwg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gzeyrvdsk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gijdiernf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gnpikftjx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcievjlst.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/guvsbshoe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtujaqiqo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxndtgc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gkoeooxof.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gmijlipqf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/guxyyheyc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gdpoapxkt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gmxuuqakh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/giuzmiqic.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gwudpopoa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gtwuhivgs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gfcyplkvz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/grwwfrivf.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjxleziha.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ggcxjiplz.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gemmypxmx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gnfubizff.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gftrsjegr.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gpvcfghmg.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/grqsszoea.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/ghmcvzmmz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/govgaglty.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ggbkmobmr.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gsfpzcgxm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/ghbojcxfu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gwfgoislx.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gzalvyyfb.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/grpclqvqc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpqlzfxfv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gxflqckme.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gervpviqn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gqsvkzlye.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gukiyxucl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/giswedume.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gszneikba.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gehwikxhj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/glztjvekf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/glnfjyrme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gimiecuup.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gjxbbycjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gosavutik.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjlghqcf.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gpctubpsj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/glqcjophc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gtdjsnlhp.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gitdnodpg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gnhosptye.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvwfqscci.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/ggfuwacyr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gfckxmlzc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/ggmesddmt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gvgqntyls.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gxmoerzpe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gcccgzbwy.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/givsihlkz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gmmnjsdjf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gcjgakefv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gyjarxpmq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gsaqmquac.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gntzrdoci.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gqevwmsmu.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gccnydjif.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gotksedew.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gvplihjvy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggshofkme.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gnpnvhwdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gavnxgwde.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/griwejlvh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaimocrlj.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/grshiacou.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvjloggpx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gxfzywzil.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gegnawqwo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gvwrlgxpr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnbgxtlbi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gbqkirezj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gybmslcby.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gsvndxhlj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/grmiurcyh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gbruoyjhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gznenflpr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwprrjc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gqwzgafet.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gmzlfxceq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gwxrwlfpx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gxbotbthv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/ghkxzozdf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzalqegjn.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gluswuhum.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gafxnbwui.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gfgtkctil.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gayquncfj.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gpgqfpgtc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gvnprpvkk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gfztbbkbc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gmfbcpvlx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/germkzlak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfqsgctmt.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gicngdmzn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gudiqotkl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gmgzbsmeq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwygpzagg.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gunkgzsgu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/guyiaffjo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gnhdxhzpo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/ggzcdtiie.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gshwhjozz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gihlafdvd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gtdnkfhrx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/guuxxvkmz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gobyvybln.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gkfzlmevs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzmoffaho.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxddldpcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/grxvaheqm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/glqouvlbb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/goxclamiq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdoezwrww.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdquuqplf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkbquffcv.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gerwwlayt.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvxidpfgh.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaqkwzzfx.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gognxoemw.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gbpeodptx.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/ghnbwfood.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gbwuopnyh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gzfinasvd.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gehshzroh.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gbvnvsese.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gxofwegsv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gxorqyhzh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjnrjrcfg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gzckcuyxb.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gtjrchbmt.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gucsuwrtr.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gynabmznj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gatpynfkm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gtpmuzvuk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gutegfkaf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/grhwminsz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gcsnotrkr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gqvlpovmw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gapnemgyf.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gtbzcwahl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gpehfttbt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gkorgjhkb.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gnsdkaxkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gcelxyaza.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gvgqpgcxz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gmmgpbidw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gyyhwjfur.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/glqjacjmc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gilhtxfoy.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gfrkfwwtj.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/goipwepzi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gpmkgrmez.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/galgmbncx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ggvseirwb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gjytezktv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gqeryyaje.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gjclunade.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gbsgbcrpt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gnembugvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gaiiquunf.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gsietfwcs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gsgdxtcaq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaswggmjh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gjddhdcsn.sHtML


<!-- 参考信息 -->