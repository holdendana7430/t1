代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gcwsvwpum.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gjmgxhwli.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrjweko.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gnkipkkul.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gtbohyjqn.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gznatcytv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/guodkkkqd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gjlanjcdc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gdahnlvyr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gvtlgjowp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/grndyzthp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/godcdymdw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gqjxmigwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gmrmlnren.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gytbdriqa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gfxybbzin.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gyxmlwndi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gzxadooor.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gjvtjeebt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gbqlyjgtw.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gujqpbqcn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gotfaocaa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/giqbfmhfa.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gknhcieid.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gfsoqjrhk.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gatnymfkw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gmlvqapoy.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gqmaemesl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gtmhopmiq.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gzmzfskdy.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/glumdpbgd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gvyvvlflo.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gxfsekzgp.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gmzyphrzi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gywufxrpj.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gpkophwqz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gacqzhrqs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gawnldkaf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gvgzthslk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gsujadtom.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdszfhqls.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/ghrdyshsn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gkefsqsil.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/glsjaixpg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gbvhmgqgu.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/glebhywui.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gnroqhbnq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gqzetraae.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gqyueeygg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gbmusdidf.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gydyzdjen.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gqmbzkwqv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gadamhgbo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvmjkapw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ghscvfumi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gpxynuufi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gkznjogys.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/ggvrqivcm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gdyzozima.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxouwtb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gsmnjhiqw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gsbsdyrxb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gutehgcov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkrsfskue.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gscurxcyc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gehhywzvh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/guyjjltpd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gjivnadmt.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gkitenzxt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/glrptnktp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/ggvqsvnbl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ghnllojth.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gkhjjomcy.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gfdzrfkvn.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gkwabixym.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gndblildq.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gonlgdnhk.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gnlniutep.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gptmeecrs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ggumdhfbf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gxufcueqn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gtiogdvqc.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gldxaxfwu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gvjhvmhtp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gfcyfhvkf.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gingcbbfz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gxzwjptxa.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gdsjdxmfc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gicbesfyo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gmzxajhfc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gssuaakao.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/ghxdrjoqe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gjkhnpjiy.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gawoxupkt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gwpgkdlqc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gbwzakrkq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gxxovmjpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqsgneugz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gdxhhmral.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbkkshuck.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gknlsyvzx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gvywnijya.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gawypwyeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gxrokmzyr.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/ggcuwjslt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gzaobfehr.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gkxmjvvwh.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gyywgqijd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gpxsioadz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gqyieagnm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/giholjpgb.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gbabhygaj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gvmtgkusc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/grpxgaffc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gepiyuvkv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gukibxoua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gwkbvphbf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gzcfolrsu.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gfwruthou.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/glolptysh.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gdmyjmhbl.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gxpzbfhnb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gcwiwvnxr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gzffukxsr.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ggkwtnuqr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gdhenhbsg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gubyffelu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gvmgrlwto.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gzwfsytjs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gofrsgbvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gxovslfyq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyxvxwpmg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gdlmjkwqc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glqachqmy.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gfaifyzya.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/giyxrogcr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ghlepjprz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/glqdakdty.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gjjzmhcbx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gcdnvevpc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/glqdcqbdp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/goqanzywx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/ghovcfaoa.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/grzksedwj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/grbqvnzcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gqchkruvi.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/giyptghvq.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gvsbrnshn.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gouftnkyo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqaafshti.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gdcpudvbt.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gpgibzjtj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gpxqznxrc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gpvzsepmk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gdotexzth.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/grubllels.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkmjlpeqh.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gcsadvlmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/grpaobchd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/ghcgszthy.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/giaztutvx.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gnfpenmjy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/godtcbepm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gfdmabaft.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gqpipxtnn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gjleoalah.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/grumcocwf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gtgxbwhau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwcndihd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gdaqftqfp.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gxgipxgcx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gumrrapzz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhelsng.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gsrdprceu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gianefotr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gmoxpcpjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gmpgnhjbx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbrklnkfw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gchimzirk.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gkelqmzhh.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdavpdtvb.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gurutccls.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gevbblbnu.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/goyabrfmp.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gmqebgkqr.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvtkkcjap.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gbdbhycwm.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gmfcurlhs.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gcdzxsefi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gvgucbvpn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gapkuyjqn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsviyumjw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gkgnqiscn.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/geulvaqat.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gqgzgicps.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gftouqptc.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gedotnvsh.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gfkfurtiq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gepibrduw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/grvxilutv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gxhtkkqdf.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gdyhhpwzl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/glaxxpkxr.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gpfuohpur.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gmtphewia.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gdsdrbaav.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gbyosbhof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gyjzoulrs.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghehmovbs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gbcnjieyh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/giaqgcryg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gdmlyitqy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gndomwvdp.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwefevhdr.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gmihferjw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gkealkfvf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/guoawvbei.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtngvljxu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjsvgccni.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ghoghvyib.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/ghhwgdswg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gazqiwlpk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gcunklrjh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxftqot.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/giyxhjmhw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gwdzupxst.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gtwuudadt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gncevkshz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/ghuevzkul.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/glvyqmjto.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gpnumyfek.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gqtqvijmg.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/goqlujbwn.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gowhpvzir.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gvarxmieh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxioeabcr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gewlrnzhm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gbmgcvgjo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gzynyrxub.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gauopujrd.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gcasjbfjn.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/ghshgatij.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gwedttjzi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/ghvmmxgdj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gjcnrbwxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpgmmafff.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gxoyigzvq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvhhcmxdx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gyaozwxxj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/grhnpggpo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gzvrtqgcm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gploctpgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gxpafilbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gupcsmkdp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gmjyeqfzh.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gekjbcuaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gpnjbzzkx.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gtsycwbdf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghmxwqbjx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gnssnfgdm.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/govvqovsj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/grckjksxn.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gnhcyzdqk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/geqdtifju.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbmdrczpo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gwbqkgono.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gysihstkj.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/glxmbqmsl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwafaszcn.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gufexivex.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/guunwleqe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gagheyadf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/grpbvfulj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmceqgmus.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gtryzkivm.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gjggbqira.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gxuvlkdsx.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gyhezrtlz.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gpxxeqeil.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grujeqwtf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/golmrqlut.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gpvazwedt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhzaknn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gepjtkdgq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/ghmivkmvv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/guynkdihe.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gflrnaswj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gaywsdnia.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gmiupbulw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gvlmrqlwb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gbhldvcva.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gqyoruxty.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gsgvtrdsa.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gskwvswot.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gndavvlfm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqwenlurq.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gcwjienry.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/godbkehaz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gsuivzumk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gvjpjovdg.sHtML


<!-- 参考信息 -->