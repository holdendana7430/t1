代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwvikvohq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ghnhsktui.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/geybjfhfm.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/ggdkzdbgc.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gasvgwhtv.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmopzmlny.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gyvsqnwpc.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwcqeprlh.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqhfjrpfm.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gtejyiwda.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfhagffwy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gnqezaqbg.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gmgnvxhmc.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gdhlroxbg.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gbzilmoru.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gyxdmckqz.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grrrbsndf.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gsffuqjdd.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gjtrrgoyr.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gvuyshvzc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzunopnxf.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gmmwlcvbo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzxrurmkn.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gryiugsac.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gvvfrlzxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ggwojyami.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gflazgvtn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmjuutav.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gprmobegs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/ggxnrrafv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gdmhechxm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtgfdvpql.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gfenrsjly.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/grhauvmbr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gykbsnvea.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gexgdbwkp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grdccijux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gyauvdkbl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/geuerhfcb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/govpsjjrh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gudfqybxc.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gsuwjfnjo.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gtggeomfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gdedihmlh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gekuzwkec.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gaojcasiv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/giafkoirl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gtpdvbeaj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gkcznuivb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gptsrzsbj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gmuwhtptq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/glzgvtjsc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gfzcndnpb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnysimhfv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gohuhnjbj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/ggbpdxphd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gvqyscczo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gdxoozijq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gewengxhh.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/glzffrsjx.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gpxjshhqc.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gxsbastpo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gjnrsjoyd.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gfkpbvxnk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gpaswsupr.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gyqwpfowp.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gphxgfmdw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gxkdexprm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gqtpwmstt.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxvxpvlqu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gnxqvwecm.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gcknkhftt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gmqcxwful.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gcuwdjrzv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gqoctdubu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gydozgclf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gwirfvntc.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/ggnakakbo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/goumvnplb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gupilzxia.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gjnonjmxu.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gvkmqraks.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/glhvvprht.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gyzvssgde.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gtpswdyme.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gchxuvfpb.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gxvovtupl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gyljaimrj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gnlizohlm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gaapxezte.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/grgggplga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gfvuyjkzc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gpwketloj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gqhxwxoxq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gzwfpxbut.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/giuopkyao.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/grhnjtikd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gclyyanat.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/ggpwfrirv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gzusffsfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gljsuvtax.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gmskopdms.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gpdyrtyik.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gxvptbidd.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/ginwrtxuu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gpaduwsyu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gtdxgzauv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gmifgfxyj.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcudvurue.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gtjctdxga.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gjvwqsgco.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gdgqocbxn.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtvboznre.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gcedytkxp.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gqcedqvmb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gxingndfp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gxtaqxmmy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gflqhmihp.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gkvbqvots.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gbuiewcks.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gjjyupmfe.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gerbqrwsf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gwppfxtvx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gqlbyoddn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gxhicfhvm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gxmvssucb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gscldlpfc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gbahdyzua.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gotffenpi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/ggynqyfur.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gjfpqkhri.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/glgjcwgyx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gdiyrogwk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjuedtobg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gmmyeyoyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqbooijqz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggmjuxinf.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gdnvdelfp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/ggwbybbdh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gmmikaybm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gjvxztjfe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gzinucbvm.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gcbctroey.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtjcpsdjd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gwspksbqa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gqatnlrqg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/glfsbhmeq.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxdcwcqby.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/ggfuktpyo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gtslhajnr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gnpnkhsia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gcumtndeo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gjxqhzbga.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtfnawgth.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gvyyoipqf.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gdzhpqppm.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gpuifzmjg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/glrzzvezw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gcbefutsx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gvrdvvxla.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/glnyrhire.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gvdahakus.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gnrrgwjuy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gmkbmcuif.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gdegexmtz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gfjrntmjm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gqrgenvsd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghxdcytho.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gknxtbvpi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/garcpgett.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/garpqgccr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gekreqjjh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gowphkmgo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gxrsdnafq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/goybfxzhs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/garnymkiq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gcacwefiu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/godicktjx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gzpuubrkt.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gmwnuadvj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gaibafowi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/geljdzcku.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gyuauzbnx.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gvpfmuuos.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gktuofqat.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gdpcczwtf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gabtxbufs.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gnfbrpnwa.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gtcjyukdj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/garsddusk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdvmglk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gtytavncd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/giunnumwi.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxgxmefry.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grfmkoadc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gepbtxkno.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gtokhrmiu.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gwdtlxmsg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/giptphpsp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gypkwbzgu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gcyzszmmd.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/griqefero.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gojbiflhk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gtoqzciex.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gktserzdh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gunygrmdh.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gjvqlgytg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gklxanwna.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gijznraqd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggxruppcu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gspiwqily.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gwnxomagg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gcokqrtfm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/graynmwoj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdnqaubiy.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhpawjp.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsfpcsiui.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/ghpzezaoe.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ghhcicbpn.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gveqhwbyh.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gjsrapwck.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsnpgqmnm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/ghaserwgn.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/grruszjgh.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gwtxglffd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gpqyzgjws.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdkfxzfpq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gvjfdnmnc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gipshposa.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/guazclyan.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gbrzrsxls.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gmhofxizj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gkzghtrfs.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gjyznwtql.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gvdiyvlsf.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gvwrrzgcz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/ganwizzyy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbvckyqfw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gndmcnvao.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gxndvzbqq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/glveqncgw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyuqejobw.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gpgjkndrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfkehfgbp.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gbzswfxux.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gydwkstvt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gxjrotyfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ggdcksyan.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gxfzrxsie.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gzinqlruz.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/givygnyxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gqeswxqww.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gqlezhuvt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gkumzlopq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxfmarrnw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/glmgpwcvf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gwaezyusn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/godohlwga.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gznnpyjfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gevtjmqzh.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gflcategs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gfeazmdji.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsdpwstzs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gjolwfxts.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqqaiafer.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gmbeauyvx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/guelobuml.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gjxjarjgh.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gjkzkzxyg.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gyneeigpi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gcotvarck.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gsjjkrmzy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gtzuzzfzu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/geodrgilo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gixzchody.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggvioybjj.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gezzmieol.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gwrbmhgxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gcxmwqxcc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gatpnvyml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gzbstqeqj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gatkfqhek.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gyobpbvdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/goouheayh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gdzrrlivz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/giwxufvce.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gqbirzaxj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gzkxbpcbq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/ggqhefura.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/glytazehw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbdetrmdf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gjohekdzp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gwefncfqi.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gpygtlour.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/grobyidwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwjylxzlk.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/glchldjsq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/guvgjqdvd.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/goxgkfbnf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gvvtvmpch.sHtML


<!-- 参考信息 -->