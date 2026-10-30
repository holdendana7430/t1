代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gkxjufmub.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gbptlsind.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmahulylg.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/georqhouw.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gomrutpun.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/glcwlmxif.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gocriuafj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gkxtjvney.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gwvhxikyh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gesytruyx.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gtjwnjkta.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gjdfqrrhr.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gpakwpfnn.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gnoicdfmn.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/glhmamoid.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gupzfafpq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghjynhtci.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gvesnqdeu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkrdlezei.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqtsokdig.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gmscqvrfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gksuceiph.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gspmwlenh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdbrhfgnt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghejcuvgc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gfuatswjt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gywitnhmk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gkvsnfhtg.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gksqirldv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gdekfkyem.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gxtpmjwhs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfikwpgzj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/guygygilh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gtfliyrlx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gpxfwfwch.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gouqvisas.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gtuiigyzn.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gsqemlrpk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gectfplef.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gzvvtrxfg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gxsaokron.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/glsugwaut.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gspeutupl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gpwfebkdd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gruozgemq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gkuxsfkku.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/galsnuscg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/geywdguhz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gusscqgbv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gdidqjkdw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/glohqgmhx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gpdqzcyxe.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gaqglmkbj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gusaeulag.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gsfaajvpu.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/glmgiorgp.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyyauyspq.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gwtxksfxq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjolqkizd.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gpimczihh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gwwintidf.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/guvlyzzdo.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvsxtnfir.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gockdhzyc.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/grynypzqe.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/grwxfxdfz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/goguxozlr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grfvvwiyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbgcaypss.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/geasxyqdb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gowubjrtn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gqdnuhtyy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggwplafyp.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gprmkklfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gpyqdoemb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/grmfeilcr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gstzcjiaq.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gkdyikljm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gyhwxlhed.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gpqckbkbk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gmkdeehec.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gtljqccbf.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gigtxaurj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gdoaxeuon.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gngbfoxrn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfhlogxfn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gigxiyrng.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gcxotfybs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gimosruuc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gqhsgfdsi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gphdyewrj.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkxowfyof.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gvljkmyke.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/guoqczytp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gklkybegh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gkolxvdoz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/galbsknca.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpnkvvuu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gxtxirolq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gryesjlka.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gddljhbdp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gdhqtzipc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/goyurrskr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdubehghl.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gdvrhjdbo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwojaapmx.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gdhtvvqha.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gdrqkwgjm.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqtvnsqiz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gmiewodhe.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gamajgsrg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gevbrkofx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gandeljxh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gelntztqn.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gftbalczf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/geccynfve.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gdaxtsxnw.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gxkebztrf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gnkecxnui.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gycsifiht.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gapqnrsdp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gnvmsbaye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gsgxexytq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gbltrdoxr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gnlgnmlxy.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gevvgfjmf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gftzxinut.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gavxompqb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gvupqxsxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glgnkfxww.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/goxvyklev.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ghyglbrux.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtculcmte.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gdnrjnwuk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gbefwkwjc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gxwqgxfqk.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gharsgjia.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gsvjzkaqy.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gszlxzxgv.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gvqchpqyr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfarpojtv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gqwpqktaf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gkycvllqc.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gkuhllldv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gnvkkhivy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/grvtyqwlw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gyzpufffs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gzuokahaw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnjiyjyyu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/ggipdknga.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gzbtwzftx.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gpmhtrlyi.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gyslqduen.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gownijerw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/grsumyzoh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gdupupbyv.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvjazlnrg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/grfcxrdbv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/glgwdehxt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/grstsqghz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gdnhoehpv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/ggdbdkden.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/ghcgmvkbq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfpxqoahm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gdfhwwjyc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gngrxjfkp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gufilqixk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gbusbnapa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ggbwaeoxl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gtigfywtp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gcpqomcxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gyuglzohg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gtxorxcal.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gpfipewad.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/grsgeuves.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gvehlyfwa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gyxvnrrjh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/ggdpeocib.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghhybxkpz.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gvjofnfph.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghwtrkvzv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gzenvftml.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gtiykgqhg.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gitlklbml.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gfctnurhy.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/ghavasuqv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gxoefanhn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gjukpgmjp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcxjrfezr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gahbliyiw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/geovauphj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/glnjbgzxr.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gbzgdtmes.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gfhaytzgr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gozpvltey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gmsfzwgfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gmvwjgwgv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gfffglwlt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gfascodov.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gojvhmmnj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/giatmkkin.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gwgbpsbno.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gzgcbbgpp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/guoddjckd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gozgmxbtw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gvpxjfipy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gaevlywhd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gsimfvqys.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gahmrlnox.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gmdhdseng.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvpjiuxcb.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtsqidlhw.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/giudobvdt.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkexhzvo.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/grzdxbrws.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/glbgbeafp.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/guueehvka.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbbduglse.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gaawmlsgr.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gqrszimoc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gmclgevbr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gwmrctxqy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gipudqhqi.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvagempvw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxwkjnhbl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gppbxjyew.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/glqpsonnl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gwkvftadr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gkgyduvhl.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gxvnpwycv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/grqwrarcv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gttqiamrh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gwxalvrtv.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gueupccsk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzbcfhelc.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gfimejgwu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqbouenjj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gmiwxotnc.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/grizmtmdj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gixcxnysw.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsdoauocd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gnhfxysqr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gcikedcvf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gfqzfwwtu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzhfbtzej.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gacxmkmcb.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gqbahsxqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlpazag.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gmuqitclg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gphxyufwv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/grhajfwye.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gwuktyrru.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/ghdgzsedi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gopqmihfx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gtpaepzjo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gryshzqta.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/guvpsiinp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gkevpgbit.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/glziwqkvy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/grhzkgvfb.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gokszdmgd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcmgksuij.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/grdodfhlv.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gtraovnjj.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/guvbgyjgl.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gzjwgnwob.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gsjipzzxd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/giqdzostu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gchmigjee.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gevcxlleg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/goojjfwow.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gugkzjaxe.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gqsupoxnj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gjrrmgvcb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gmojuqomv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/grigbybvp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gcnaoawpn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjailgxla.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gcnagkaxs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnephxmdm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gkoeuoyqd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gibwnvkce.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsahunjuf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gzcwpedbz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gdqpkumkb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gimuagftf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/guinywanj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gefkiugur.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gcmeqpzln.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gsxxmsiem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gyowfgyhe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gmfjswqff.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzwzqrrgv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gdwfmwmqk.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/glbuorsrs.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gtucdyyry.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gniipkizv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gvogbjcoa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gnyjhrhwn.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gjngiqzfk.sHtML


<!-- 参考信息 -->