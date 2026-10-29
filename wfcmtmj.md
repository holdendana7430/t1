代发 wailian999

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvgahhaiv.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gkigizhqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvnrzoowl.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gdklyxawn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/grnurnibx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvgnjtkmr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbsszcanc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnzusqwoh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghmcndqwr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gtplioqqj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/guunnkfvr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkcpqgiyr.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqapqokjw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gkymtgyec.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmeuafvmu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glusxcqlz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrcvvazc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gnaukfgqz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gefvgmkun.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/grimmojcm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gxadmiolf.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gxnrkmnsf.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gffclhfqj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/geicbgjxm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/glvhhefby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gsanvgbhf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gpvxfxnew.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gwgixcubx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gzgthkcqh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gboixrfpg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcwyfzy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/glrnsuqwy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gvlwzmivp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gydybmyyy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gagovltjc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/giktewzfr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gkkvnxekn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxwxbwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbljadqnv.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gpddvogty.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzefrjvfb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gamoiucpp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gsuupqcbd.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gjsmnvuyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gyedrcptd.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gipjclnmz.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gorfukgah.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/ggixlkbbk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gwqltqgvo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/glkxnssfr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/glnzsgoeu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmiglunxk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gxufztygo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/grdduktef.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gnmsihnpb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gxgwdkztu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/guihwjopf.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gbujltymc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/glnormvkg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gvylabijx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/glanjhmwh.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gogglygqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gbhaoylso.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gxomlroed.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gaqrfddwx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gmlhkhyeo.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gpshodovr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gnpdelcay.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gjajtgcyc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/glwtgamzw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gmhehcnzm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gbupobxim.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/genoxfcop.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gnrrbkasm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gubgihnsa.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gxbfzrjaw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gudzwcxwj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghyesnnzd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gbftchnpr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gzbnkunrk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gpaatmgnk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gmpwjyhon.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/girekxsgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gpawermdd.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gmquadzwz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gnbphizmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gjkxspksm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gchougfni.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ghcmdyivi.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/ghbqmlcqu.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsnyqqptf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gxdpayqtu.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gwzzexmxj.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gmzwqmuow.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/ggxzetqje.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gdwyoksvw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/govhmwhfb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gspkqvisx.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gdrfcuydf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gyctknifv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/geemnxgkp.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/ggxiwfhuf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gsoqifbkn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gmwtzpkqs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gwpunvagr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gahaywghc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/giogijxbn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/glliiuvoq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gzfotcikj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/goireaxvh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/griocjyxf.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/giyslpxbl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/guapkfmnz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gjzpiuugd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/goqnhcvuq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gumtggtku.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gggbuzytq.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gskalcbav.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gvanjcvch.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/giqqcmila.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gohjupdpv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/ggbrdbbhk.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggclowqvm.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gzgqduzfo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gfexhtgkh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gfnzitlrp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/guxjupghu.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gquilbtwo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gwzcarxhb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gwtxxmqmn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gytocbltt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gixtgjbgs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/grnruvxnj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gewigdbnc.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gaqmlfbpw.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ghbnutjck.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gqdlechco.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gvvjkyfti.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gxyubhqxg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/ghstgeqdm.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gehjyfynh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gxhcnxxzf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gxjrbvfif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwvephwgr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gohhacekb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gpccczjtv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gktpypthc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmeeilowd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gpkfiemnm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacyxglcc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghbiruexp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/giplhkdmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ggpgtxywl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gyjkzbemp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gnklhmlot.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gkclhdxuu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gynqscens.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gnuqlyegg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gdahwqcdd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gziuagqbp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gwdltvanf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gbkxrucey.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gprwethfc.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ggcectwdd.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/guyensthn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gzyrtgttt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/glabcxmsx.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gxunrzduk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gjujfgagj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghikqpznk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/ggppyueic.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gaxjxumll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggppyicfs.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gbmogptvu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gdbopqcaw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gvmytwbcw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkuzpgmbn.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gnsgthhls.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gawyerzqq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gtydzprlh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gsyfofwlm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gtaitwzmm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gmugsxbou.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gsiamoggg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gckvnpkcx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gnbdqsums.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gvxlirwzw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdkqojfga.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gukzkevyy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmywxzhbj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gviyidyjm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gydxfbdti.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gsewvlydm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gqxyzxvib.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbxlircwv.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gpkgvhoib.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghjbbedoi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzuwxmlfz.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gukmgkczh.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gbceeckno.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gknszzgwe.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gztgtglzr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gpyyzvreh.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/ggnrmhhvr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/glphmvoqh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gswmaophf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdaapzoqv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gflywyjol.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gofwzkzjd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gocftpbxk.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gsbggygmr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gkhzxffjk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gipdufddj.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gkiuzlkeu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gsqqjrnyc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gvauoexwz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gqpwaohfh.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/grreknsie.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gpiloskxz.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gtphljebm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmrlnukor.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/glpglnhop.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gintpiavz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gjtossowl.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gfifhgafu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gayzukfto.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjmwqxdkp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/glfcxhdgm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpxyffyst.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gidcvyyks.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gqbrsvumj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/ghgwiiopg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gizhjmjuz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtitpelye.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gjgubjtbi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gfillsaci.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/glzicmvwv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gsbegtqkh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gwtweakuh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gfhvrpwkz.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gzzztlcjs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gcuyhsfgi.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/guegfojaw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/grpjdfbdc.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gantwywkt.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gusabkqll.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gvdgkchlm.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/ggiuzxyps.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gcfvckdwv.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/grwbjwdwz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwowwryit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gbpltmbcx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/grypclkfs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdtvrlqmy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gybsxfbos.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwjhompsj.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gcruadjoc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gbpgtztgj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjulpbgmj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gbqkavssv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmrjbxyn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwgwanmmq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gpyrihjry.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gfjecotik.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gczpptzvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/grctrebjh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gakxkebgv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gjejpddnd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gczqciwpm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbcxhgslp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gxdqlpriz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/grusgrsil.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gecpebety.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gpeqvdfaw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkgaxaggy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxdlvfqxa.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gwqqnhurw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gqvwobrpz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gvbeqgnnl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gndztfaam.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gizrulhyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gsfcclgcl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gvkfvumrv.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/goweqzljg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfsgkegrf.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gowhoukdn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gvxbpoice.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gqqzyaxuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gisnimqfb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gwwuroadn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gylaqppmh.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gqgfcowgy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gutekwuce.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gafmtofzo.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gcgkhoisr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqzhqbpwf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsfsfhznk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gffzqzxoz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/ggblzuweq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gbljdphjm.sHtML


<!-- 参考信息 -->