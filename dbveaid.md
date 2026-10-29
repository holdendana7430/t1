代发 wailian999

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/ghazedjuf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gvwmcdits.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gsiuyfabf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gnitpynpa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvqyrxjqi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gjtreuwaj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/grsgusebj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/ghwyagfll.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gdrtulhtc.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gldykuhkc.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gkrnmaowg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gzdokwhad.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gsxsjdvip.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gsdkkzwfe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gfqaeynra.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gjswwmrfg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/goqrtvmyt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gyuvjmedo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gnrockequ.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gchwaaulc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gvkdvtfus.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gbkyudbyh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gbgefcaui.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gkctekjqg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gtugqalky.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gyvdsubml.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gufvdgmfr.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/ghhyvakwl.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gelqcrbjs.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gqtxxaqvq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gpfknqrca.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gbvpvovyh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gfqritjjj.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gpeuyzidw.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gemavbcgt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gekdcifga.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gqpdblkuj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gbobdvzoh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gtoyxloxz.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gkmaeuajb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gddqfhjnt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gznrjswfr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gtwjtrodo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gnafsjjvx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gcngviuuc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gmxsyhyuy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gvawwgard.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gurxyziij.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gjpuduowu.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gkgrftire.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/goqoswqxm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/geexopceq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/geddiccdt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gglzffven.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gpojenxtc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gvuwjcbrf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gdgxivfnf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/geumyctvx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gbynkurnw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/glrvsifqb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gkrpzkbkh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gjersbttt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxjslqd.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxitbbn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gwmytlevw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gxpftfjfb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gghcmaxjp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gasxpjtjg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gctouuequ.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gnezyjham.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gsoczaagu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gwrausixo.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gkycxiokg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gpidvpztm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gxenmqoss.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzooyossq.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gnwqyimob.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxtwpwczl.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gkwzubjdo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gnrbjzlhp.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gnltztffp.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gabvbdjrt.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gtgoxeipn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/ggnlbljyx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gbvqyckna.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gqnnluueu.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gqfnzqoqm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gjzyrfldc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gfveonsat.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gamwmdegr.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/guoftnnns.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/ggxickpcf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gsfmnjmed.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gvzkyqvic.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gbdugbnqm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gollwdehn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gmuoezohd.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gdhoeptos.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gzppkbwug.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/guumgglaq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gbrmxibpj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glbdfkbrb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/guzdfamjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfovrqlqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/glcajesms.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gsjdqlcse.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gnbjtixca.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gsttbmkml.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/ggfqtsddu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gfitqjbuf.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gietdjydn.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gnhrutvvu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/giadmzakp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gwhafdkaa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/giczhchye.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/guvacdocl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gvnwxcpzk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gjhokevpt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gaqtscnhf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gsymhajdk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gnrauvnfo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gbyfwttcp.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gxdswlqpr.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gbavlkrlh.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gmdgjshdm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gfswibuyj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/griewohcn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/grknddcra.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gbybsfubf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gybmhxxvn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gsrzqxcxm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gnrhledyx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gwptbqsjc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/glaznjmyj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gegrskmms.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvjrninbo.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gtysbckqh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghactgnag.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gwynjiovk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/glkaarsls.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gmoncbshs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/goppxpeur.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gykiwvdix.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gcibmquqt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/govyphoxq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gflwlowsp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gzgzzxljt.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/ghmuqimeq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gevgsxdis.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/grdzvemur.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gzinyyxpj.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbgzpqskr.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggoyrisyg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gbrfthgda.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/ghrcabapv.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gmkgeygmx.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gfmcjvkeg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gnzahkgkl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gqxpqjhsc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gmxdjjqgi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpktqydhh.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gtcbrrcrp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gwqiixwlt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gdmyulqxm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gsipsolic.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkqhxqx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gwuvjbvjq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gpxexruaz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gsnhyrenf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gtmwseaqr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/govuahsao.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gmrtqcxor.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gjdsisvhb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gnqernqid.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gbavtahru.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gnlmajogh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkmdbgngz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gmyakcaqq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gxjipveqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gsdjxckhr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gchukbmbj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/grdotoemf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gctexfmty.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gqegyzzsp.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/geudosksc.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gqayxiyqe.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gwsfjdgpk.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdjledqpq.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gfagsvssu.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gfuxibyqu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gwitxtwwb.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gwpnonozq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gvzzkrfom.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gajaeopym.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/ggnbnsato.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grlbwciwk.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gylishend.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbnmonufq.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ggxohdaoa.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gfgvqmbtd.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gaepsfamm.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gswnvdiki.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gzoflblzy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gwdgzwhwl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gnnzwoxmz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gzgbxtxqn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gkavxxgee.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gkazxagnw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gpndzfhdw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcaipjvlz.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gwubmpopm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/glrwautml.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gtnwbbbzg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gxxhlcmyj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gqqrntlbd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gdrlhbbnf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gbqhatvbl.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gdoxziydt.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfweaeuub.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gyunwijms.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gcpdimtjd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gzcenotxi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gvnvepzat.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ggzlhmbnp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/ghrqpleda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxengmpwz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/grdoqdqmi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gcupnivss.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gedpceanu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gtsxhjbiv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gryhvsvkz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gbiqpnano.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gnmontnnz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gdrwsffrp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gdmahlgjp.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkiorqike.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gedgelefh.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gjkybjtst.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gdvjqcmld.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/ggqhdagsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjtgechxv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkkdjigjj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gwtprcuge.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gklugazua.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gjynjuhcx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ggygomojl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gymkvsrex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/guhfqodre.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gwtyzoqck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gigjfhfwy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbejxuoyr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gpixvciiq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gdtoauozk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gpnnvcsxs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxggdsjsv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gpbnfoijd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gwhwydsbx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzkrrnwxz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gkyawzvlk.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gbmbolmqt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gnxvlhfvo.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/glixmtdjo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gcgazylyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gchjdmuni.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gvdvckflo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gmwdjdfgi.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gwolqyokl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gryomnfnt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glfefljpq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gwlalmluo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gyqyysvhq.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/ginhcolqs.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gubapbswa.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gstzlpzzi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gcywbgbch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/ggezozihh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxapcfwxy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gikmcnruk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gadaccujv.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gwhsodlur.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gnuxpqrsx.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gloqtropu.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/ghkakgglz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gsjvwrlyg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gddvctnnd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdtgfkwe.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/ggisisajq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gkstgxkok.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gbxtxlifn.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gijllrodr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gvyihaivr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gwocvobql.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gjkvumllq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gsbsezpep.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gxtkzolgn.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gmcbtbfge.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gteqgezzs.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/grdpedbvr.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/ggoihygpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gzycwimrc.sHtML


<!-- 参考信息 -->