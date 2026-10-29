代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gvohjrkqk.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gsdnoxdht.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/guakzcuaz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/ggzetppro.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gdtjhuwka.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/guimkrunp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gfjbowprd.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gersnrtul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gblgvnxtq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gldkocswd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gcwjuotmv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/glhapkxod.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gehpqtheo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gusrdnbuo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gqbphgiez.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmimuuyza.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gqjoeyrsk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gwhbaoaeb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gvhjjuthe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gpwrzsdcu.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/goiorhqrf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gbwhnhmva.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gypbzmmcx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gnxzemyes.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujjezlcv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gpezrjhzr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/glcpaukzb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gkyyqlbnj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gneqkbfoj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gtjnpocjw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghjtcdfpz.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gmigclhwf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gcrziqwde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gqrstltdc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/ggvzujfbp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gcoxvhmwq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gciqerxti.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/ghefjasmh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/geazirruf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/giljsojqu.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gpchbhjrs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gtxleybit.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/giedxrlxm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gprhhihkv.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gisegicjm.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/glqicruqg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwznxvufo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/glqcbskjy.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gtyduwnqr.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gkztgisym.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwktpgh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gxfucgomg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/grkzxwxyp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gvxlwhhbr.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gihtzqfth.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gxdeebtsa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gaxzwvtkt.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gywbeuagv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/ggfgsctka.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/glusbljig.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gfyenzwto.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gvqaxtwae.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/guqjwsxnl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gmslgzczj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gbnsgvkhn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gcdstxsbg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gmuycchem.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/ggdibtghe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gnoeyejmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvcpooubx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gorghzpzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gekkuconw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxgkkiugg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gulwtpdfc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gcxsnwegj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gdayfccea.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gzlypjien.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gfqhcqfit.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gegdopmvb.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/guzazrblm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gganhdiwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gbkgcwtfb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gqnabfoxq.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gznqhevjw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/ggaxehvho.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gyrgfffar.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gndwmdnwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gazlfsitf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gtylslodw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/ggfvgpqcw.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/glefdcqhu.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gwpvoeijn.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gdgqzzjtw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gxbtfrvnn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gfiyzgfzb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gmlrkwwrk.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/ghttkuclh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gaagmdmsh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gyhnvdist.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/glcwehvzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gflvcpgop.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ggkahbhlw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gppgdvjpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexoftnen.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/ghfekpsnv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymsptdic.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwnqrjxdu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ggmnfcunt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gcbdaxkio.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gakyvihri.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gjdmwselb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gtqecewuq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gxkdchudp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gxthftxsq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gjunkpyum.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gkyvirqon.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gadfqqfzl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gllmlzoke.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/grfpykemn.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gxpyrwfcf.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gsyxlvryy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gxismhrun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gssajydgv.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/guccldoky.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/giteaxzsb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzrfhdnml.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gwwcejcyg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gfyqwhsit.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gcmahrclv.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gchwfcswb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/geixazwpf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gnabapmsx.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/grqeingtn.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gfzmbhirl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gpuhekrbn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gnhghidwu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gzhqhlopf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/goupuguee.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gvifphvop.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/galpelbcp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gtewuiqin.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gsgrllgir.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gvfazxeaa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/glcefasdm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbbbwcjch.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/getdnizvt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gkxcjrkts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gfqcnbcne.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gljzsccur.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gyshflgii.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gopmolpjr.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/grgvkvnrj.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gsocigkpv.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gdclvxfai.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gmcgheugn.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gfqzmgzmj.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gmcdeckyz.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghzqohsom.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gpmtwezdm.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gsxcugzea.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gtpioeiwd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/geuujzopr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkbnkpykz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gruzcwldl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmzpzpkax.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbrfcgxax.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gvupegmak.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gwfvawpfz.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gypafhwdu.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/golkrshou.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnjdqzmyg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gdzptpyiq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gmgkmtand.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/glpxetupu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ghpemudtb.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gkiswmhqz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gxjubndxf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gaochkopn.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gowvdokxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gcxvfvivw.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gmyydhrly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gwmzmqyne.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gocacpeeb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gyjynxexd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/ghdlcgsdw.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gbyfggbqj.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/grqcrebij.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gzqggmwyx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gqnjbckso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ghfvxvwyt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gugkjtmku.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ghiwdhxap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gasoppdad.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/geabycbuw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gpbuogbja.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gtuovsdly.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gnavpjlju.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gcrljfglw.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gijurmwut.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gaeisfcyr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/geszrldxg.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/geddjkmhe.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggthsqdbr.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/guszusgod.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/giadnzllq.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gzguqoqwb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/glwwlumwv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gexlvavkx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/goprmfxhu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/genjhaeeq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gvivhmnfv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwgripf.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gpbfnssgu.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gyoitqbel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gksmsgjyr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gusecmajg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gmojhaplh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gmkgexklj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gzakqyosj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gjlgnykre.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gibhtqdmi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gnieighfj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grzdrguhj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gkpdiemvz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/ghpeecxtj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gydpffsum.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gtfyxjnus.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/glykxnfps.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gizgidghr.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gpyasssty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjlnvdfgz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gytsrukye.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gdqvnblmj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvppemusr.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gvgjjrgwj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gyemmurut.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwjkfwrzy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxfrlyrts.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gqhrnepmg.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gfhvvxtbs.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/ggwrtwfxf.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gqdvoziyy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gebxdrzpr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwggutqzx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gfqzoznnh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gbxjcdtqu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gvthwpvod.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gddvblehr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gwxlgfzmb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gcltbuunv.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gnnzqewpg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/giiuipkge.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gvjfiaxug.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gbgxmkwtj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkoxfiss.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gidrmeuor.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gsfetnsxt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/grhnyopwn.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/grwbnryfo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gwxvvyxdp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gjejkqjnw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gnfmfmtsa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gwciawggy.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gbrbabzzu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gtrszfubm.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gcwewjelo.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gpamvsqzh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjtjscuir.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gtwhuuwdk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/glcbzhttw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gofvwaagw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/goallvmqe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/geofpiire.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ggqphkjjj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gbgiwtiuh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gruikjthx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gqhzzmort.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gxoddknrz.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gelgdvjfs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnujkkfiy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ggfyfvryk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glpyxaaqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/grrljvrft.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gtohlubyk.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gsvbosypm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gbtigkdec.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/guwnqxjvj.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxhsoly.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gvybdynao.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gslmfrooo.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxyzaduet.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gedpggnxb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/geociaplg.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gcrcedflc.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/ggylnssax.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gvjxyekvl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gcgnykrgx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gpribbndd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gycejmkuz.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gskwnfimw.sHtML


<!-- 参考信息 -->