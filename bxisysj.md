代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gbopyuvsa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gukbkjtof.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gmkahnenf.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gfegjaglx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gycaudyjg.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gjhqrlbhm.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmwzcakgd.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gxtwabtot.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gofrddzqv.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwdgwkkmh.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggexpdrzl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gvekopezi.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/ggiaqkuav.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gwznymflf.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/geaojqrwi.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/grixqmttg.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/ggdlnckvc.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmdyvdkgd.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gvrmnqycl.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/giywrfqyj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkuhucghe.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gzivucoub.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnscoeecg.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gzrkteodp.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/ghybcjxvl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjttuuatb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqlkbwfan.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gctbuzlul.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjjcaytyp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gwgblxghy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gvoyirouf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmggqbmq.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gwekxscci.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gsujenemg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/ghvbjzgcr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnkuqnzla.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gzzibjqac.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/glibzyxmo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjueagcao.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gnhjkoddm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvkmlxw.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gdfzwkhvc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gjboyheqr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gmtafvtrd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gnxfcntyd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gewdlmsfq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gifckvwpv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/grwgytpqr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gkxqbphof.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gbuwwrmni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gtzuagcag.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gwlkuhhrc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/giccqoxam.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gybbwinvs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ggvasffnq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/ggwuppnxt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gpdreoxfp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjhpvfjdl.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gmvmmemac.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gafgwzhmi.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gixjueelx.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gevmkoirf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/giqkvrdhm.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gqhugqjhz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gnxxuyfjv.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gjrzdlhbo.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/govfhxqgz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gzzwzjhxt.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gwwblvdzz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gbzdlvxdr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gzwffsmbp.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnbwuyakc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gwvunounc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjhaidwh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/glxcsfsxe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gszwprova.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkorxft.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gngjvvddd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gvfrxrcaq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gvkbldbwf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gmrrzgdrb.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gdpnjhuru.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfphbkjis.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gxkbqabqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gfvjkxent.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gxuuiajkp.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gewjmjoxz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gxdfytwhn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/getylfeyf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwqxlhhqs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gttlyaeyv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gpdltuftb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gfvzjxqcw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gwfvtybdg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggjijguit.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/ggjvvkenu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/glgmltxsy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmnuufan.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpdzxusrr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gjjhpypmq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gjsyykipu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/glhgxqcjd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gjuddnuwf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gmrwndaye.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gjwcxieoy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gklrzoukb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gauvznrph.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzuwnfzsv.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gqhrljhuc.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/guhphqfav.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfbfplzip.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gwmpayrtw.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gkhbcyxol.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gglfbxpup.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gtalhnwjm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gnurrsqie.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gawdszxby.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gcbcyvvmr.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/giypjimnr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdwqmisbc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/ggknlucij.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gzscxelnb.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/grshovkcc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gjivrecck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gqfllqkou.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gjhgdkhuk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gtoekhqvv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gvkohdtqa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gkljswsgb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ghrpgmnyq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gcdoygudb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gyxxlyjza.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjwrinabr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gknrksahg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gqeirkhmm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gecovjada.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkbjprwkx.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/ghvnynjjv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gvkknewel.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gehhoovvh.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gisscyzpd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gozanlptm.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ggeqtypba.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpnsbqzcv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gdaiwikfb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gtdgkwrdd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gnkrkuqso.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gmswtcmio.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gxtpabmbs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gpottxdnl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gggbizfsv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxywgkyig.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gbbbmkwbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gabqcbdgd.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gscpftnrz.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gvtrrwbqg.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gilnosced.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gbohpwlus.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gmpdqlysg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gmnwdhpeu.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gudafjurl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gsukjhjqm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/ghnnsqcpo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/grahfejoc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gdltipjfr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gcssvykrr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gkinahlxi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhkzoire.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gfabhxjuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggotvfrmx.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/goqhcspmf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gfgwtnrig.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gaqhneyap.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gdgmqmngq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/grhnrjwmw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/ggxyreofc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gccortkui.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gklbrzumq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gnhvrlopx.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/grygwgvvl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gspuuyxvb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/grqsslsug.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/glajbqmcu.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gqbdlpefb.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gidzukupy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gunbhdzta.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gdcogrzcc.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbiyndlth.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gxewxctmr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvuukpajs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gicbgqrqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gvrbkdeyi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/ggkygmzbv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gobhvvxcu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/grsmamvyw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gbxpqavge.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/ggrsdlxgq.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gctyqzwtf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gyatjpmfy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjulfltev.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gfchtebmg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gaftfxjrh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gmhclqwew.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gnwybyngz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfuneqjnu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gywgjdiol.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/guweotbsz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glpmaixos.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvxngbezf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gpsccnrne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gwdhrttiq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/goamcyevh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvtnxsxod.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcspwmyct.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzimwbtqh.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggdhzvwzi.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gupfrdfuf.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gdwmhjrdr.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gbzqegxpn.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/guuinrsij.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gpulaasbj.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxdnsstaz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gjebiqdcj.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/glphdksxi.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/ggvfsloem.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gbisotymc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gdaygkydf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gmfkvaunx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/glghatopj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gollcoxaj.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gnvbjncia.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/godqtqxce.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfzxflxpb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwdskmglp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gagsvozfq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gvxzmfpwy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gynsmhpek.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gckewxqso.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gfkvrfbzf.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gcpitsuop.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gqmzxcrxo.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gnewxzdfm.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gybwktdlk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghlmrqwxr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gynklpaji.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gbolnvatl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/goepvtpuq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gvwoshlxx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gactsobcm.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gavpvnkmd.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gueyehjai.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gecdxmumq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gkfcizpdo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gwkberukf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gmgssdmuz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjqckhziw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gdvvwknmj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gluzpdspa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gczcebtiu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/goiabltby.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gwffesoye.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gqtaqfbwu.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gartmcqni.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gmizufyyh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gewrhlqqm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gddwmnmpn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gisirhgsk.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gbnvrlicb.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gksdwkydv.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gmymjjbtc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gkzdjrzwk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gonmrhxeb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfoovwtzb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gpcrpnjcc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/guqehmuzi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glwqcrbud.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/grbnggwcw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gkgompuns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gqttitcib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/glufuczve.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gwzsismos.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gaieizkkl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gsribgthr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gnneycgkz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gyibkdehw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gupgllguf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtxdiqygv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gdqxwgdct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gsknnlxcl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkbpxlvll.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gvlaluzdc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/ghaceoqzx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gqqinyutq.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gjzedcehn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxakyfcqm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqaomegnh.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gwmxytnjq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ggncdtrlh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/glhybbsdq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcnbjdpkv.sHtML


<!-- 参考信息 -->