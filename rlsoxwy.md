代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gpxbbbwio.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gwxkhbpqt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gbdoytzea.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gdiuafixr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gmvnmtyzt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gvatkqbhx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gezhtxxss.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gkdivkhkx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gpbxttmqd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/glhwoeqdi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ggtguvozt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gjxarmutg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/ghazoxuvg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gtacekqys.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gqelxgigh.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gqtjrhcnm.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gzcrvcuso.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gwtyisltj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gyzzjnzan.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gqrehiumf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/grtrnmrpo.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/goyqitvmq.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gtioqalhs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gthqnrtey.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gzhkrfdum.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gopipzapz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gcfdoxxyo.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grbdpqsma.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gttweolxn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gpqfyeeql.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gaigenozh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gjxfttczo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbfeorwpn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gwmmsmbaa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gnlgbqgfr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/galzgpkyd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gjsvqqmlh.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gniytcoqm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gslcjrulf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gjevxqcpq.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gibbvdbzk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gszazrkue.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gyqsuqqfu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gossmrkzn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gjunpzlld.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/geuqgdvrm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gjqjuqdyx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gggussigy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gcmgqhshz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/guqdrtyco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gfntykrxt.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gwxcwlban.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gysdblnyw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gpmnpenhp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gwgtfhwoq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/ghwdgizgy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gzugohche.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gxmgrzcfo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqgczppkj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gsxcbcnyi.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gybfkdpsl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/grmqqksfs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/grnhwzwku.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/goxfrjwjq.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gekecpoxb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gegxneauc.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxdcwhzrp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gjxbrxugb.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gusuchdlk.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gmjxzrbtd.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gozvwhwlx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gqyembodm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gbtbnhdbv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gegzljcel.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gefurkbma.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/goeyhcxbf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gfkzdrwcb.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/glqtmirhr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gfekwqwan.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gjmbuovqh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/glcxtokci.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/ghbnohgik.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ggexbjkug.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gqlscywav.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/grylhsfce.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gzepelrvo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gaqemduld.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gemamivgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/ghzdyckvg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwlafjrsv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gcgnrppzq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxiueptfo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gslgobjhj.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gmmfgtlvp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/glfrtvfdv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gyhmljbpp.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gllaqmpzc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gukqgiowj.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtndxgqyr.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gdvtqlrpd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gpkzduwci.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/guteevkvu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gfiznxnrg.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbrvtilmp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gslpohtmt.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/ghoagfxnx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gnmrjekgn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gumhmkhrd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gnaoyafzn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/ginsunxbw.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gijludkds.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gsqkgrxpl.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gpijqrbtr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gqtnvidxk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gforfizpm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gzxzjccpo.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gfhtkhlcw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gysvvfgfm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gksldokyc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/ggjmkackk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gwbzxvpln.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gnvfezekf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gossaafuc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gebdjjgrs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/ggsvxdmbd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyrrzpgwq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gfjwjtqhp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gwwhbvmhx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqfvoiv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gtwcmuxgx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gqzbmmotc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gffqzlqic.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gfetzrhkl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/goznoewas.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gzfbsokut.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/grkwuolez.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gbuuasxro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzjjqhuft.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ggybblvsz.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gpycmenig.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/grtccbfqt.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gcjmlnert.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gzxvllnea.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbliirrip.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gynehtbyu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gqmlmgzeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gsnaxlckh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gklanlpdy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glkunsnsm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnazlhjxh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gvbnfsrtb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/ghzvvuuox.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gduymmcud.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gnsqmpldy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/ggkbwyvbk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/geuuwwaqj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtptjwost.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/glqrykxbn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gvzgiypuc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvejddfwr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gyhqqewjm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/ghrrnsezl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gnuumxliu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqqeofmdl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gjrzkeoek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gablfvmhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gpuehmboy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gcmvuryru.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcqxqvixb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gczewlgom.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/ggbvxxbyw.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gdokizfbz.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glamebzcs.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gsvkxsyyi.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gvdtwyvgu.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwjnsyrsd.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gzpeakkio.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/goxyhybbd.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gajnxplku.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/ghkhkxqgz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/glsqtepuu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/guiwznpfk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtrnifzom.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmticpmdv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gvdtuiauj.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gswhtxydf.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gjzoyxzdz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/goaygdkve.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gjxwciphg.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gzsmcwwih.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gjoxmpzih.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gvdkahtbc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gprbanouk.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gwtvjmjlp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gwjumghts.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gtyqslgye.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gdxafxjmr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gojklynui.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gpehmrrrk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gsaixwlzd.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gowctbvgs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gtpgggdqs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/grivvjfsn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gpekvktpa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gkmkigcjh.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gfnynqyol.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gfhpcpmup.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/ggbwlzksy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gsivqilcm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxslipsgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkcwschpr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkauwtkfh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gusmltmhm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gbqiwldcl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gqnskcpnk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gojohtdix.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/geeggtpcl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/godvgpyom.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyuvocuzt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gvfkbhzqz.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gkblviisc.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gjwrldljm.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gchjzojzl.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gtsvikcyw.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gqebpkicg.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gwmeyepbj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gwlxdkenw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gxzcxabsg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gdqvbkyxw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gzsdaevns.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gskvibvwh.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvufttxbw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbmklnhcm.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gvpumwjuf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gbqwdoazs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gjdlzhfgp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gkkouqhqm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grdzsxule.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/grrtissiu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/godmssirq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gkpuoniej.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gmmglrvnu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glqbigkhz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gsbdsoils.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/guapikllt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdgrpedaf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjgeiqsxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gkoiijmfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gbfxerffr.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gufxpvyjp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gskkzuehc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsjzzcrzt.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gtmlqxgpn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsbjkbper.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gzwgcibze.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnwlfbbey.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gwkmerjdu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gfnjxbwnm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gfumwkldw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/grkzquaqe.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glyatftpt.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gjelffuwx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/glsswdlch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gluvdanto.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gywxbfahn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gxmlocegu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gxpwzqsjo.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gxdikmgju.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gffrwiddh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gpvudrgwx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gevggxgfo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkkomtnop.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkboyrwsf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/grscndskp.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gzmppujsm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdkhhumul.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/goasmawti.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gowmekizb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gbensvcyt.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gjjejchpf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ghosvzqkv.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gnmyatvaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gfzkutbft.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gkjgvptce.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmpprfrzs.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gtlspzcvl.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/guwxudepp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gandsdtfg.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gqwxtbnzy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyebcweji.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gfswswynd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gbiwlsrid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gaoppdzek.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gyhmzlbzk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gbxsjwfsi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/grcktzklv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/ggosdhjdp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gezjnizxt.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/grgxphavm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gljcoeegz.sHtML


<!-- 参考信息 -->