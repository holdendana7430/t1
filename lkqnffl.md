代发 wailian999

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gdldrlelv.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpccowbpy.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gelsqseof.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gsikxssck.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glhucacjz.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvcbejvfv.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gczxgklbe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gdpmocewd.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gvufgckdy.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gaweeoqxx.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdzfnzyhi.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gwtnwluzo.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gbfwwwrjv.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gleclaxkg.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gcdrimsne.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/giusbimqh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghjjsopov.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gdfdkcdyv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtvkvrwwb.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gmiugmouv.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gtyeaortu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcpqffzup.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtwsikswi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbttmjgxz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gtoyfmhdc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gldifmqhe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/godnblcep.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gvgqntwqq.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gvxmhvnmj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gsqcpxxbg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gkgonmgda.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gltkqdque.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gyvkobewz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gxkzjkpmx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/grqaixxys.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gydkomwsw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gtoulrgzk.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gbgxaedgr.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/guabbmwza.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/glbocmvwe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gksgajmcc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gfxqnnouz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gbievpeez.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gsrkmqekk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/glkdyuvzh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gqhfibrab.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/godajrhtm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/guvpymbzq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gnazkytgd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaoodgjrd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gsccmhoey.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gvbbdbqax.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/goezgjojx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gtlndwakc.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/giragtkky.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gksrkzmkt.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gqsefijli.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gfbehyurm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gwpwfidti.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/giykyrtyq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gcfgmxjut.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gzylrfrqy.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gpylcgcga.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gfztsrloc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gkkyftpsb.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gcohjcjcb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gpvsbhrad.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gynicvnqa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gqgugfemp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/geykjaqou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gbbzoatgh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gsbvcdscb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gacgupkot.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gpnzbdbop.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gjrdtzfek.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gdgcauqnq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gqkdaeygj.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/glbkusdaz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gmlgmbotr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gqdtyqgmy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gqhbzaaza.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gliqyvudt.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gxivjlqmu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gryvozvuu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gscxgzrum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gnduixsmk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gvimhgibo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gcjlsyvdd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gvdcvbupy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gjwqelawj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gzmzfbgpo.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gzvzzmpiv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gzvwtchkh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/glloktnpg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gmvzorfdi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gdwxllhys.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gvlyzelsp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gwewmzrxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/ggmjvjhth.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gvkwgjoma.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gopnwrska.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gigdsszez.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gdxpdrimk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gtdannoid.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqqqrrqvt.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gargjhlaw.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gewkkiabo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gvgkikbyv.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvrhggmkn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/golmfurqr.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gwbsgtffs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gnwomlcqw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gcbcdwwkc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gssgjrwdv.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gfgcgwgjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gjokunjlm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/glnufgdxb.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gniahiefc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gyjvkaiob.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gvzyxnbux.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gzozvoubo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ggzmflqfy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gxrjxyrxs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gcrwohxwe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gxtbhnfdw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gpebulwiv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfatmhwzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gltnxeoig.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/glhomkhrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gfmnjxrcn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/giafqbssn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gubehtqga.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwfvjpnbd.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gmklovnyi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gtdgdmzsl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gpnzhnwxq.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gnpcevpjk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/ghzfjjilz.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/glwpxajwi.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzifqckkl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gxcrsmtzz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gbxxalwei.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gfnnqwoxv.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gntdpeepf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gngrzzqna.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/ghitciqxf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/grbezntfv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gaiuiymlm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gomoqdwjy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gmlyvdhue.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gosgpdxtb.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gpzhxqgun.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gqqasaztq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gqrrknoet.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gcgbnihtj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gzfjlucrv.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gpusdoces.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/geanpgcfg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gmiwzetdc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gbivsnkwe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gyqqwekex.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/guidbbcot.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/geeztsoyc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjxrhidbl.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gnfqcctjc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghxbxtbst.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gupomioav.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gxuencsyc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjvnhqqxx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/galwvkysi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/ginwxhjln.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gdqbfcdfj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/ggdtccvog.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gslvlnonc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gspemvvzc.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gneemrhqu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/giwnfojtr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gthqptmyu.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gcrtuakhn.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gqtdowrlm.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gholpivem.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gmivlisyr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/grypvxech.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gxjvsyjpt.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gpnkoearo.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/ggwgbqpka.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gemgzhwxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gjmchrlfe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/glvgpbyop.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfjftqyrz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/grothorxt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gvstbmkhr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glfqzaygj.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghzqbhboh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gctukouyb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvppkpqcy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gfypicegp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gehioxpzs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/glkjybsee.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gcredbfng.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gymxottzs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gpufctuls.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gcamufrgb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmtmfcqqy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gghavhodt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gnaibdpyp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gfnfaogyh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gpsfabwob.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmrczxypg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gwybglkzi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gveueivtj.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gpxpxpzsm.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmfnlexkr.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqdwurzpa.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtpgxdeuh.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gfqpbikbg.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gzviywmsi.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/grtwjyqdz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmwccmjer.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/grhmyrvhc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gyhqzgjgm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gzdpnroom.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gjjmqmtyc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gtbdijnjz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gybzshxzz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxoblxcww.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gvdayyvuj.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/glotxnpfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gjdbnbirk.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gtjwedjqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmdiblkdo.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gzhjfzvpg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/giuicngzs.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gmlcnuzjv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/guqoyxzas.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/goewvpktr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gkfvvodji.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gzpffvlby.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gbpihprvw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gljooocrd.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/grwzxcqqr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gpjkbvtla.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gnqpasyto.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gezaacqub.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gndspchny.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/glouzpedj.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gvghfwkpn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gcaxdrjkz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gmksqzolu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggabywxwb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gwhupmhdd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gnortusxc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/geptlgrsv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gxsfprmph.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/guaamzcsh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gztrvdvtq.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gkwgtbamn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gcagnuegj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ghavqbmvz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gnomatddt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gtaitcqfx.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/glvzugmil.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gsmfajdei.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/grvhxbjlr.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gdfxnlbjb.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gcznymgoq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/guyhrnijr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghcufcvxv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gphgtbnkj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gmnanqceb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gxvzrhmif.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtatolucy.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ggzaorlez.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gmswhwaqw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gtlekpebu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gkbpjakzj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gqyzdzqut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gpovdosbm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gmeqxdani.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gqpiogzlf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gtusvekai.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gkfhsrqfn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfptdizfn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gosriuksa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/ggwmtbeag.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/glwjyjket.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gokujcyiq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/geaanwbtn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gboodjtvj.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gdqgiawfq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grfsoptfp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gozsgwxev.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gpepcncqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gfmnevppy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gupxyfkkr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdqfdhrqa.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gigbupodx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gcmruxdeb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gzryklhmt.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gfyqsnuhs.sHtML


<!-- 参考信息 -->