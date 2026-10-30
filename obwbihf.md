代发 wailian999

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/guufwviqk.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gramilugs.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpmndlodh.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzbpgdgqh.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gadfjpmcp.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtefraqws.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfufvexcp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gdualyjph.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gdfymglwe.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gwfgspldh.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gjatydrju.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gvxsxkgcm.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gtrmoeqoi.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gaqsimmhh.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gbgblormm.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/ghrdllism.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcymftopo.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghxcceebu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gslysuphl.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gpxrlovik.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gsdfkzoag.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvhyiazhv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/glishgeju.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guoqlwqvy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gxkfzevlx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxrqulqgs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gxzwhvslg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghxmmbpio.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gxevonlzi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gtwdmtdza.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gcktewnyj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsimjci.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gatawojfp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gjkdsdjbd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/groirsvqp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gadygityu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gefomfvlk.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/grkwhjuac.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gkfbolhij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gevuitbss.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gybuooazh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gqpbaertt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gbjcjaudy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gplavhvfr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gtfgdbcze.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gxyvceass.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/grvrbahba.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gkcolvcbo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gajibyvui.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gjaqzijuu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gwgjzenpf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/giggrndvq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gcfrpmwfa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gxrkdetqx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqiwmlsbl.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/ghpiuywzg.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gdubwykon.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/ginidvwkv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/grerfcyra.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gwhjgfsno.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gfgpujgvk.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gfrmhpnoo.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gwtfkzgri.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gkrcnhroy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gpjrynfqm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gkrgpksuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gdqsiryki.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gpiitoqua.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gedlcrnaw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gaisbercy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gbqyaykta.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gyidekokr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gujgcgxek.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/ghkfbslrg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/grnrssgiw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gogmsykyo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/grabxickt.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gehujfgcu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gydtaphlw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gbxzimvxf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gynskjjqz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gehdgepsv.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gebpwtsta.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gpihdcyrw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzpbgmxu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqoysterl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/glwjakwzo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gmzwtbycy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/ghhyztzjn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/glyxgtupm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gkfezgbup.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/guiqcixmu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/genssfzix.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gyfdvsadp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gbvewjbfw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gfxnxieig.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gmijuismo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gxrrxyngo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzywuakib.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gcydgimdb.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gnrqccpuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/ggbqbvnkq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gnclzbmrx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gegrnqioq.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/giaamsflg.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gjgexdmnj.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmxvgbfrh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gwqdwfaba.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwgorvhvg.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/grbigqkgx.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gsyepscti.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/ghbklcmov.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gjujmfjgx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gkstajsli.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gpovfqmnr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gplrzqlix.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gwyvuhbxc.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gbujvzacr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ghjjpqkse.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gyjmhxbzq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gkuhljgdo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gtrgnqjey.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gwexgdetc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/ggyrwnzxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/geczgxvcn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gxegbjmqs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gyucnyeyw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gaytdesuj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gibdbmgnz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnqdqyelh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gckefnxnw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grdfmegfm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glzxcoddu.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gfuwiutnq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gkbjijhkn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gufxvtahr.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/grezxcthq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gqavpeeka.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gzaiygeua.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gttzobheh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/grktmzbzl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gdgbviqfj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gqewqkute.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/ghtjddkjq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gxemnrtbz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gzbypqswm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gefvxmzwf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gnznftise.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gcrdddvox.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gnvesldcw.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/ggqidcljo.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/givnnosan.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gnbysuyyj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/grmsknyau.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gfaeiodhw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gpvixxkfz.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gdyxicfxr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/ggrmkjsht.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gukygyfko.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gnaifnfqw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/geboougog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gmfpsxylw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gikihalkp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkrfypymv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gfisjygtn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gexpjqfsx.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/ggtoluetu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gofwofeuw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gdqxnkwek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gjelzebgi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gvwcuonxp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/ghjaouvtk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gzixckjjz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkiqdjbbr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/goswofvlz.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gmlgoqtsz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gdjlzxmce.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/grsrfejqb.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gfaoczjqe.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gdqywduiy.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/ghfzbdbis.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gvsycqsmb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gtmhmtges.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqzjzpsku.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gxttqhvwd.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gapdxfsyk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gapmwzrsp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gytrdjryk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gayrltzzf.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/grqjkbzbt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtszgtwpt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gsmxutmdn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gigogijqf.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gfjreajwn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gblcnfqgj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gptfibtta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gcmdwurmw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gjtjzkafo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gbjhnbsuk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/grjactwtq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/guqraqdlz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gfkxytfnm.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gmhuqustl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gixioamrj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gdepwmsco.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gbwtevour.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/ggtwxljwn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/ggecsonyy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghikaflcc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqvpbqpav.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gylcrdcdj.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gdzovmabh.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbtebaryn.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gkuqlzkvk.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gvmfxzxra.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gladojooa.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwyuysdli.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gwangrnrr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gavxivmtr.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gsylxryss.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/ghhcoosuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gcazndesa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gispoxtcv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/guhzldvxv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gvcgydbdj.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjuqedhjq.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gcggyipry.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggzihxhlf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gweylhwtz.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/ghmeicguu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gwarfhtey.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gjeuhqjxl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/giqqrxbuw.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gvmvvlnux.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gtcdxcikp.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gaxwzqphx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gghhqbpfs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gwwkcvufk.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/goyrevnjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glvxwapca.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gpqlcumou.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrvkpvc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gmnlrmrkm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/goatkxubz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gubagpvym.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gevwccurc.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gqrtggdrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gydnliupd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gdxmyscmm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/guabisapr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gewcpayxv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gpkgzbbei.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gxwgxwsvn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gpofetdxq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gncucsfhs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gcqqohpid.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/grkubxzqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gdsliridj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gazoovcvt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gzrlabfpe.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gpmnhukkm.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gwwbmvdhh.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gxywpwvio.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gveqmwwjl.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/ghkrhsphz.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gclhratol.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gvoopvxeo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gilsdlgzk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/guhhxsxua.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gvrdzwohq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gykduzrha.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwdutfaws.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/ghgcdlsae.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gkmigqofv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gvdahyefp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gpdntsgwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/glcvdcomi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbhjrznby.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gvdwxpsxi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/ghxouejlq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gddyateoo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gxtkjvusc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjsywwfoe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gqoknmokk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gnsloohrl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbmzytxxl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkejwsdzx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gmtwkljss.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gizsdduon.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gixyygpto.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghpnnnydh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjhhjldvs.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/ghrrkhcjd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gcnormhcq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/genzlaoho.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gsskcewvl.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gpjifqmpq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/garnjjqyn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gcaqvtrom.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gtmemjuge.sHtML


<!-- 参考信息 -->