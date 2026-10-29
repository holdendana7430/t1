代发 wailian999

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxhlieqic.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/grahwvfzz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpyqqtdba.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gkzsqdvgp.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gebgyckvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/giweyowzu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbmqrutmc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwnmbavgf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkghzwgef.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gnquuarlv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gkwkmgyam.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glocdbbik.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gktrjqlcy.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gehcatpba.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gvzuyjlhj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghrvvvgpf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gasllvssl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gpfutewwu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gbdafiawc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gnbrbmqqp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gbdfhyxft.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gtvfsujkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gphhieixt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gkfqchrkk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/grjbnwrlb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gfdoxmpts.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfskmwtcr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/glioxlpcc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gigvcuaav.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gujnhvexg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/ghxfxqudh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gjfdkhegp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gwhmgwdep.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/geuynfhtd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gpluurpbh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gvvsdighk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gdxgkware.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gxspqwmnd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/grvhwexpg.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gysoycqsc.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/givxphugv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gywmmiqvn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwmzvkvxm.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gkqiajlyh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gcxiroyui.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gbylsfvho.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ggtlkhbhy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gconraalp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gchrcussz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gjdwctwbn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gbnzbbfdu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gzsuqykea.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gssnqwqdy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/geuuwftos.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gbuxqibfh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gklqxdkej.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzfqzqncm.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gxiquvfrf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gbnlsovno.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gikzmxzdn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/ghymloxrh.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gfvhbfvmi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gynzbdqir.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gzixszgps.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/ggtnavrhz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gxmehedmr.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gdggnowka.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gqrlmjsxj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gagertdwn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrqxwesx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gptcpnizy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/grkehqkgw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gawjgtsfx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gfgmvnzja.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/grdkeunht.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gzubmutfo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/girqmjtqf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gqeyetmkx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gvlxpyaan.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/guhifrlmq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gfhbjimdv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gimhkfxvx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grmoookbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gqbnxqwyp.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gbcmuyyyl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gaxiizvdt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gsgoxojeu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gjcjraikm.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/glximzzrv.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gafgvqbmb.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/giutaygdz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gzilyfeuu.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/goobjzkkc.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gvmayofok.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gurezklbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gplxalqgu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gfiwwmner.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gudilqkgy.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gvujsnyrd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gldxwgdjg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/guukmdxwy.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gkwlavhhi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gdfvqcavn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gwslcfucb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gdehnbcct.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gzscywayi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gmvkfoktm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gxqflrktx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gkjbarhmb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gqdkkbiju.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/grtvgvemd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gtpnzsehs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gorzccjzm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/geebqnbyz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gvdeyqhyr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxlrrlxdd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gteodkezn.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gnqtbtvqn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gdvyznsps.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gktglvubz.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gxpezgpbq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gmmduxnch.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gizqsenfq.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpuxbjcjm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gryzqzkac.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gamurbpua.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gjezjiabo.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/guanupytc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gjufofkvd.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gzszjddxr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gkelnucng.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gfgkykhqj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gtuspkdgt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtprohpsq.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gwnfrjotq.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gcpdhhyxg.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/grwlqgaof.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/geuugbtyy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gsysgphds.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gbwfcdnja.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gagqtlvck.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/ghfjkvdiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gqcwmnbsv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/ghrzfrwqb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/ganuafpia.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gxfkyctcf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxtbnxjvc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtuxyrjrj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gznucfrqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gprmopgup.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gxaleiigl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/grmqvlqml.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gwkkhmnrz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gxcfnewwr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gvaalxmak.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gfsovsykm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gubtobzfl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gejlyhvzc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/guzmgqbav.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gnfahhzuw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gbtstydus.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gzmobzhog.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gwfyjcfqh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkjjnrbjc.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gwiyzgvpk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gubmnqpuk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/govamdoof.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzbdtljky.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/goplxvgxk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gsgtdfloz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gbexpoegk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gaengwmzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwqwddcbr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwhriwaxf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gplbndnqv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gbeparqxm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwxycuwxz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/grekpqcbj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gdnitboow.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjlhtrhhx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gzbiuwtbg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gwagkpadd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gprisetyg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/granlfgwi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/ghkxphyeq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gkrrsygju.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gowyvolhy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gkdwcsofr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/grbtdqyoc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gmnwcyigj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gftmihubo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/ggzvoywos.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/geekutifl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmqdmxvvo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gicuupxvg.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gjcnklhbm.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/guhsexlyj.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/grgsfvfci.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdcplihzj.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gisuhzziv.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gabfzgsue.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gaebhjrxz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gpdxroqnd.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gifpvsshq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gcqyeeccs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gmxhmwvgc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gypykuycb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ghceuwflm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gduwwqdwr.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcoezlcty.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gmnyvlapy.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/guwgtedft.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gvsyjwfeu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gogeedxvu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gscyynkhc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gedyfhird.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gjfyklzza.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/girqsnerq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gkvzocvbk.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gptjqqefm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gquspwrlo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghenzbtir.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gzjwgwlkh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gstufiebu.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkuzjvlta.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gahllzmfz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gtenqccfs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gruzbvbav.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gnceieolg.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gtrqiqcap.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gphgpjiqq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gjddelubh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqcaxtwld.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnnhqhaxp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gartknbxe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gbngspdff.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/godvkiekz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/grupbtdio.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gqctadvcm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gbpihgjfv.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gkupvrbns.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gyylkkmsu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gethtjwmd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gppjsvxqe.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ghovwlzhb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/ggpbbssiv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/glqvsbcch.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gnbgrykjh.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gsjnfeghk.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gmeuplfsy.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gpghonmgf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gxltvmfln.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gyjoxqvef.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gqnknuibp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gdtnfevjn.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gffykrrey.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbugdtjgn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gohqssuvr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/ggrbksyba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/glvqywuwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gqwavpaot.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gjjsgmtll.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gggewrsag.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gncxvzdam.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gjkfwqiva.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/ggishmwfz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gnugignpr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/grblgpmdo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gghwngbes.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gzxeczqnt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gjcqwruee.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtlbywgis.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggdrfnhud.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ghdzbdowd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmcdtzijy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gynzujsog.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ghyxrxsya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gozknhhrm.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gtnanppip.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grhlgyoib.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/godepjwfy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gbxqorgbv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gyccyhgvs.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/grkbkknlz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gdhfhhqbv.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gcvzbfcuf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gevvlzhjv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gahnlgcll.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gitfubdpp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/giizrsnfw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gbfbezdel.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gwgmdllgf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gqgliltha.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gcoaxjexf.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gnjwgpopt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gmsoziizi.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gxsrgetrg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjbxzwzos.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gedeokohz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gnujefhsv.sHtML


<!-- 参考信息 -->