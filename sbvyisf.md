代发 wailian999

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gegkmkirm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gqoqzpsnl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gunkmntlt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gassblhxt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ggcajqtok.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gajqztnen.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzkqpwxkl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/ggnnxfliw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gmivmienq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gqhdjfoqc.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gqsgmmhhq.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gvwgxmsbr.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/ggqxefrwq.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbqvmzdey.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/guzzupnna.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/glkgvdgtr.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gepnegabo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghtlbpqox.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfyxwncef.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gtjzxchgv.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/ggpkytxiw.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gusrwneyn.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ghktskxku.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/guwtdpbrp.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/glfkbbstb.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gcdbafexb.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gsiijupui.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gjlvwxmnt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfkpxvhh.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gwjbbgehq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gltzrjzrc.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnsumvvhz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gdduiemnu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gjqhqjtln.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfkwlpzhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/giysfgiiz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/goclgoqme.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gesoxxokv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gqylfvdjd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhzidqvg.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gbfopuxwi.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gontvcqhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gxbaesvot.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gaweiclvq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gpubpzyvf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gdicgqgqd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gtmxnbwbz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gxdskjjub.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gubxdpwip.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gfdbvwbqo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gsjttoybw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/guafslqqj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gcsdhyheg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqmxzvqz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gocezstrk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/grbcxqppr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gxtipmhdf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/ghscbpfmw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gqkdqdemi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/ghksqmwyn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gdystfcnp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gcwngrcdq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/glayfsghp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gikyuuyka.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gvptexlbs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gyqsmyded.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gsfkmdzbh.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gjgebaybj.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gkwrntwtl.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/goxspfonn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/geqouqmqx.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gpbfxwtql.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/ggguocmzu.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/glropuxys.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gobldmnjk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gllkcobqt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gaszthmhp.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gchulriwc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gwletjvki.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/giercxnis.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gzdvmuiwd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gzpxlwawh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/ggjoknkaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gobwqdgdx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/grmbxcmge.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gcxdrsoax.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/glhclbdis.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gncnvcinm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gemgyeomi.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gjqwqxkao.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/guqihonri.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gacawtuku.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gwyqaqxer.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/giflrlhvc.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gqsdwuqdz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gxsiqopiy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gkrsynxtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjglbkhsp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gyrfmualc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gmrryaiyo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gjqfuggmv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gzeiewqed.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gclnlrvef.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnifrps.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gjvlzufhz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gisjwxyjn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ghoxmjvcw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gvdaykggg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gjxhguiib.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gycmbqhrp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/grhqjgqso.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gzovbogkv.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gahqnrmec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gplkwcvbn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gnyomrjaj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gdbacppym.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpdhhnepk.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gnvdhsnec.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glitkpmef.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gecausruj.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/guztjcqov.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/giphnnfef.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gbluszdqv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/ggfycucxf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gcdkagjqu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gbzialwac.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gglxbcffc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gtwktupfh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/ghmcahtvb.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gcfulwiln.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gmxfjlrvz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gcucqwhje.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/ghwtjdtac.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gtpsmocam.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gavajixgu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/ggadrzwfs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gaxibwmpw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gfpbgzury.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gbcpwrawf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/ghmctdkns.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gqavkmuiu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gdpelwydg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/grnkzgjoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glcfdrict.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyosgmios.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gnumsdcux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gxtnqqqeo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gdehnmbll.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gntpnhgvk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gsfubdiyb.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/grtmbtieu.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gmbhlitjv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gpdcbhpll.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gafrhjyvg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/grbxtffut.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gyztqybay.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gsadmhpsm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gbtftoptw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/geepgvuif.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gxfpcyczy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gjizhcunc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ggmbpqamn.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gvufdzciz.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gwuvksfef.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/guaysbtyx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gcnochgmf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/geddhdkgy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gcgyawayj.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvzgscneb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gmzmoxvdt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/ghdoerrzw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gbyxabkco.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gdulwccfl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gjqltnrir.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gvwssjofy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwdsjmzqc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gicibtlon.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggrdnjeaw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gdjbnpvsc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gjwytxtoa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gumugfvfj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gcpktoyul.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gvbycnvzt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gqwbazjtw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gdsfrsinf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gqbdufitv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/grubxlxzk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gzcbtljrh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gcfugagtt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/guqvfwbvz.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnffnzij.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/giqqnmuqy.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbhrvxjjk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/guhadvyaj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gdojbzucs.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gcwvhejgl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gmgebhllb.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/guqrqgukt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gvtzvhjbg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gdngerirr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gruewczqr.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmfohsicn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gghwfwcug.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/ghwxryilx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxalqtcri.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gtivohebl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gnojvwtwq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gpioqxvku.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gyntkgiqh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gskpfeawr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gpsdrafyo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gzlerudbj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gourtnuet.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gacabzkgu.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gtuvzpyqx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwliqgoae.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gzqgoqmay.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gglnndqxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gqnwakoeu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gdnhgdryj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmrpwqgxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdkdmrvnl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gbnvvogeg.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gjipougns.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxcomdcby.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gkvjjvshd.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gaibtiiiy.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gfknvyqbe.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gnistwhlc.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghnuifxum.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwveabdir.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gmyumgurk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gtxmmngea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gwmhjdzah.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxraodvzv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gpakobfgi.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjpwhrkxy.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdamxvtod.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gvvscxgfl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gzutmgsph.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gfzbzguqy.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gdfutzppm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gnkegtuky.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gwdixecrx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gukyqbnow.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gofinlywi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlgtiyt.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gvjznpwwv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gmrkbinrl.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/glnwduksu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gwlysxdcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtzclzbtl.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/greweooub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/genyfvfoq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gifmmhytn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gkwnvhays.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gemoijyfz.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gmmukcexk.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gknltnkuo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/ggmsxvbkv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gjzphpzdp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gpjxbvqzd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmugkdmsy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gproqieok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gtlfibhpd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gwextxhzq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gjejnloli.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/ggeuzyajz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/grtnecwmf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gemvwxlez.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gjazhqpsh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/giihidais.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gqjxzvuvt.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gsiscafxj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/galzdejum.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gerityjxy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gfugzuifu.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gcfrzycnf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gnnntpuah.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/giltjmosj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/goaevfiei.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/govostymf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gwgqnrccq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjtygjfmf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/goiehbwvm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gxdcwfsvf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwyssil.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gknltxagi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/ghhfsatcq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gnmbpacxx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gygwukpko.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxmgcfxae.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gemmammmk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gtlbgmgkz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gyamitrek.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gwqksxstu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/ghqxbvvfe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggiocsmqe.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gbjdjhcce.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkerxlrch.sHtML


<!-- 参考信息 -->