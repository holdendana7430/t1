代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gfjpznzhx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/ghuwtdmeb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gvrppvrhr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gthsjqroe.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/ggdjytbci.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gbhvukxhx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gngirsmdy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gvtipnpgw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gdrykbwrd.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gqysciwer.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/giehumdyq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gqzcgowcx.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gfqnewtrv.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gckliizgq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gupzffazx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gkpwrviyg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gfngrtkbl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gjhfqkrao.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnqmqhqeq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/glbjvazwi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzqjfttoh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdrmujyud.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gwdkyokol.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/goictxypt.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gyerhzxwh.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqncnotvd.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwlviggit.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glnfhjfoj.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwmsseouv.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmjxqucqo.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/geaegktkq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gcrivyaln.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gfkbkbakx.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gukjdizcn.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gvemyayhy.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ggnllsxmv.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gnyvtutnc.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gclevoyhy.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gfrtjmkvq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpjaskmix.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpobkejdo.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gfhtrvdhu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gisybdcyz.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gpgtjrgfw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gvgltzgfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gdddqtnsd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/giahvpynw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnmuezrtc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvfpgveke.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/giapxxhva.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gkebwmeyq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxfhajzso.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/glemcbchj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/grucfxapw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gguwuvgcy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/glvvdkitz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gqjitmpvb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gbkqntixi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gybmqraju.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gqofkrtyr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gxmsahgrl.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gcdqtddkq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/glphsdsbn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gchyrqngu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ghjyzxcat.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gouwnyerb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/grayekmxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gweuklvly.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gpmbubvvc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gqnxrwfnp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gioujgoch.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gmxyvopon.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gmstwncyp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/glfnxbpqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gsayfdnew.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gbkcrozhr.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gesxdpvwl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfdbqihzo.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/ggvmgrpqs.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/ggkkknnvz.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gldzzsfow.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gkdjdouxj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/grfwwjejb.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gafsohoxy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gwdumuenx.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/ghprdeqoo.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gecavqwqw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gzbgrmvpw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gdsjttosk.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gxfvshjha.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gqajwqdaw.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggdmhovkr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gpsuvfqbm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/goynctzch.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/ghonkcdrx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/glxpbjwgr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gecukjalg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gpuakpmdh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpcllqkf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gabpfmqsu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gkkkufeie.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gvnuuzzuo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gmxwqlhta.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gxlofjsbi.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gjpjkgdvp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gzrzdmrwh.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gzluhuuvc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gpvgovlyt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/grbdbjngu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmlzpafns.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gufdpktcv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gqgjzcwur.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gncsrfgaj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gxpwvrdru.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gsupyqfum.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/grmlzmlir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpxlranru.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ghfklyyrz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gydxlgjvh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gghacrslq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gqgqcuzrk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gnoiciwjx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjwgufqbv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gngtbkjki.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gqkzbzxtx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gfnigupid.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gxzupkkvt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gcfoxivnr.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gtfdxufnz.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gilzqrdvw.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gjkzowcmq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gesrpzshk.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/glcspczwl.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/glpeudzwn.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gttrrpqgc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gfdwztimh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gtluftujf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gzewjosgj.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gixhsmgsc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gbwixakkg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/ghihlxfeh.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gzeywgoup.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/ghsdbpydf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gstokqcom.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gqbebviio.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/grwxvnmqy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gcesulnbu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/guvfsnuxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gytugzzih.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gnfyciovg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gvsssnizx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gyslabyjo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gaeaohmna.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpqalewlk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gnfulffex.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkoodazdg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gghrkblie.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gsbkzdjyt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gwzyqcvcu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gfjskwipp.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gawojwobl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/ghtpanekl.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gyjbcuemn.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxlmnwnqg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gzzfksyja.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gbdgfhnjx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gxoethynq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgvcjjt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gmwtuolum.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gvvcquyur.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gramjtedw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gpiunrfay.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gkxqgdtuo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gseqnpllx.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gnggkwcts.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gcxqetbts.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/goaitzudy.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gajauxcmt.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/ggkrhcybs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gycmvmcdk.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gtnsdfhtf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gkmrsszzk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gpqesdlbw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glwrpyrjx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gvrtyctrb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gidhfwngz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gerewtwtf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtfeyysux.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gahzmkzbf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcocdbsxl.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gkcbhkqzf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gpnpfyfph.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gzxqzwusu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gobkuagbi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gavydbiqj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gtdmuudxc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gpdtxxvdy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gonzfyovu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gklmrqezt.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gnfufboox.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/glnyoqmtq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gghugljuj.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ghdkjvsos.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gfkijhuib.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdbuaqrge.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gakwmhhdm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gftlircok.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/goqsjbtpk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gukgmhvlz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkjkbdsvw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gehqfrneh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gkebiqaww.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gcvvyeoys.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gacmkqhmr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/giuvazqtc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gkgjplkkf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ggjkicimg.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gzilxbnpo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gzzaxunen.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gmdleutas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gvoukudih.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gihrxpliu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gmxcakkvx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gfogojyjz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gsmklcrjc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gmognjwur.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/glkwvqfvx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/glfirybde.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grofqieig.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkkbxovhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gceuitnza.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/glccnulrz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geqtktoly.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gabavzkim.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gysktmpaw.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gxxztysfe.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrsqmop.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gntozlmrd.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ggrktmwmx.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gfowcgxqg.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gemedfrac.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gtkdjoxui.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqlyyzp.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gjebllpng.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/goibbeuui.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gyfbkgwrc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/glckmbdly.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbzpmvvqm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gsgekkysy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gaftewdto.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/geigzarzz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdhusimlc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtfrvmqdy.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ghjyuvihz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gcltvoocp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gbgontcyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gapjujrom.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gsxbcvxav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/ghbtvpbmm.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gqqawrgbw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gkesmrfpv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gbmcvpump.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gmfxrpgql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gazhrctbt.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpcraujph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/goltxofsr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gooascmwc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/ggfyyunau.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnsejcmvd.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gjtjkzboe.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gvyfaycjg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gqxxsidzb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gbutjewgz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gajsrkcfd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gbqocfwrp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ghrtnqtej.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gndqvffzw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/ggkzvkpxa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gpdyairie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gjzfnlbpt.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gtzmusqeq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gupjcswot.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/geoechlsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gyxmrzrcd.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/galbejuyy.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gvxcmtpdn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxheuhxqg.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gmmiccnaa.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gyndfzcig.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gcancbbsn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gaieggsqo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gexafmkys.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gfcrcgzup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggfaxjkkn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gctjvwezv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gusslgjqp.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ggoviyaqc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gafolontr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/grfzjuzyx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gkbdtoqmi.sHtML


<!-- 参考信息 -->