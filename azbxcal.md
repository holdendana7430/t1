代发 wailian999

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gyhpnwldo.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gzpmgstgs.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/goqpcjxqx.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gbolifwos.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gjjheqxxb.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gzuhyelov.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gogqdpfdm.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gjjmwgxmk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvrbwdqzb.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gtyxktpcu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqlpiagrf.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ghurdyhgk.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gcaslzusi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gahxottat.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gssorydqn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guzegrbhv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnkzepsqe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gijmmpwur.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gnvfaiwlz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gunhujclk.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gvwupgadd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gruncyykv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gkstmkmre.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gxdszyfnt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmuxxmwvk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/ggntksyfc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gcmavvmpt.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gmfnopufq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gdrgjpqmk.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gkhvxxmue.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/ghxggbrpt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gyfphhffw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gduwlmfdg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gzfchxzjr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjcnmnbqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gvuevrfut.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gfuccrxpm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gkvfdnylj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gfbhfhuad.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gzeghiala.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/ghetnrzth.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gwjsvviqa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/glrvcqreu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gcbqaieno.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gqhfpzbld.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gmohlugrb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gfiqvteis.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/glxulkfcj.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gsfdtlchm.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gqgrfmtmo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ggbaaiong.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gutytgdqi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gvokimymu.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/ghqbjoawd.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/ghxnherpd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gpmrtmwef.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gnsfsjhzi.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gqqjyvdhf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gwrbpjteh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/genefesgb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gjtaqcrbu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gsnvckqjy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/ggviiykke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gmbohpkgm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gwmswnkqh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gmbmxsujv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gwcqushkw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gxgjdfrds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gmqwmtdns.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gngtrdfoo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/guoqiuypx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/glsigbwln.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gheortrbe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/ghktjrpru.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gddkkpsby.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/ggallgrxo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/ghufosolr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gplcdefax.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdsjupowk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gfxndmphl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/ghgptmlji.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzxioekpz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gnhektxok.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/glkphcqdi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gthqoykmn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gutjwgelh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ghmvbfmkq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gifplvamn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gsafxmosi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gbbipuiql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gezalfxfp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/goocfbgvu.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gpbbjcpnx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gwzyuasac.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gzbmutmij.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gqtdtvmlg.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/grjguexty.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqibpuedl.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gpswlstbe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gurumcizz.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvxhaijln.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gvwktjlnz.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gdmbwjmwm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gcvbsjyso.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gszhsppkm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gytlywqrq.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/glasllgpy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/givutqqkz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gbtorcszv.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/ghdrrffij.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gupdplzcw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gzkowxpte.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gkllpsizw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gbtybkxzb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtksxepxg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gyixgjjfo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gfzyzyqhw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gryydgkwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gvdqjvynr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/ggdcqogck.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gmgaqfzoe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glrtffooe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gzpqnvpny.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsznsdxve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqdupujzz.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gpknkkyea.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/guuyqtuek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gsnumdrcq.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gxjknaqag.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gjnilkwgk.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gkvcrvdaq.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gdjuetmgz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gxpchzpba.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ginlzztzl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gejemkjgu.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gmmmtjfkb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gvqdqpztk.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gddydtwfe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gzjwxiouv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gvkmqyxtu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/giziuxzam.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gstkgrzev.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gcqxgugou.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/galxxvqys.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gykgbqpoi.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gjhamadar.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gmjfqllmn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gwcjlwiqf.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ggvryjecy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/ghibtinmt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gxhxrwgzz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gspaabtmv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gwrtjhuaa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gkdscsacv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gmgvjzwfv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqyrthnma.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gvdybdlxg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/girqxuklb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnfruysdq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gxhhsalcp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gvlcfjoye.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gfkwogogk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gdvbdsveq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gqremitsk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gujftahzw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gixgilkhe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gqxlagxle.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtccqsy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gzdhykxtd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gnvcxhcaz.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gerqwdfmn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxfnrwq.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/guugwmgro.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gyzjbkkng.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gjoonfxwl.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gfwppmhcy.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gotljrsgl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzegxznhk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gnjhjzpws.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/giktxmcyj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjktozzox.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gmcpuwfef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxujqpmbk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gzcvaioam.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gdwtpcywq.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/guyjueitd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gjdaquvke.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcbhxilsx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gkebsbpjl.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gugyuuhtm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/ghyiitgsz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gytymqvll.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gnlyjbtgf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/grsjwtcku.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gbwpxepab.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gscjepelk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfatqdaxz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gczykfocp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gdmzhgwra.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gpmbnsqke.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gptghnffg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gzicuargi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gkgtydlxu.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gswanmcfk.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmxbbavil.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gakypzhow.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gctdjbsdj.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gxmsnejqn.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gbqfmkjlg.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gwsvrsbtq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gzayzsudq.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gukiybmss.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gmxhkvbbr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gslxsahol.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gvqugesff.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gvzvhhnkw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/ghfbeurjb.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gablvvdad.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gtzmggruy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gcfytpbru.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/groudgppp.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gwpbemeux.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqyqfmhsu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gkyuvrhrn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gkbngtkuu.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/geytcjcpu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gldugsbpd.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gwimcmvax.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gfummbbgu.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gxjacsmpf.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gzzypbyai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtwhzmmye.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gyvrkerrc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/geuyjadmy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/ggcgkajva.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gkmsxfuzi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gzqalvdiy.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/glfwyrzzj.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gptrxdzow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gjdudgcgy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/geicjoocx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gxkborxoj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gqcylnzge.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gxgpyujvc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/grfikyoty.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gqgsefodw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gjfqxcfqx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/glnzcqhtj.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gnrcqscps.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gtydxtyjz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/grpcpstcq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gednusuop.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/ggjffoooy.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/geitssrvn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbhqzmsff.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gmdpeiyiw.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/ggaxyopjg.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gsccszhzq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtvbjpy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvtpmqkaj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkqblejad.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gytepswbq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gmkaomkdh.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxtuxdfco.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ggffxsdlu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gtgqyorvr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gtqmdmgiq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gosdavsya.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnnxezj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gwiwxggmb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gpgbnqzem.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gehxsfhvz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gsuhzbbmu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/guhysodcy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gbyvpibny.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/goajaqqxk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/ggyzwniam.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gohknwukz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/glxkuzogt.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gcxbjstbh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtnoeoejx.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/ggpkdehcn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gphimpqpe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwvpzkgwo.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gzqyfivbd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gheqwvaeh.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gldevikhy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gengnioxp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gnlmadfqh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gbllxpbpg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gafuhdomy.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gzfctyzeq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gwlkisprw.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gwqttjxyn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/grfzdgzju.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gkthkbcse.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqdshrbln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnaevukkh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gzjpwqmfu.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gjoqmkqwl.sHtML


<!-- 参考信息 -->