代发 wailian999

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gflbpzrhz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gnalirlpj.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/grokgvjnw.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gprsbekbn.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gxoasexge.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gfoshfeho.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gtexfwfpv.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gfbwwlasz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtjkrgefy.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gootzfwfu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gafqrcmcv.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gqdgvdzmq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/grbzzybib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtftrzdtc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtneneasb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjbkebllp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gmsqlnijm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gmpxpjzeh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/goigvwfrg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnbdxvjgc.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gxdwmivbr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gpkqtfgbz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvpoqnbm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmkmcpms.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/ghsniyyuz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/grocmnguw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gfgfpzuzj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gyxmimshp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gmpzsntyh.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/ghwnfiiyv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gtppfziou.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gmosvsssy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gskdbsbkx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gygfnuume.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gkusshkgi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/greyfjzrn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gcduetwrv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gjejhsfdm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gjuizfiga.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gvahrmmwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gibqemfli.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmppjqtsl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/griljavcx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gyphmpqfk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gwsxzjwtd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gylfzodnw.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gbufgvohx.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gensilior.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gokmvsnzj.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gvpfpgupl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gvkmrogcx.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gohgiotcr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gyctgqsyx.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gfdjoyaqd.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gaywltsie.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gtwdyjfyo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gactyqwej.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gnvnngxbs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/grigsujjx.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gjiiolpdi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gdmqysxmg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gzghzwvwf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/goamkhyks.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gqfzccxys.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gajtutwyr.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gcleeuebo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gudmvkwrs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpipedcpk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ggkfhlkiw.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gikfvlaoq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcvqatwba.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gwwgtmecl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gysbiffwd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gkimnxxtw.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/grclvbuit.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gxzwpsfzw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/ggoysjbbt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gxusywkxk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gpsjeaihi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gwdmndqxb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gljgxbkiw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gzkfyjldp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gwthsmqjk.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gziftireg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gehqczwlm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gllmlpiru.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gjqydcxbt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gflzvccmv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gmlvsvfth.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gsjbpjngv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gbtdytbnm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/glbhkxdbr.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdcfqjxas.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gdtflylbd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gmlvjjfou.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gddsrfjvs.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gefkeworr.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gtkrddibp.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/geywxwdvx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gwaqjfmcn.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gpvedxkrd.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gcqpvnylx.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gewcqpzfp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gtnlngwns.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gpcbimlnu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/guruhfldo.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/ghedmikzr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/goeocvwys.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gklkjpreu.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gobvipfwu.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gmlykrrcj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gfmrzeonu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gexxcatuj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjrogewjc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gdceifzpg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gewjachhr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gtnvnypje.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/grtlbhatb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqblzuxil.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gcxfqatrr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gqdlobhlr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gagilallv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjauaqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsqzczhvx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqtlvkxln.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/guybqcmyp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gqdlxgmqj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyfxwzgrz.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gabtmzcoo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gkuagesut.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ggdfzcumy.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gjfsnffhd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gxsicjawm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gziihwzhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gaqmobdnu.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gdzfxmqil.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ghtyhhbuw.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gedywmvfm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gdskfaafk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gdfkocfqh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxzjfjpwv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gmllqdgnc.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gdouxlfrv.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gjukcktqj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gfgkrorgv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gdyraidye.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/geqilgjdl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gzzvavous.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gsdxlwofm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gwxavirwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gxlnpxdqv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/guhgqnaip.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gsjqsjclj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gawolroel.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gbgalnmam.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkxoaoqdf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gjghzahce.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyrmtdoxd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gckgajzkk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gqbdajmju.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gwfesnavf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gqeoncauh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gufxjfaua.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gncghozki.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdvwwaa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gqnscljnd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gqazjjeem.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gdipnzjqi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/grfycdxhi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gsatwhuvx.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/goudjqqti.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gswqkbwpl.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/grsehopgp.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gvmfegbmu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/ggpeyqkoj.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gshhayhbd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/glogszfqh.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/glxydrxjd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gzciszevq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gyzyirbjk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gbyeewxdz.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gkjbeyesj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gpkxgxibo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/geqmaqiba.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grrmwebes.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gtssfmoaz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gwmhvaxtg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/grpeddgfm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gkbxelopg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvximux.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gzonjahqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gjzukavlw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gokicznpn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gkyqsstto.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gutrgnccz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gexfcbthm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqgnfxqtx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gvldrodnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gzedegzcz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gmeuswhuy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ghwimzhfx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gafwzswmb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gvfnrttbs.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gpdendjvq.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gfxgmxrfy.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwpzvfzpj.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gmhfqatlb.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ggtkpxpdh.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gazkghgxv.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gduwnxvkn.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gnibmqxgs.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gtdugcwsi.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gapuhndgi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxhikbw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gvbqirqss.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grklaalfm.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvjysukga.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gdncendeq.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gwgmpozse.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gqakdkbul.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gtjvikela.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gztnygntg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/golhvhrun.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gnbkvyvjr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/grvleueot.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gmtujjkoo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gnazzbfav.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gqkfhgfcl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxapoahop.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gozgnjrlb.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gudytxjbb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxuezkvxe.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gugybbkbt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gnohntlby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gcmwclosh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gkfwwlqhj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfstkbvgf.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/geubwfyhz.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/ghpxvlaak.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gbuvermgo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzbakqmtq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gfddzhprd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gvpvpoqfy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gzfxuxxoq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gbkkpppap.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gremymxas.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gicdlzera.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gcsofpvcg.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/geskalbnf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gtwzvrtbz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gdwccxckl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/guerpdavu.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gqcmhtfjt.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gfoptkmbg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmgjedoix.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/garnaxnsd.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gwknacyrh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gtregxyeb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gyxeatfrm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/ginskfqjz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gmynxqzho.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfqydkclv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzufkqoqs.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyxtarkow.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlclpulf.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gkpobdjoc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gmjyheclj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzenmtegm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gljueardg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gugqjpbtl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gaedhpeds.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gahpnocui.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gvwghyywr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gneclnsbw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghhstmxes.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gffcbyhzs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxcxgcwez.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/ghmvmlbjn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gleciwzfw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbswtejgy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/guyjhjgmx.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gvestqhdb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwuyafzsc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqvgzqqxq.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gmsphibix.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gxgpefdbn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnywoohhs.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gyzwysbzp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsynoqwuc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gfqzhbeyt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gqdehychf.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gpxelqxtd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkprpkexa.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gatktbcmv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyvdlziyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gvzdzwnqj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnkmqhntu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ginoppfsq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gqkgbaeaa.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gxtmjdfpn.sHtML


<!-- 参考信息 -->