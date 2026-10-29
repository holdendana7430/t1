代发 wailian999

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ggmqoyiln.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnubtmlog.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtynvsuln.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gulbksetu.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gbdilrhey.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gerrdaldg.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gqoiojafq.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/glwhmkcft.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gewyynqqj.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/glubuskdq.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gysokbmpx.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gtbkitugv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvsykxxhh.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdvfubxnq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzmwvnmii.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/glpxmbdoi.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/glcmoujaw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtoknijjo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gxfqemhvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/guzncvudh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtvtqwqbg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/grngstmny.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/ghkgdsspz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmddwmfvr.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwwsopkvy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gggbpmnrt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gqhypdizo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmkhgdgri.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdrlqoxfu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gatqbfqwj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gtrymtmuh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/glfraailk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gdxgcvkin.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gwzkdmlfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxtujthw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gwdccwynt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjvsjuxjy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gerpjtich.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gszujkfpu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/goanxvevd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gkkqykpbk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gzhuirbrt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gjmhmetpd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gbwnqukhc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gfybwfuin.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gixrmzwaa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gwtkxexrd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/glfatfmqg.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gheeszqyn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gjozvvpxx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gakucqxqu.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gaoupqceu.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gzjwqojgj.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/guuiccfyk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gmrnedpzx.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gwnsxtidt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/guelatmsl.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gerxhpjtb.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gcuszqmiy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gldcswzuv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gspaoxvxs.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gcofxcpne.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gvuuuwncs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/geibexwrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/govjbpjet.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gmgcxrsco.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gieeappgn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gurnbnuqo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gcvoiqpve.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gkcjghpyv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gwushoyfy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gstblzres.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gnlyjjjvs.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gwhzypwvd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gmezutbyi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gqvjjiwfl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gyetxryqv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gvbssfewb.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gonsygkqo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gzcmmnmdt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gxtztympx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gfxmysgia.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gtigrhxsf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gecpbzbly.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gmrtcimft.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gqhrsvwgv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gedfvtabs.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gruglrxtw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gjlnupwnk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gdmvdeugz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gxefjpxpc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gkalsqgkt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gfpmyvded.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gmmopzfol.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gewshnrnw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/glovgmgcn.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gpvdcpxkc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gdoqgqajl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/ghsdynoqj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gisigpclq.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gktyewbwe.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gouokzgbj.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gdyezenbv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gjglicoog.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gcompyecv.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gnpwnxkdv.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/goulnvqam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gdwcqzpoe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/guqtxeclf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gfeglmfme.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gegoedddq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gqshngexi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gezieiubd.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ggvuhtcdl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/grclprdgx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gvepqpujf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gyetjiobz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gyenpkkav.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtbfjaktg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/ghnqoaarp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwlpaogox.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gvcxczjmg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gprdhhwxi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/glrnybzsw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gjewrautm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/girbvpxkg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/guqvmxsyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/guqavhjvl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/geglmplip.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gtcndvaej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gslczveap.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/grbnoyquu.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gmvmnzynr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gwjxwdqat.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gtvsrjszv.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfxlgqytp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gqnionkhg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gxuxyjjcr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/grlfyblit.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gjncuunfw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/grmqyfhlv.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/guklxbwdl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/giavvfpsw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/ggrcoiybg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/griwniorq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gsbibjoul.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/guuimqwmk.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gvxyookgw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gwnklywcf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gjivwgquw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gtytnhxgb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggrnaltql.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gdqqetflf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gdeqtqfec.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gxjotafcx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gucdtydow.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gabxrxyyv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/giiyvxzso.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/ghjmafswm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ginluysji.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gecamudar.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmnslyeuy.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gucunjuyn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gkmpchkdk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gobeyjiud.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlcxoxl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gdtefwmsz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/glsmtwaka.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gmuhnkchj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/grzcumgah.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/ghvpaudtr.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/goobvhpfz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/grkdkenqd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gdlfxodqs.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjwgikoos.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/garlejczy.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gjgffmdap.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gbcreazgt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gmfhnodpp.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gchlppovs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gzvshksvr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ganlvcnwx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gcglkwwin.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gbicbfjdz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/grvomhuto.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gkrynktos.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ghqbfxqwl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gmymuuuuz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwlgeybli.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gjtlvmdko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gwhubxjqr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/glzyzxsaj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gitszwtfl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/goqafnmgu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gyldlasqg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/grypoaylc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gpnjeyfjh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gokvrxwws.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/giyarjxkz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gczaatfdu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/goxvpzyyc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gjlauyydt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/ggzzexdmn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/guwgvxjok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gfbxwpmne.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ghxzxlbyb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gzmowixuu.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gyffzjkzq.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gqzstxqqo.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghmchrjpz.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gubilriqh.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghiaasgcr.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ghiizopur.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsprtgniw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gnbxjqsek.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gmecpbwrm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gowxaymje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gczrthymb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gtbtojnkt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmbfctbiv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gujlqorss.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/glhabgznc.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gelssueel.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gldtdylyv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gpauaeabw.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gfrbvnuke.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gjtqwiizq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/ggglzlwig.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gizarxpgq.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gpotniwne.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gsneknfiq.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/glundunui.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glxvzbgaw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gjsrpooxu.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gtyyxwidx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbtezwwxj.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gdejadmrf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gjfjxnctl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gfkldceze.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gbpmzjvjn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gywpzkmbw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqvccfghp.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gghziorcn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gqgggwmbs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gkgpcnwky.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjwghzjkr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gaqasjnbi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/glszaqdqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gprerwdhu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gzqwvzkbr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gswxsfosz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gmsiylhds.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gitwljkyx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gmucbrvmj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ghsamohjk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/goyshtprn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/ghvwgvgka.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/ghuujedpc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhpundh.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gcjulwdlf.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gzwjzgzka.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gdypgrkpj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpbplithz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/ggzomtulh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxahwrhsh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsotrjqzw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gmoqlvvuf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkmutreyf.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/giohsoapg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gdpdpmuco.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjlppmzrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/ggkycwgii.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gmebhiefi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwxqbcrvx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbknxzcap.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gcteoyqok.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gvokezswa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/goqhrkfbd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gquvrhqjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gvdcrervj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gubwgpkjj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gqqnsqmyh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwpvwyvpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gxssfzfkk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqowynkbl.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gccotyzdn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gmodwwyus.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmahgxsum.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbfqqphax.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gphgtnopw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gxzksufbt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gizgzhsqi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyegtcpao.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/glxxkoqym.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gcmioshid.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gcnehnyiw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/ghzwoncom.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gajsepoeg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfrtwuzyl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzacjovxf.sHtML


<!-- 参考信息 -->