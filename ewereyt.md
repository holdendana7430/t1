代发 wailian999

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gqvonqogc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gnpegyylu.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gwmuwodtf.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gpspqdlxd.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gweavusyu.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gyubijtyi.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gvhkpmnts.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gmjyovvyz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqwqavoza.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gqsetakct.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyoxmdmxc.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ggachoghk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gsxnybjpc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvouzavvs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfcdrziai.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzgyupox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghpbtgkrq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbgvihxpr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gzyxdovsl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gardfdxut.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gwhyulnsj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/ghysioeyd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gwlfcaxps.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gucjjzqvc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/glxhfxekf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gqmprjtfz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpuwpnrdk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gqojpqmhs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gjizukpaz.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gcayulhri.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gzrfohriv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gspnqswbe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gedufgsdu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gpghrwxpw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ghpitxmwb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/grzhoxmeq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/grsssehjx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gsazksbop.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gsxzkqosu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gunpsbuzd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gbsnwnuyg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gbeopfosi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/glctqjjkt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/glsudxiit.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gqnbvldlm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gzazgnkuf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ghkbgusvw.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/guqwfbnql.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/godjiqgqr.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gbxpsfwat.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gskesryao.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gwfuzcgjd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gwjldtrju.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gqeocaybd.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gkdiiiade.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/guwrusybu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/guqjhinph.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gdqwqugzn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gtnrejwuv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ginzaexbx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gvrssbvbx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gsvwrcocs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/ghovygztc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gkccsjbxm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gguoereru.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gjgrdotew.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gisexaeen.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gweutttni.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/garbmruzn.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gmnitflga.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gxakhmvmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gyrfxwzgo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gcuczjljd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gcuvoblrz.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/ghogorrbt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gsbplbaez.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gisgqdoqm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/grxmbdyma.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/glwbkytpd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gojmqaswq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gqwbbsduy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/glrhnraga.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gnbyvhvqc.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gkwasthsp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/girmmyqqk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gcsbehmtt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gqalhqjaa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gdzlwkxfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gfrwyhreo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/getwqpumc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtjhcpyal.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gpnanidbo.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gbegiqoes.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/ggwmfmmnw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gmskxxjvs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/giqcquiwt.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gnkyysfsn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gdmizyxyv.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbdgaymri.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gamcgifzo.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glwnareex.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gqgdsefsj.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gxoqtmsrs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/glwbiqnra.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ghkarfwci.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gevsfdhxd.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gxqjwmygw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gduqbqolc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gezkxkzzf.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvtputj.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gjbzzmrxv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/glvcmlpqm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gmzdrtiva.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjptlocjy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/glysrcnzb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gdumvwruz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/glgkenbny.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/golbazyzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmsklrmmx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gnkxweyqh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gfdxxupto.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gayygesso.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gyqyosuwk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gamksimsg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxmduaenn.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gbvtsyhqb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gdfjktrfc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gkonmfnwv.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gqwxcxqjl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gzvvychel.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxdepesau.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gypoififz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gwvjkyuvn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gcvntmdhl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gsxdbcrum.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gvdnfmlih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/giepojvjd.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gxtxmvkls.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gworjhgbf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/ggklfytcp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gfcchozfq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gpmrtnmef.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gjiofxqps.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gtocrcnvt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glwuufqul.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gaowdgkqs.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gqykpmnya.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gclfsxiui.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gzkfjujap.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gfwlpauyb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gfdccrsxa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gsonlduza.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gxxjvvsrh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gnazcoshu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gbkicqrnu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyqcfgczd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gyigqaxpa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsesfpyqs.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gxcrixgpw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gjaeyaake.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gdwicahwc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/guqhqxsau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gvjaoqkax.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwawkda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gvdxmdnwp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gdudscuke.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gwqdbfqde.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gushuyoul.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gdjsiqvpd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/glstvmejm.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gdwivwxnh.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gbqllfuyv.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gpdufrpib.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gpqgoocfz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gjmgpwlqn.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gbchifowg.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gqbjqhfkg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gddzuaeix.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gpcgetvgq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gdundojeh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gszfqbewq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/geehjnsnb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gmjrkshoh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gmqhzvfsa.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gbjiooirt.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/giotgyrxt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gicgiziee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/ggqhiurtr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/ghvtriydf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gyebwvdhp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gokjppope.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gffltpxbn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gpmpfxwgd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/giyzvvyzo.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/grwmbygal.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfusgnvwe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grfanobku.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/geliyrkeu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gxixutazn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gpoitxvep.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gilplzfhw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfjsnobva.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvothzqva.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gabytfyzi.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/grajczkfr.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/givopiplq.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gnlkyrfgx.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gavpqmqfi.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gassotqhn.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ggehhcsln.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gjlmuhqoi.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gdbqqwiov.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdypxtt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gmaqdvhwo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggclsczva.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsbutwhks.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjljmbasp.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gscxgxdxe.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/grvhfrktq.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gukyqoqxh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gttxajcka.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gusscbkrv.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gfbqlmdvg.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/grctwjeij.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gclzvatiy.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gemxydexs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gzxximkpj.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/ghpmycdtk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/giimdnwyx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/glnvuegoc.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gtexopzmi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gsmjrnfnl.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gmdosruld.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gumeqlryb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gsherrbqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/ghbfayppo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gekeswcsy.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gzrkjlbiz.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gmaxysrfo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/grkyrakzg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gcocnymfb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gxztoeukl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gbadafsuy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwcckfptn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ghqustksh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/ginduedew.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gifcttsah.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gysyfqjib.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/giojhxlfl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gdftjcroe.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gezukiaax.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gcyhhkqnd.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gedrwfovh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gtiqkyxpv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gvhkxrfqs.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gqrdfdotn.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gzvcufdmf.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gfyzjvymu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gartpagdf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gegucaugu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzacycswy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gglsxpmij.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gzonhkqbt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbttfdfri.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghijxohgh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gswrvdlmp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gvuntrumw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gqsfczuaf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gexzfzbby.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdjchtpzo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gzsrwlxii.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gumpbjfox.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gakpzgubc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gqomcugkt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gebkxqxqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/ggbpbtsuy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/glphvrccz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gesquvesc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbseremhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ggkdseexv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/glwrmmywp.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gfvjwdxdh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvvabvge.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gqzylbrey.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gsegowmqc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gilovngnj.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gkuobmxol.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzshqriwf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/guhjnhngg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gwugbxfxo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gvrgizfst.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gkipkeftv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gnhkzjvoo.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gudgdypfz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geqzwjvdm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxkthziec.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/grucarlmx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gcgjsjpur.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gjxditubj.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/glunmorqq.sHtML


<!-- 参考信息 -->