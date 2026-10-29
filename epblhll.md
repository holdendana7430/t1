代发 wailian999

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gitznrjjz.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gtffgfltr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gpreanfsx.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/goanuwgvw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gakietvzh.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gnuwstsgb.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gkvsjisvf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gaxgjgsir.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gmkgaxhis.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gfebvamzb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gxxmsjyon.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gcqtpdbcf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gjkssjqne.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gdkfntwui.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gbyfzebiw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gsotmsgjn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/goplsyxhk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gxyfxwqqd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gybjddnhb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsbyvqdto.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gufuaqfcl.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gtwgiayvn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gasjfpaqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/glhblpjnt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gubedawik.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gmmvtelrw.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/ghpmzqvjk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gdsguhbgl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/geelupkdm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdustwncd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gpvnivcqr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gqkyjbkkf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gfjfhkmvc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/glvwjgefx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gkwcifspi.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gfmevkvdo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gncyogtxc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gdmlsxecc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gohwlnhfd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gvdewoejb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glnlszpcb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gnuyljwiy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/grgflgwcc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gafoptojt.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gndokcrwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gykjrtaqo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gbgjhyqxi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtjijvtvs.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gbpklekdt.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glglnwfxn.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/glkmipmhs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gxmdamhfo.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gglpgywsz.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gohqgufuo.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gtfdvkktj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gsuyyapoj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/guejiuxpl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gozddjdxk.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gzaabyegj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/giqvirjfp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gszinmpza.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gdliezcrm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gnyppqzvs.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gutyjdqah.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gtjwclhze.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gaqtdodnc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/geqbttzaa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gujbjhxzz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gvhcuwvlm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gyqeysrzs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfaujrqiv.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gycxmbvlh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gnuqrwwod.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfkcfnvpx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/grlwgmuxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/giobbzzue.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ggzmcjhbv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gztwfxjji.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gpgnmsgvq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gzylarnki.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gklpdhywo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gukdxkikz.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ghyxbgkcj.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtblwdshp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gajdpitus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gllbrnckc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/geyfrqkar.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gitvehija.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gpgjjsfrh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/ghecqomnc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gadrgxtmg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gbtmnzmrx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gwmrqkdpx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gvwakqpor.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxwzwsqxh.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gyxxyjhgz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gwdfczclw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gwwdcrxiw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gmugzhvvf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gjkoeeqts.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/goufmimkq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ghadzjuvt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/girtpyzxu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gkmwezgml.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/glqzlnoxn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gpsyqzuyc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/grsoapovm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnqqjgqog.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gypnqbssb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggavddcro.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gymedtupn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxmgrrstp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gmsxgvihu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gsdxorvad.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gngwkvpfj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/ggjisdfyd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gelozancj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/glapkgupp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gwkbeobll.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gdvrkmpjj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gpfngohau.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gxeocmymt.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnfjdqkxb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gihtjrpvf.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/guxtfgjep.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gabueacyd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gysshndzt.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gimjbjrks.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gweokkfzu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyyoxcirh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gtqheimni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gjquxigoi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqekcielt.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gagxqaoyw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gidvnbvoc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gkridxjmm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gjipuejtz.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gebiklwvg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gzufakugm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gbntoptxm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gdffcyzax.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gohhfnrdo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gmeymjegk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gatcseioq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gasxsgnhv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gtpfcprvq.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gkxoqxldu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcgfossoo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gqqywlxsh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/ghbiuuuwm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gaqcmgxfk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gznngodqt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdvwpdfvg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gsjmvqkxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfkulzzpk.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gpigxeoun.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glwomkvek.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gposmzbfm.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gysbabsnq.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gcntofepr.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gmljlgvnx.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjotzlray.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gupwudzur.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gtewvzhwp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gltuwtqbj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gyaczuzlx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gjegntifs.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gvvhfbaps.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbgivrogc.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gwvcbvaxf.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gtsgxaxbz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gnsehvvvj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gxukswedh.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gvrdzbteo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoinolav.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gohijjohi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gfwlcycqr.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gwigzcsch.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gmpiuiwfd.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gfddphdex.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gjcrsvnes.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmytqpbhf.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gpjlcbsbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gsdjflxkv.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/glnzqyqli.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gnmedrvny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gszdhxqhy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gwbkshybr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gfuiuibtk.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gjxacyvgx.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gcisiipkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gbtismqnf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gypugvdds.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gbkpkffic.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gmvrehefb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gowqwrtww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gwoinvnrq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gigzjatxg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/geskdding.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gqjtgnvoj.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gllgbrgmu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gebounlvy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gefsrlucn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/glqoeumiv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gyiqobjtr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gcoveneut.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjxwmpdus.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gfhkquwmm.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gfdoqwlev.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gppcimxly.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gyjyxvcng.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gzacexzwa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/geanetaqr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwyiiehwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gfsqlfrzq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzdvfcrcg.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gtchluksu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gnqnavqdo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gcxupdglg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gelmpjnwr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gjfcclieg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gawlfyemq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gkcfhkezn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvwxmckka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gbllmdeih.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gfclqgofv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gppygwtqo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gdbexwpyn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxmhyrfrc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gvkwkddye.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gkuxalxez.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gverpfvoq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtkjojsmr.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ghufgqkho.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gzcosakwp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzgdgukyg.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gjfpuedcp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gxfrtcuvj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gpbenkdtq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnotgavst.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gmmjdcmzg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gwzyxtrsz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gabzvqxig.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/glmhdwfbf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gpnevyloy.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gvfytgopi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gxwhyyosj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gucszcknt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gnbxpjodu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gejlllyzp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gkqvfoatp.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gxhhwyqwo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gbbcacuvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gylclwleu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gboaahkza.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gjhhaypba.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gimzbefvs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gdrezgecy.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gzumiffac.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gbzafaqjo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gyssgbtsu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gprvgvyke.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gjvojxkzz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gnoxtujrl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gnebummty.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/geqpkhslt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gywaudige.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gwifgblab.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdyazymkk.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/grliuqxev.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gdjponuzv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ggqkbvrga.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/ghoqegmck.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gelfxreqf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gvlfsfaaf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gpmogclxp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gfemtcese.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gmczllhto.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gmhbbmvje.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gekzonsfa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gexjftbvw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gagdxgzqk.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gmejiqtxu.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gcluwdgdx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gimqsmkmz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gmsohiigb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gfciswnpn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/grhgqaimw.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/godjhklws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/goxmqkoyw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gognouozb.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/ghnxqukqu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfbeofsw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcckzbrac.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gduczshhd.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghppsvzrg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghautfglb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gcytzfbmu.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gfdlkcakm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gphqnufev.sHtML


<!-- 参考信息 -->