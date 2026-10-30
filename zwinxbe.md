代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gknbllyrx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/grrondbni.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gcvheypbt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gopnslczt.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdsnsmbvj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/goftbsxqb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gkfyjlieh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/girswkbjc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gerytpcgh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gjksslxlv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gkenmkpmm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gwfnhkngz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gfuhmrhzn.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/glgonsgci.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gnyzgczss.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gttshvuah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/ggljawhma.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/grigrkpfy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gacnxmrel.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gyemtsdpa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/guopbulds.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gyueubjno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gqmkyazfu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gauandhly.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gikulvduy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdlfygxqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gpgxsqaqi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gupfyuxmg.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gpefemfpe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/ghhmekjbp.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gwskdjqsx.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/ghziesjgf.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gkegfwfgx.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gjonqhkwk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gwtrfgikz.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/govjxgtcd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gpyigjgok.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/grrcoxtpu.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gygdejcre.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gadrtoobs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gsoaapput.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gtcrkzruj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gowsleisu.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gjtfddmed.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpxynjzq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gevzocpru.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gvzzxvzdp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gzufdvgod.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gcshficir.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gdibaxkij.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gyzdexjxf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gnzcubpvs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ggenlfadb.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gnpgnokdi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcczzmygm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gcbuxpwud.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/grlputwnp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gguwueyrq.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gjluyxbyg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gltvzzjza.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gzmnusffc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gezilqfio.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ggaotecjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gvuggttdg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gufxqnswe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gubljuctj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gscbymaky.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gpjdskojs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gwsldowqc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gcnrbppdu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gfodnjavw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gcehqqbht.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gbndpzzmt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gaoiqoxpe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/giipujkuw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gqdmvouqp.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/ggxcywniy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gwejcbhhn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gvuvepfhs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gjgkofvbb.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gihjosdhv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gijdcbqup.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gaszvszwk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gklrzntil.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggwtpcxme.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gabrsztcu.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/giduaswrs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gnemukgbi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gtnbpzbvv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gjdnbwnaq.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gvoblnuqi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gthfsvovb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gersqcvqu.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/glorlytjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/grmehbohz.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gqzxsdqde.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gopjxukff.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gquqftypu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwhneoqra.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gltcegwzb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gcanvfxrd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gzwsseyae.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gufctfajx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gtvedjnvu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/glglmpsxa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzsplzbph.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gtslrokfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvvlvnjfh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvfkoryzx.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gglmszwdl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/grycgoods.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/guxwwwiln.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/grbdgpbyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/ggznbzqoo.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gmdeuhdvf.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gilupjxco.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gvnhfevsw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gqfnnwuyi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gowrhqkkr.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/guwmgovxp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gnitceyou.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/ghvoooruy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/grydtnzyr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gyvahwzbv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/glhugzumi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gbwhmjlpt.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gprzgyayy.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gpncziicp.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gryllpdba.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gpjpnkcay.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gkoovyudc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/giejrtgpr.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gemelxxdl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gjwjsffra.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gyqdipdvv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/grnlonfrd.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gycabbqdz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gymytxnmo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gobutmxrw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvvqbeaqv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gdtcozngx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpnyfnclx.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gjclaakfs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gtoymjfjq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/guapvdpuc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gtysyttiy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gtgrioguo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gbfpwycof.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/grbrhduap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/guoiplqvo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gmctxupwc.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gbevigrfe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gcmzcphte.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/glpbfdygh.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/grjloylpe.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gwyqckniw.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gbgelkjzm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/giefhzlox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gnkbobrwi.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gxuviwbkb.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/ghtzmhagw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gpauedhzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gigddptka.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gudsuoskl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gloutyztq.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gettzajuc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gdrnniuzg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/govdvdtzd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbcdpsndt.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gmzglwhdz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gpatgljdp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghpwwtsta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gpdtzzglu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gzccdewsb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvlpvmy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/glwnypile.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gcpqlkzad.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnalijgnd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gsblcibsv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkuszxfmq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gldmoalhk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gacswzrgc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/grozovnun.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/ghanqxzzg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ggqqdovit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gedocpvnp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gllpqopsf.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/glroblkiv.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpowfmkux.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gfzybfyrx.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gizbkuieo.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/grhtbixap.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gyazqbjns.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjgimxoge.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gjjubimdw.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gladwxgaa.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gqqsvterf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gbnnjkpdk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/guxuybkks.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqfgfxwbc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gtlfmrvnu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/golltzaya.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/glwhltfaw.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/golfqivfn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gmtcihhpn.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gflxnzvlw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gmbfikgkr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/goqwsrglg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gllbccwus.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gqxgkpzoj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/giyqvytad.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gqswyqpjh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gnmnjwzdp.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gqbfijimk.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/givzufbag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gnbhmjbub.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gtxcuqrlw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gelseiawc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/grdsreiso.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/ggxxbivyi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gmtbpzhmn.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glcnowrhm.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gfzkmgcqt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gopnytvon.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gyxsbnvju.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gwtkleojf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gypowkjol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gierzhhng.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/glytxnvlo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gnpjoppbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gkokenyoh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gocfxvpyz.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/govrndnye.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gmcfamndk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gdikxagkc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gskdhwklg.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gumbrcvxo.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gbdkifpcu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gsgzojyyy.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/goknpwzlc.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/goxcpqyoi.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gvbxrzrrq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gvnoyomdb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjhmsbhmm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gxdyofkje.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpnmhazn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gyeeshrew.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gilnchuic.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gvuartpdj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gyppmadon.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gtijrydme.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/glwczyuxr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gxbmmjrzj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gohpthmwk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/grgcuqtkl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzmevswsv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gheuagybm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gfyzitasg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjwomwgfy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gzxywiyev.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guvuizzvf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gmilqfqnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsquowhvc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gmiqtejuf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gltljpxra.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gitvhiiya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwgsngpuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gjmcnvyrq.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gokxgwuws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gxhevnbbb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gpyymyiow.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gemboqdru.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqsxscsin.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gukzttsro.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/giwefjybj.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gfqhlenwn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gjktcygph.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gmsyoprsp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvaywerkp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/giuxiesge.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpfdmevkz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gogwrthtr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gdlgcapwm.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gyhipsqxp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcddsqufp.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/guhtodgxt.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gbxvmdvkd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gfxqmxuok.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gciobhlaz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gnjfwdese.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gvycxjpro.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gakdqtskh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gekwvkzlp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gxdrygubn.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gttjxyzxy.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gwxuztvov.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gnvjpmcmo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhngntdq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gtmzwysod.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gbnvwousu.sHtML


<!-- 参考信息 -->