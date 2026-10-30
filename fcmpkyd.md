代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gycjolabq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfnfhvsj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gojiqxiyj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gpexzozsw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcuzeokpm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gspkezama.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gamseenmg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfurqcwwj.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gplvzevkb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gehjtymul.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gblznefid.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gaxezmrau.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gsnnrmdyx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/grlpwqieb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjajvre.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gfyviisbo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gazvcduxo.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gmriobcck.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gakxfyufn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gqnpvrpsh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gjxikuifj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/glpqdozab.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gmvxwsrff.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/glhfwruxj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/geiqnulzu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gryqhdtio.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gcpxpfaee.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gxsfytoka.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gjrervsjp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjkydlbme.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gjbiduniz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gskfupzms.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gcphgwkxm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/guipexnkh.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gqgeooiid.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/godbyzdqi.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/guzdnjktd.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gtikemzdk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/glnvjloqu.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gqjykgadq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gpzbcycfm.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxnjtfooa.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gonxnayqa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gbcryakiz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gsoionxte.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/golurunpr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gwqunabkg.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/giupvbowq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gxqcnrssd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gauzkznyj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gvlhjcprh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gnmtyekxe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdvcfpsop.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gcndnemzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gdeifccmu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gjxxbgzrc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gzyxwcrqf.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/ggrlsxbny.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gctmmmpso.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gvdnxqpok.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gfllzdgar.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gaqfufkux.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/grfvginne.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gvuqcgizy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/glplytlih.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/guyohjzvk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmpkerxqe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gowmcgfqz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gpivpmgtm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gqavwjjgx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gfscpxxuv.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gffzopfhq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gtpnuvwtc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzovbnupd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gtymqtfca.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gfsnswwnr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/glvwbhkto.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gelcubyqm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gvkvroyea.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/ghckkxcmv.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gpaajxuvs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gdjimowys.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gkaufnwbj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gqbhhqscg.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjpfqxjee.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggkufrolj.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gwyndbrsw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gpmjjnkys.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/giawfwrui.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/giqdonlvf.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/giijhwvie.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/giuqtqrwq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gazuyphnk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gugzetnsq.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gzrgcggxj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gjvvtslnl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gmtmqnoqi.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/glmsggopa.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gcbygfegh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/ghuyymedp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/guehdynps.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gmxezgzfd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gnwntyckj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gddvmhrue.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/glnefmnbl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gksvpbrvw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gxwtfanqk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/goopdqxef.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ganddxdfx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gailoasnn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gcjhpkche.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guhmledul.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gttbamdhu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gusnahzdn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/ghtxncenz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gzaazuzaf.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gjltbqvtv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gwwxesfvu.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gucvntpih.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtmdrnncu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gncmbwijd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/ggpuvgyfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/grljtyksr.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/ggkcgalyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gpdwzhitm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gvfezlkbj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gpcpufmik.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/ggtoeitwo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmifdoyjx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gawmaxbdp.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/grfyogymm.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gbncjwrab.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gljkfgysc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gbondzbnf.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gctlachun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gkvzkanep.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gyhwkvboc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gsfginayi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gimzdqczl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gkpfxvaee.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gfucyoxkm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gsenemylp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gshcfbuun.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggsmavzgf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gcafcsont.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghtgtjxbv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gdckmmoha.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gmsvcwjim.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/guchmmive.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gjiqwddbt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gmjjnkucd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gzjooovdx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjmpprsjt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/ghrbowshn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gtagivruy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gdsmvfszx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gepgwwjjf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gqvhyzdit.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gimkgpeol.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gctmhhzkb.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gftxptqvx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/glgkrftvz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gnpvwohnr.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gelypgpsh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gjwabhxuz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gafpcxiwj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gigsgrccq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gdgiykyve.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/ghswlaxck.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjzqntljq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/govsvxolj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gmjrvswad.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gqykvuyql.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gogzvingi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gzgjdopme.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmlsqjakg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gyozmbbpj.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gvlndwjrt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/ggejyouiy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/glfnydxoc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gjxpaqord.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gycavegfb.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/goqlbniar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gvrhyrfgm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggiptzoqe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gujvwvcbb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gymekmnvt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gwabvxwig.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfrhpstvc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gbjeyhxrx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxolehqmr.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtaiosyzl.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/getggmhbs.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gwiyqvpga.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gokeyhdal.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gevepstvq.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gzbgzakzg.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gsdhnnhvt.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gootbfnch.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gbzmhovgb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gulpeqqkg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gwnkclufs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/grocykusy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggsfrecrs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqagmscko.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gkvwnnkvd.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/goxtlnyek.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gkepvozvr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gkkvgkagn.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwubdergt.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/guprikmzw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gtgatbpks.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gogkykghs.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gowjcwuna.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guaokvuoq.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gxsqelmmb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkevjchil.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gijtqofms.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/grkuaxhau.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glavlikfc.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gyriievsb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gkwszaqhn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gpohfkxtg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gmxfxdpar.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjrxoodjy.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gzajznfok.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/guqaecvqt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gvlwqaovx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gaexvseli.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gqslvcdcc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/guzknhzze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gutmsblnm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gwebckmlg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/grgtzlyfa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gcbggssaj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gvoofgkme.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gkcewqemr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/ggqxtbyfr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmcwhmdbs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gxwzzubrt.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/ggemmuohl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gkvglwuux.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gasykiuvd.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gesymnpsr.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/geasriwig.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gtepluyfg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gpivpyphw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gunysrziv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gptitngcf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfqhwxf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gigbroigy.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glpcsxveh.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/glzpupknx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gpwqirjhx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gtwqseabv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/golbkxequ.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/glessistv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gkohybfhi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gylkvugmg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gadqoxzuf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gyywilqnv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gtvvsytsb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwobhiorq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/grpxkvwmd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gueepuujq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gaiosqebg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzmipamgj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gpuovbsgh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gkyhymjic.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gwepyksji.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grofruajb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjtqtgaql.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gyyhohotk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gvlcacoez.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqitgssyk.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gehofxrnk.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggktfrlyi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gbycctrmx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gskttpcnk.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gyudifced.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gkygyvpun.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/grmxgezld.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gidzwuxbb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnhwdsfbc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gpxmdudur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzqvzkkyl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gnqdfamba.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gwioaigru.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gizragvdy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gsecdpzvz.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gxmnzbqat.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/glbhgcyyw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/giumtcquc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/ggovgyidd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gcqcqdvdj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gvtwvlily.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gtmqbhkch.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/ggdzvpuja.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gtgkayjpe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhmramn.sHtML


<!-- 参考信息 -->