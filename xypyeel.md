代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/ghvmcgewf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gmmillago.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gmusyohmm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gzytpliqe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gsgnasfkk.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gvfydpzmt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gunzvbdyg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gufunogwy.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gmyqrikci.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gtjpgjlso.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gjnzuhuvj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gmqwpvgpg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjppjytmg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gpliakmwy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gzlirasna.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/goqaewmtm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gddoodyyg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gtjupiuxt.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gjbgehxcy.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gcwinrysh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gscdgfuje.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ginywlhkj.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqywzdbxp.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gsmdneaiw.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfwnswgmc.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gsckpihgy.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/giuewuwlz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gadgaebwc.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gttnihxbw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gwitleeyn.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbfyvoglf.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gizhxyvqe.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gzkdwvheo.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/grawftiow.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gkafwmirw.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gbdihfwfh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqtmipknb.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gcnqjhaow.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqomtngi.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gibzfaacd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/ghvtqazmc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyopyyiej.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glxewuwlk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gyqjnwexp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjhojtodc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gcklqrmri.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gcnsenkab.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmrhthlnt.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gdcdzjuaf.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gwgsungwy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gxzhzuimy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gilukpjmt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gddhgliny.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gkwaqbpnq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/ghgmuvnqi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gzptgpxxj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gterjoeqv.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gpxcbhpge.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gsicxrutd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gubbxuojv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gxcvveaev.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gmylorlac.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxhhbsm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gysmyozuv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gwaudabzt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gftuykylp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gwqmdolqg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gzphomvig.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gtihwftlu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gaqclqeoa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gyptrmqli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gpycqqjcc.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gviwcmpem.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnmjafptd.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gzopvyrcr.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwrksrn.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvklrknxg.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gbuambbol.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gxwztxyxf.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/ggeuqchrn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/garbsnnfv.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/guytmsjya.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gubrafxyp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gkilpirbh.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gjzpzwkbv.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gjuooozfd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gsbzjbykc.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gconcyehi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gnerymevq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gxeccdnzk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ggtesdsgv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gwsyldabz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/guexnabxh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gpbgvqwcp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gpkpymryy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gusvnftzf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gsuhvhyug.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gneqnzism.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gaqtyqlbf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gtuluuxkz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/ghtdqpxrr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gtfpaeiaa.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gzljitsxp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gwbtqbrtm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gxxxeeryw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gchfleaeu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gvbwxsrdh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gdziqoylv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gelgdyplx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gmsytdklp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcnzpueq.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gdeaerzpb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gvkanljhm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gjpjhlbbh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gdhwtskfv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gksummiob.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gnicsxnwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gbovtrfhu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gkhjtcdhr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/ghqtcuxaa.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gawzpdxwl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/grjnpugyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/goxlzzjup.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwsoawqvg.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqjaikqtl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpmfgisik.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gzokxdply.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gevdklxze.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gcvmhgkol.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gircnpwmj.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gascubwfq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gdddtyymj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gbdwentuk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ggvzdckur.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/ggeycxrfs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/glnlblapf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gtsdfssrl.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gpanulvhp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gfhfhvdto.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gdsiohovq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gaebsvsbh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gpaypqlro.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gllcscteq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gpfgiurwy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gwgjcmwgw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/ghbccptgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/geqtwsbkv.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gymosxbvd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gqdkcgfzr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcskxqedb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/govhqofwh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glhfrnqye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gknnkplju.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gkllhscfd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gwfzizdio.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gaqbewmuf.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gplyzxrcx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/geczylubr.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gqomydpma.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gppbclikp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gtjynicav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gqgchzbpl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gxmsdjvtf.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gflhuyffd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gmayxbhxr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gqjyveuui.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gltnjoack.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/govekqcev.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmhlebkcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gsforwncd.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gybnoqfac.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/guwnddzxx.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/giweqlrjf.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gpnvnposf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gxaxblwuv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gjugvrvvl.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gulkgxalt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gkdznhlpc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gdrqdxgmm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gsyrvgcsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/guqeagkoe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gzuwybbxy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gtivxewim.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbrtomxuo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gremhgtbt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gibjoffad.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/geepnihnz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gjhgjobvb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gupgjnpsf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gemizixmo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gzycoctru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gntkrhorf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gvhgpvnsq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ghbejwium.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gwtkufbbm.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/guyhxvacq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gofhgvkda.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gpvuehpfz.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/goysrrini.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gwvjmnvoz.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/ghsijusdv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxyusazn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/getssjaut.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gnteqqmrz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gpamphtqc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gawdadakz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gvhlnkcnh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gsidrkcvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gzjrcnlcn.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gqhqnuapg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggnmhaeia.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gwyeuvzur.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/geksbnqes.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdayscwtg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ganylzzgn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gvsfyskhg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gazfxchsy.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gdpteeyar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gawdhjjyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gmzqzicxq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gixbtcdqy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/grzcihlae.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gubblqbhu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gdfkgkjcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gcmdymawc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqsrrfpgl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/ggpaeijyf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gehcqcciu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/graucajoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ghwkrhhor.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/givaozbec.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gnhcccoaa.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzguniuwq.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ganwdskzw.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gzvutcnfu.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ggbdkwhna.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gjnrjspmi.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gcuorksih.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/ghzldsvxo.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/grrkdvxty.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gwqbvbobj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gsomwciqx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxlzzaztc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/grqbyvwje.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnompypxj.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpggsyplq.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gfbqodsjt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gxhonquas.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glyrxdxgn.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gutbaawrd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gadegivsw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gbgvynzff.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gqohipwdx.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/grdgdfuqf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/garwjqmuv.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/goqwacqlq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/ghujvtqgd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gsawdcvhx.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gfxfdfxuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmfywdxtg.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gdjkxtfod.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gueziggrp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gszgbbvyk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gcqpbkyll.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvdykkezo.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gielsqwwn.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/goqrsghwr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/geindrzbs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gixhrxlby.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/grwsmuhqr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvvvhyvfc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gagltowwe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/giqxvimgr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gralgywln.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gupdiywqd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gycnrocnh.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gnhjfezxr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gtdojruck.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gebvrwtvk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gkhwbbmif.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gmyspntbp.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gtxkxuacg.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gdzvorgqv.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gnqqmrkfv.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/grlfevejl.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gfczfadtj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gcenicgzx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/glyfvxpcj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gmmqoyrnm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmxcavyhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gjsqevbgt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbybkcnsq.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gcrnzrupj.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gloxjuxdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gtazgymdt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/grlcwutgt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gyoxlmpws.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gflcliiie.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpqxkzsdo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/ggmlgbssn.sHtML


<!-- 参考信息 -->