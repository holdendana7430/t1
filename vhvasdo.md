代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfvrbooyq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghbjvsgmi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gykreyzhn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwnjzyrsd.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/grzmfgwko.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gsguqejkx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gcazkvuyz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkjpmjgvw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpquultnw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gnvkdircg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gokuwchzt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/goczwdstb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gbkwriwoc.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gploavkdo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gaannarxo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gcsirdlsu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gpgrvvzit.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gupcxhasp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gyuycipce.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsqfdmw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gfrkursag.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gskveiyvs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gnxaglblm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/ghrlpvjgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gxdtjyrii.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gtkfvpicp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gznwzqrwm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gqtkdeoxv.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gimrankfq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsdldetft.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwxlcqax.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gsmrsxzpc.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/glrkjoaqa.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gfgaohcsf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gjwetigsx.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gujnvydjx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gwujxyela.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/grpuxthft.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/ghrjgmtbx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gguxpyelh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gtflwrsth.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gvgrnfsrp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gwvqkvsne.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvatenkhx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/glpnhnhui.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gieubxwua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ggdtmkast.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/ghzruvdia.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/ggenrxunr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/glfuqxiyz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gozzapbcu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzxwsfwzx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gxqutinmn.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/ghotwjevr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gukvdotsp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gyxgpxkxx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/galljuwbq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gneznjhat.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gepkttafb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gosdfdhzc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gohlcrubg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gucvqaoda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gcmlpkvnr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gsfzmpwoo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gfwhbyzni.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/genncudzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gzfsnoaty.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/ggxfhfgxv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gczmqxepu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/goiljnogr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gpirwhawb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/ghljocmsb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/grxoottgw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gghwgzaoq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/goultmypw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gzyajrwtx.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gyqkbwqen.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gsmvulxno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/ghscmqqvr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/glcdzynln.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnhnlak.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gtiuubkfp.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/grdhynlda.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/golqzydik.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gndwkwvkg.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gtuylautn.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gzohucvcq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gnarufudn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gpvmfhjxj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gedvfwxxf.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gvuvykaqp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gayoywsqe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gocacfzyk.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gymlgfjqn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/grprxfhve.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gcsmhrswt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/glqcossqp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gwnuxyxpj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/garymjzgw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gtawumzbn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gckodzrwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gkjqgjxxn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gswmplxns.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gvnmnqgcb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/grfrttcuc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gxdztaays.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gypijaqus.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggaugtlxh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcmaxwshm.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gyhbpochb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gsgcfcvsn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gkphhlqok.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gvdkbihgo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/guxucstor.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gbqspmxaa.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gyziulbhu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/grvibgern.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gnoovcdxf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/ghdzmixdt.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ggwmzcuqa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/glffdglkt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gzwnhiudo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/guadhlrnf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gixyyppmw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gwussdyix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxjafkder.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gkhpabihv.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gvlfapccz.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/getncdusu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gzfgtbsrz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gernamgzi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/glbojvubg.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gdzyblohr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gsxxpeagz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gjnweyhai.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gcgnsxxwx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gcnnlqqpg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gkxagkckc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/giptbemjf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdonoihfu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/ghjzsbhpb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gerewwkbc.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gpvtqdrie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gpewhfack.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gbxdyscet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/goqdypbli.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gfpmfhtaq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gnujlzpcp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gcbriefbh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gxpscbanz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gbtfjjjwh.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/guwwilste.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gwtmypwbh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxjqryoyl.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gswzozcjx.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ggjfqqflk.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggryolarw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpgfsowmh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/geitzclws.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gejeaiqmz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gmeuhisfn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gwwvzhzet.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gwnapfltd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gbdjoppak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnbvomsfm.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkacyemlz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gawfjonfn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gvcyuybeo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggxnvxmwz.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/govzdrgha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gnlsoqktz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grtoutyyd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gknvjhcrb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gathmobiw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gddjwdvuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/glkccjvnf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gosunpggk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gaybmgjsa.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gjmlymsfq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnnnmuowz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/givcmhcvz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gmlxiirkz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gmqmkrzik.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gegseaxnz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gxxncqstx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjjpwddlx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gstjhlxzd.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gmkpfkdru.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gcghxgajj.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzgnvhncn.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gmykuztjh.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gxwizvtdt.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gxoktlyao.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmlgblnmn.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gqgktcwgo.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gtymkbdya.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gbusuzejv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gvxgfxhvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjauodany.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gwxjriooh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gahzmpqgn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gkcwgevnr.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/ghefjrzdx.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/glgvsmvxf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/ganjhqzht.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gwnzrhtix.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gvxbwqvkm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gljcpbtcq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gscsmerqc.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/glsltvjau.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gffmkghsd.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/ggwnruqae.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gdacypwdn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkyngcyxu.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gpbrkzqlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gapdeguuk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkhtafrta.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gotdddnme.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gmwnnhdro.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gwvhksyak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/galrbnljq.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsfglgcgu.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/giuyqeiuv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gbingtams.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gatewuxib.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gafgzwwoa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gwucjhwya.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gpzaeaibj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjybwotji.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gptcnieqe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gkqzznqxl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gxfoebwgu.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/guxhssygp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gqubhnkyr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvdipunaa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gjfpaufim.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gkqevebii.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gpjpznctp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gligckkrs.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqzwilkwk.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gfwkgbccu.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gsowxoazy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/guacvzswx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gojiehlpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdrlzwbom.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gpqnpmiut.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gtqdpjnuj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gggcqpkza.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzwvrpnrs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/glbyonwyl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/glxjfvecn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/goffbfunt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/ghvxrhyae.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ggtrhvtnp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gzmmagelg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gqmipzinu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gstbaywjx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gbkqfjsnl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gyiarhfph.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gwsmajzei.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gsaelrffo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gozyhwwxq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/ghzgtyyxb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gpdoqttxw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gnzeaprsf.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghaumnpne.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gnxuapmur.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gzmmuuncg.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/glefbfxdw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/graxfzxae.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gbycilrsx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ghbxchiiw.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gopsrcuzf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gxtwxfxrt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gkpxozark.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/giwfbtnes.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gozypsvck.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gklmulfsu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwdgiqgfa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grbuzggnk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsbsantxe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnwsatvwm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/guewgeuxd.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gsybkqqvv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwpbcwkfz.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/geaqdmrer.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpqmsrd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaborhxmj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gprqdztni.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gproptlmr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/grqvebzhy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gfrswjwgz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwqcttamg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gkbxnjlty.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gfkhrblyl.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gefifbxsg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gwtbwmobu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gmugzdgxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/guwqfmdox.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gzfrlzfhn.sHtML


<!-- 参考信息 -->