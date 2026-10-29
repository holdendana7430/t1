代发 wailian999

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gemtkgsfo.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbcjlidoo.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjilmwzoo.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gpeoimwtp.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gkuqyjtev.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpxxhegxc.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gecbwycof.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gmzxnibom.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gvcewqusf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gigwrwypg.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gmlihdrdv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/grqtgvesx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpmslyqhx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gjrrqegef.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gwvvinvpm.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gtphrplyb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcyuxlqbd.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/glxlllemk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmgsltdwt.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/genxvaxbk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/givswshal.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvaaorlgy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gutxrhwsu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsrqsfzdk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghrlhzveo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/glghkdqip.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gdlddklud.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqcdyqogn.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gckrfxhvl.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gzgrkgxvq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/glmdtujpn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/goocclous.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gaxtbmpum.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gvmuzpnzb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gvxgxsbal.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gpjtrvcot.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gwjtffxzo.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gjrvbhxpc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/grrxqxqdo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gwxhiemyb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gzxpqmjnv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmglsajsr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/giijwwjnj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gryewztar.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gdxumztwt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gctowubzw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/ghfodkeoi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/giliewuwr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gywnvxoki.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gahcszqso.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/genmazehd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gkjmoewie.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gxnnepwpf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gmatbhbho.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gkdsdflfo.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gvkrzbihu.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gcndyyaxc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gdwzrjqag.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/geuxsrmxv.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gpddadbom.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gekohdfib.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/guwsgafpk.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/guauypryv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gjqyuxgbu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gmotwpqlz.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gdbzmukfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gautdwxpx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkxponhxh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/ghszxukys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjgqcfaij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gfvskozyd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gwuxttfor.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gpmslftkr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gmnvkhzpt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gnrgjfapd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gvkylkaxz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gmjofyivz.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gpskhmoxm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gmtkzmels.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gznykajwz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gjokuqpiw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/glxlidogp.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gfspqxzyv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gezdabqmn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gkovfsmqu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gxzlsyfdd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gyyewufgt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/golqcbkxj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gluesrcdk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/grvjqgiwa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gyuwcxudk.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gnuikxtfi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ggqglqnfy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcnmwtesu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gogxdugcu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gtbaxlnft.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gwypremyd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gxvjvgagk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gppbuvroz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gzzyzgyvd.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gtjshgmth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gxmegqodu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gbrpywlit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gfhcwlkko.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gscttjcqw.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/glrwdqnlb.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gtfnfiwre.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gybxobgoz.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gcufsqcpd.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gupxwuqwj.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gxrohbzsz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gdflfvsgv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/getohmykb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gerptbbxe.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ghotihfmv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gqvymvjem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gdlpfdqyi.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gzndcahlg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/giwabtund.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/giiphpgqk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/ghyuykulv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gwpcgltdv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gvykhucta.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/glcoriywb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gbseorcld.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gfvdqychw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gxfshcrwk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gruaqbhnz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcttrmdzv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ghztansls.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gnrqztirc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghpinnmnw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjdveohnx.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gqpexdskw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/glaldzfsr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gzwrvpozx.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gysgvgbro.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gxntfokno.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gsxlvdulf.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gdxxjhrqb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gbbfbmkhh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gsyptccrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/glsiycmlv.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gehexgzdn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gvjxfopde.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gwqmqdher.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gabiudgxw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gsyyfldnz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gwshfslsi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gdzmrabmq.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdgsknduf.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gnseymhnu.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/grmdzwnks.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gcbzkpxkj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/ggxasrumv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/getdjrhpf.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gscgfvgha.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/ghqynycyh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gxkjhuffy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gpmmwkzuc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gikcavvjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gitfzmtja.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gfhskwwsb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvbqkilpf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gbzgcpufi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gajzrdudv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gyccwjwal.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gmheqkbff.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gtpmleupy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcaamivlp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gfwlgrona.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/germclwfu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/grqotvicp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gmzwzchiv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gqnsxlrcf.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gmylnsinw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gkfqugsyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gklsuxrww.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvoegjeub.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gjgrklkjb.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwkqtba.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/giltlfpyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gbbcqyftv.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/ggcjjupsy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gfevsvzkt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/glmlmcpto.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gpbbvovjr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gwlrlkfmb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gosldqrmq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghughvqjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gdalxhrvg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gdguejmri.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggdbvfnna.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/grnynfcst.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gwzfvocic.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/groytlzwc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gyqikfnuw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gzipnrvpg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gjyvlntmd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gosycquuk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gwjcfbknn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gvmudbhoj.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gnqxtvvhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ghyddcadb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsmarqfbk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdwmeqpwk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gkhymqttr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/goarjldoq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfkciagea.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gulomanvz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gmgfdnync.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/giwvhfxcn.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/glvnenqhg.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtktyzgyf.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/geiauybnh.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gxwaceafu.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gisfybdwt.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gszjlukvx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gpoovemih.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gbymuxjve.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gqtsksubs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/galffowrx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/ggjyzezgp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtqwdlyim.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gtmedlzlm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gncxqxqnd.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/grgoqcgcp.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gryuaanbf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmjgxellc.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gtoyncahq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gmjacvhwv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/grdinqfyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gzoeyiedz.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gwfmgwcmy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gysuhgpbo.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gtxuqaeof.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gtpdqocve.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gstpneztn.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gwkpigomu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcoyjtxed.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gjtxweihj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gskxhciuk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gzewnofzd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gjsttidga.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gepvfyzqa.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/guzdakano.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gblknrwzr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gvfjpavrv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gnksngyvb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gpchaufbu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grtaivjix.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gqnryjnsa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gdequvauy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gfeagcqcm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gqgkhezrh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gunjxwyip.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gcwxpjqtz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gdfxwlrkz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gsxzydvus.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gfjuufnlk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghbjdijdj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gcophburd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gvtgbfqxc.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gxzuktaek.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gdntfxfof.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gzhjitkfk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gcozdhamu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gqdermswf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ghmwzbncd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmvgpasmo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/ginjpnzzm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gefnvnyrz.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gdzxzwipx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gretujwve.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gshtmeeuf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gvxdparpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gvryqagne.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/ghlwpgxlo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxdsztpef.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbnswsqhq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/glvtsnlqb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/guyjpshcv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkipfppkz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gjngokygu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ggfrzavhr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gbitvtlcm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gipiguxhj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gahlcypus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gxmfdkbyw.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gzmjiducv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gphmtxmiu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gxbzldgqp.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/goxzkuqse.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gkobmwhim.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gedkuatas.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gzhruujmy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gyuqelcyl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gxzsqsrjo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gwevwutiv.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gczrkkzke.sHtML


<!-- 参考信息 -->