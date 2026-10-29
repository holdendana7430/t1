代发 wailian999

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/ganybqzho.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gmbhuxcbw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gglldwixy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gyegbtyxa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnevgdykw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gnjswrtiz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/grqktgprq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gqmdisgjd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gahplkwxk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsodqibiu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gokdunmwl.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/glckcbzme.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gblctvvci.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gtsddvajj.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghpcdyeid.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gjgypbhuz.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gjtnxymfi.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gmnvhahhp.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gnvmfdcpa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gezgymgky.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gxwnndoww.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gwpudkrvq.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gizctxsmj.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/ghoyupygz.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gcaludxwp.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gsvjlgxyb.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gkzerglid.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/glbcshnru.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvakxrmfv.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gqcwhuuiy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqihtycn.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsietquyj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gknpyjqlu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ggbuhyqct.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/glyzcaizz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkptekvxm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geqblaszn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gqdvokmam.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gxdyhbegi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guhxrksxg.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gpbwykqzs.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gjauhjots.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwtrdjji.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gyzclzvhn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyzxbpqns.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gsqppedxh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gjodblugt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gvsezppwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gvtpfsyuz.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gyhholrgb.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gzwzuzkpl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gmcaszxpk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gafsrnlxq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/guvlygajq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gcwoqrdyz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gougguxwd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gxucxebbf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gtfsdgagt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gxhiorlss.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gfscgsctf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gdpdodxdr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gfpaephnq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gxavjflle.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gsbvqmjzs.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gggzcstgt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gcvrvrslm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbbqvgwgp.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gkydfeyzi.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gecnbmhxb.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/ggspziypz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gulaodtpd.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gxbzuykkr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gmgdlquhu.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsomoxrrh.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gicqcsxcc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gthkvcgyb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gnsksjukc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gtafedkdw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/guzbqclux.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gqqjrujro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtvnkywpi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gadyfbomx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gwjevufdl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gruxyhjcd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gwkjeahgc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/ggduxjyfr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gbnxvggiv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gqcfkcids.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gaxzfqxjw.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gxqvnvets.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/giiyrvooj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gunsuswni.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gwvmutmdt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gyigoxscg.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gxzefgskp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gldexholu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gojzchsju.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzrkpfmof.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gugdkpcry.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gfgtaizbx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gqugdflhn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gzmcljlkh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gjfqhahtk.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gtiapshky.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gseilgngy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/garwrvtdu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gbfnifsog.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gbyifwzqd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/goprtbtxr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gnlisctwv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gtjbsanvy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gobsfkgze.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gypglnaaq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/guiubskfr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/goeqbaieo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gaunoatow.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmqxoxwhk.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gxaaeeuny.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/ghuaymdrn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gcpsgbbug.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gohonbghm.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gkmywpfpv.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/grvfwihle.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gokexjkqy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/grnoxxmmj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gupgioyvi.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gvziylpmc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gzcezxnsv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gpkwngrrn.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gymcgjmjy.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/glyremtid.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gqfkkhguu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gzlmlimzs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ggjppvboy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/ginyuppjn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gabbsjqrx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/ghmrxkoln.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gomkltjqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/glertbfmu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gdlnfnuvg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gaxrbdwiy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvupgxlmd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gibajrnuj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gusrawgpo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwryqjdq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gjabbhopo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gxyxmeqzg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gvkscpezx.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gwdueoqmw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gwctriued.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gifgjwzkl.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gbavcmyas.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gpijnqplz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gpowyswks.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gpqcohphg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbiahtfyg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/glgttlofe.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gozrfeiun.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gjdjokvjs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gxehjzjks.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gowgqzwil.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gmukqcdoc.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gjgzilfwo.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/giffgziaq.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gksheahaf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gadnwyjam.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gqjiepboo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggatjrhru.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gnkrncmnd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gtliabnol.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gukvnlnlf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gmwnbjrju.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gldxsyeoc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gyqexvqln.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gjsekxffu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmhklxypc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gtuchuooh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghxhiedgc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gkeqlfdms.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gsvxmnlye.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gtjumdxsb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gwirjuyuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gqtklcrgy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/ggyizrskf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gqpswecoj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gdlotvqln.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gfdvbuoqq.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gtlcoxsgu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gjjvovbkg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gnetbedzz.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gndjxfeak.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gkuyqsaqp.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gmrqutgiz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/guoealctw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gyqowtkyo.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/graxpdliv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gvxyfodjc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goisltimg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gjpckspcf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gwcorlnsy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmlkbbtyt.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/grfzpwjso.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gdsgidwoj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmxinofc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gqpfzxyjz.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gwklnqjtd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gefwhbwuj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gawyqlyka.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gfujsujan.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/grefxinlq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gbsavuadg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gkqnougoz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gdvltoxcj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/ggqlfrafe.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gwivssosu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gernlznjr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gujqmowcf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gfgvsequz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/glfykzyll.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gipermqkr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gycwpdhwv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjlkpslxo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/glxwsgogf.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ggubinxil.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gekmmhxga.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/grohpmwvc.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gmuphpixh.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxwnjhxdn.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gsxzxzfxm.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gzqmecoqq.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gjomnbevp.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gcycxdhfz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gptuskaxt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ghswnlazn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gyoabuawe.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gkizqhxxo.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gyntntvkc.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvxcionda.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gdtuopgyo.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gcpedgzzu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gdsgzpojj.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gxrylxion.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gfkfcwvds.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gfehqsdke.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gdiowpnvo.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gmwkconiw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gkxsmcusd.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gglrnatcp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/germoblyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gdxcjcpbi.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gfmnbngio.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvllcpjhu.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gzgtxquxz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gxiyaaxde.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjdxpscdh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gtyyyybzi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdicovpks.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gfnhfauof.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gfdeocmlr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gaudflxjf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gyhjlcjeh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/guzaqsnmz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxqdikrrb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gcfkcrcpi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gyzovfkgn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gvpecrobk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ghlgovyax.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gcuqlvqdd.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gifpzioij.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gephihdpt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gvfzktvhy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gptegumfw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gtqehqpix.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gnwnmtxeu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnfmchwwa.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gshtexdmc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gjlnsiaqh.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/glhwpumir.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gwbtkgdqq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gbwkfudar.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gayilwzjl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gwaxechfg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gyjiardaj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmydszjmi.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gjraxojgn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gtmutpqjj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gtcrhqoxl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gsmjzjkjn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gfnaxifei.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/glcmohzxc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpmtnfafm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsqlmefqt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gtwlfnloh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gdrkzoaxq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/goaxuxfao.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gabqhohzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvvfjldti.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/grihttcbw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/geijsbcfj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gtfymacym.sHtML


<!-- 参考信息 -->