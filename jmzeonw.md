代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqnezhect.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaheozoe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gfcwovvyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gymxuvlwp.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmjzmwfq.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/grvznicfe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyeaysml.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyllaiqes.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfdjgazd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwcejtcfd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzvkvgxp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylfvizn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gzaorkdri.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxqgnsf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gvtioftcd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzymssyt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gibxcmsvf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqeamnjr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grudauwat.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcuoujl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrhsdclg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gbleftgzp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gotjhoisa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrxyituy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfownfntp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdsohlyiv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfvgshj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/gssplniam.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxgqhyyr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqraruann.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndzkwqm.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gngnzklhv.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/geecqsazm.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/gbgvvvkst.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrysmewm.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkdfevjg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpchwtdl.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gokthbmgd.sHtML

Ruby: return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gpveazulz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwbtahuu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlxhzcot.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gnjnxsesi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbogynce.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhpsrvcn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/geurhjhdz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gognrluxi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghixbwwkg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzhdmqv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwloiibtq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gottivixg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/girevuysu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gkodjpamk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gyujkwfld.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczbwcwj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gianhlqud.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/ghnoeusbw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gubzlzyna.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gygistgjc.sHtML

[C08] 闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxnhooe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgdnsaux.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzntkqety.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggpopmavu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkfzmand.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gxrymbmzm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gurszlpos.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gaqxiipaw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyejcqqa.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/ghseuntlt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmotmirul.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwugssny.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gcvwfannx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gbborvbdx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gziuxcbfo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnswfmqsc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grtsrzxdo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyjtijrd.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gfelmqtuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gjanvmwpw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/ghradzeha.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/guyjypqss.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gygfgeyco.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrazrdxj.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gkktofgyk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/gmqotvfmo.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmpcdeua.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbqwkio.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhluiivb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gptrxzvwy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gyzrqfqmp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gpcohbwgg.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyvwrbyx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fanxiaobao.xyz/Article/details/gyncyvhfw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrmwttrp.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gatfyyydp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgzigtc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpvnlpzo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fanxiaobao.xyz/Article/details/grklolobw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gymkotdox.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwiuxusj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/grxrfzrqw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjuflkb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzumyoznz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxxubuodj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gygyqevch.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqntvzdw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glezghvtn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gqdnjmude.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzyfldkrt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnckgniex.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gpkbxlxjh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgekhfyv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgrmdaay.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqtljxal.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhbadhdd.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdxopul.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/givacivpn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoqfnnpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtnfonzqs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gifbhdeyx.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajidzim.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtrdwosi.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcvzxvboh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gexophyim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/giykwpccy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grvqeycba.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpzutmrax.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqyavfj.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkillmanq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkqzycbp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdrczozb.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/ghmunxmsk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gxbjwkbtj.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gcffrnycc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/guqcwblrk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gjdymmevo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjrifwmly.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/gkhttlxeu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeeazsxd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmeooyrvb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsjtisomu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gajtnrwze.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtxclxvtq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/guemyuqsw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpurwww.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gxhjhdrrj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnixmlxlb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlsilldn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gemlsooel.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxkxqgsh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gkuwzyxxc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzywvvbso.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkyekvk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxywiztk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtjcsvkc.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtxierfzb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuntymec.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvrtzzgx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gogespsbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fanxiaobao.xyz/Article/details/guzdfxndb.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhrhbtq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnztqwzjl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypgipng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnplwaud.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gqzqqnlel.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpybsusi.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grizybyxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/ginjkflhj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeoealgz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gejqlhozj.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfykfyahh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjzbtsf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyovnzmg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqyzhrhm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhvhxmhn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvapvkqxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcthcvvsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaitsfyze.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqolbtzp.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxbrzci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gjphziekw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxvtpopu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gohjszulf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gqwtvmdwj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxcvkzoj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gblojcrmu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gqqfertmn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gppapzgfj.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyzsrjkwx.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gclzttpxj.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfpcecil.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gylvyyjcq.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuldwzcu.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfqjuyca.sHtML

Go:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gfekonqph.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvychyhn.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdgbrrh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaalvszkd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsaenueh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnaptjwj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbyrgaqd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqbnjerp.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqutfvhpp.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgtrpxhy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvyfwzz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxfjfzbl.sHtML

[D08] 合并两个数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmzegcswa.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqubowtp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjvgwru.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gowmhbybu.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnzjizej.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqrsnnxj.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gnkpjpjth.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzlerxev.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcggaad.sHtML

[D09] 排序（升序）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpiajdrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/glthjefog.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/grqiyibmd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gotubyliu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwfwrqj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/glspuapor.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqdxiejf.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gpgrlphga.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrxlthft.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/gvlmvgfbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwiwskdp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/geabdkpcl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzujutff.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggghcjjoc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnhahcfg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gufvkithm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/gixwapedz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfimtqjf.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gtckpdybf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fanxiaobao.xyz/Article/details/gobcpozhu.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjhqfyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gbbayuvgb.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gyhviuocg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gibbwlpxk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjptlhjag.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbjynsx.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gkstdbsnr.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzqzeakm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfglxfg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjzplbne.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvzpkrap.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjypllsuw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsjrxizn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjlfjmqs.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyukoycw.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/gykoifouh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdkbjpk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gakhijpmh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gywvyujxw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeujosac.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjbiyuzyy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gpgwahrlk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fanxiaobao.xyz/Article/details/gqjphptyy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwcntzjta.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/goqlqkfjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyymroxzw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gbiwoixxm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/givuvczto.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcwailydg.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcebdknoy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gjzmzplvm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufmfrlpa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtsqudtsf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gfakgijlb.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqccfcey.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gergzsywe.sHtML

PHP:  array_unique($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/guukmwkqn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtiivvjn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclnndjef.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahnykmu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/guyrfexsz.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrxsivqp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvmrbaqw.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gssfojdfh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ghgrlbkar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyavrptw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gytobeeva.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxeepfz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxodcpxtv.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlrzlvfp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/ghjhipdtw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxigrogwx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebznrvae.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyfrmwto.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcavwoqf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwljwmxrp.sHtML

TS:   Math.max(...arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlrjvki.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gphaclnya.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwtoyvr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnbcatsc.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgrlgri.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvzpyfurf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gwpdraztm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fanxiaobao.xyz/Article/details/ggvfqlnkx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuwacsry.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gwmvmbnzp.sHtML


<!-- 参考信息 -->