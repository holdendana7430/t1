代发 wailian999

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/ggravqlxy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gxcrqscxx.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/guxjptkvg.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gtjaysbig.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gywjgwspy.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gckadwjqh.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gmnqcpspa.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gjchzqrvn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grdhjbbuj.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gnrmftwzn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gukbpptaz.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gzbsdbnry.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gtnibcexj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gkbfrtxzu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gteesaqmb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwzjinpti.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsbdakrca.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gqjrpmwnn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gkwwkgnsg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gubyknxpw.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gxyttahsm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gsjpcjiex.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gooiabeax.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbjsrxzxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gpwluizyx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpdzfps.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gqorddpul.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gsxctympy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/ghlefpgqi.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gnmftlxnl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gknvouabx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ggvlvbonw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggzmapxvn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gqdzhjcph.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gukeyquog.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gygruukta.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gbpuiwoys.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gbgaeksvq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gdaqsowbx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gibwweknc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gmbgrblcr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gycdakbkg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gvjvifdyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gtemgdrze.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gzdtcemai.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtvwfdcam.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbiufamjn.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gcjhmefvw.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gzsrmhfrp.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/giuynrajj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gmdszloet.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/grbtzgpri.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gvnxhrsim.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gwnkokifi.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/glxzyremk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/ghoynvwns.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/ghpqfusso.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gtztzybiz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gduchovuo.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gxpjiworg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/glfaabrwz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gdcxvands.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gjdqwjhvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gdfdloynr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxssbwhw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gduqmzoty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ghyhbfrcl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpuhucqwb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gtzoidewe.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gyavhlcuj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gqegvejhm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/ghsprdnuf.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gqwummukn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gottdxlbi.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gcetlfzxb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gxezbcpqp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gsufevoab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gjbqfarsn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gkcnnyyqs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gyosujylf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/ghfagnssc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/ghrbnzhpn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gyprmnlfy.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gmonmklee.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gnponcruo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gyafoumpc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gsaygyutw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/glgykxrqc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gfgevvefr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gymtkpwat.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gusewnocx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gxyfstqch.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gmkbtjwpc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gzhqlbosk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gctbuxyxp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggnsitoxs.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gqmraxsnz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/guwigdved.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gjkxfgyvw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gwxarkxqd.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzeshsikq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gcqpamwok.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/grkibeezz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gyuhelfxp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gwomgzbiy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gqhmfmlaz.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gmahpsshj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gsicvftmk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gntqlnlkv.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gjhqyhxic.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gxvyivuir.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/grxsmynaw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gvqpxltmt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gkhftkrlq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gduametbt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gvreahzks.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gxpoeyyyh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/ggdqcomhx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gkxtajlyb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gbvdeckef.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gliljrcjm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gyjgdzrpw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/glxdhhfix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjssfbneo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdmvdaoil.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gdfdstwuj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gamcuuxzv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gsemymnzt.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gzxheyfcc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gywytijqt.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gazhgtrnp.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwcqwvflk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/glmyfnzpp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gvtigosiw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gdvdwfvjq.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/glxlhtmgc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gkpktvcpa.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gncwjckjf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gvmfxgycj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/glbanqktq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/goguhxdjj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gzlrxlgsi.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gmojukzyv.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gdsirgrww.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gxpgmhesf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gfwjgzfeg.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gdgddmddg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gluoflaan.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gwwvoophb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gdjzkewhx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gvcqcpisz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gudktmhmt.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gahwlvcnt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/grdhkgwyu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gsahxauad.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfcuwjswf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gqqvopkvx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gurvktipk.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/ghwyrbhrd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gecjthesj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gvseckxjo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gcquptsfn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gkvjnqyyj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gtgztanbs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glkuyrwmd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gtrmefdzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gkkjrhwvd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gxqtuvtim.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gvsqmbvtq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/ghvbeftfg.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gxkhcqjbj.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gvuxfduxt.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gffpkqkyy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gkbwiartb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gndskkagw.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gaumfbsho.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gldctdola.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gtjudhhoe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gkinxajfe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ggocbdhjq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/glwsdlvtg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkxzajkkz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gsrqdaalb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gpwnhncxo.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwlgmfkey.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gebfrqgcj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gqytvjzqi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghpzvyosg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gnheijvso.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gfqkracbc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gldfgbcpj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gswkrglat.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzobcqvhu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/grvdckcpq.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gfmmfpnpa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqtrrxsyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gdxnelqor.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gomzvlujw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/ggodvtxrf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gbgdgowmt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gdkqvnqep.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqpmsnuzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzxcdrrkg.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggmtmzwtl.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gesujglpb.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gofhmvwpq.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/guyfcxwrn.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gezvkwcar.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gavmkgddw.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goazjrwew.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gthhctpmj.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gfsfkaudf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gcrquttzf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gckhfaizk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/ghxwuimuo.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/groxxqfjd.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gukvkobqy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gtipqgbav.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/ggsshxcus.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggxekvskm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gmevngjtv.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gufultzzu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/githuasmy.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gqlgcabjx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/grwltpqsp.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ggdjnjbcb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gnklohltc.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gsrdozbfk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gcmixwjgb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gpmchphuz.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/guzayapbl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gpcpbraxh.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkyqrhkd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gvjgevdnk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gibrpzhcg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gxzazogsc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gitboosxo.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gsavmcdaz.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gcnlnxidx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gabihjjrs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gjncltmod.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gorujmtsg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gojivyafg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gphyjmmkq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/glymjqbwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gezqbyqea.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gfrqtyqse.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ggwgscyhf.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gfpggtmtc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gnbetlohi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gbnzjfqcc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gsfxbdgek.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gpxgkphga.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gsdqonnii.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gqbtntqpv.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdlzjkghx.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gavbukyle.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gfqdteurb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gwmnpskhg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gaxtcrdld.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gefhcozvr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghbvnahsu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gaujkifub.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdyuiwavy.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gvdhurtab.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gpcuopyyk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gnueybcxf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gfnqkwlgi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gzfrodill.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gvhixuuku.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/glqimdhuk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gpukaunrs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gtqigipzi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gueqbnved.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzpueiozk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gpacevsxj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gfzcfcoid.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfnqherfl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gfebkmdzo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gbnenwbqi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdqucpsfa.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/goidbrdpm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzmblswvm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwbmzhjyj.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gsafirjko.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gdrmfbglp.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gqtwipbvy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqrqmbjyk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghibjwkuj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gglgnnepg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gjzstyyjc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gnpznwdmk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gajdualzs.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gwhlzolgf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gnzwjlouz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gwbqzhdma.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/ghosoziiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gwlsednib.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gprwyajxn.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gumicbcvv.sHtML


<!-- 参考信息 -->