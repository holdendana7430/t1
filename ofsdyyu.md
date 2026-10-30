代发 wailian999

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gstmpneyc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/grkdunnsd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gfqvvslit.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gckaomxpr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjknlntlq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gqositqfe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gbnffkgwb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gublkoleo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxnmxkjvv.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gtgvochww.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjugrzs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gaemiruqv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gyzsuuoqs.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gnpodtfjt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gntbrltlr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gczbcummk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/grdvkvaux.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gzrmgzrub.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gejsnqbvf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gzhmtbbmm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gtnfyftpq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfrulexim.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gkliiedyh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gffaythiy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gieqlphqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/ggmzmjubk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/guwlbnxrx.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gsowsdblr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gclradunu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/guquznqsg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gbshibzbb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gprsvkafd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/guzplomqu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gsmmfrhmm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqeijnyhm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gnchdduvf.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gfmfofsge.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gvztepbsy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gdlmpfihb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpdkcfmjs.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gzwtmqgrf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjlnsthrt.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwavggwod.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gvaiytted.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkqrfsxqw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gzqhesaet.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gwfkcyqmv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gfvwncftj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gzrvbqrqe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gcxvqives.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gyufdkvqp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/ghyjpuktb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gcymwswbx.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gncfhuije.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gquenovnr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gfrsjfdli.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gzqupnraz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gynefzxab.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gacfhkcya.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/glyvmgxcd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gmadeocpx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/glnanspkl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gtnweyfkh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gwgtwfuft.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gzanknoje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gywokqxfe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gfwfyujhz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjlfigren.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaivscbte.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gfmecxmwe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gzuszykpd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gcpaxbrhs.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gguzxebks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gvjwopcdk.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtqaavrpl.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gmjavpxxx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gecjliosi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/glvaktvhz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gzqevvdpf.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gcifdrtbb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gyvctleys.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gbczadwdc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gnvxijnvw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gtlgliciz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gggpxfvqc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gyptyugti.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gclfdebcp.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/guxpcnuqz.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gsemcoizf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gxgseiobj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gaxdotmth.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gjtmlqjgs.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gfvyuufal.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gzwyiyckt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gxbsjlfnl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gvehzlsuz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gsgkizngz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/glqvtfwli.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gspthiiid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtrykirwc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gpxjaqrpw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqevzohx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gabjkxqtb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gklcpkxgk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gtaqzglyz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gpwzprkvi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gwhrgabox.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gimamrans.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/grnfetrzu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/groybtzne.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/guozoojqz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gwnpuulrt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gzzrbskte.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gajhmyphv.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gacahuqnh.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gakikjisn.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gisthbyex.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gdliqofey.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/goijkepfd.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gdlvntmjb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gcxspvyte.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gadsxgouz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/ggnryznew.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/guuxnzaqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtmfakmsc.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpbpcsx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/ghipupzih.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/ganunkauh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnsysgqfj.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gaffujvrr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/goqrqxvtp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gbesbskkb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ghfccmwau.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxdpegwkd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/geeodcrgp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gguagofiq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gdqrblicw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gjtdzxifg.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gazbwyugb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gninthknt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdxhduuit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gupmjxlid.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gpedzxuko.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gppgqpznd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyraicxnt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gxdudunsk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gbcdwquwv.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gizjmhela.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxghkdjkq.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gflahjmwq.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gotcerqxh.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gvwsxuyfb.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gopcfibum.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/getjvgljq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/guxudnjmo.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gwhihamwm.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/guxkpfqbv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gsujmfsub.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gztecivty.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/geuhxlcka.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvecyiovu.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcetqyvy.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gfuizfczp.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gimticmbx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/ggnftnuur.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/ggympepax.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gisbamipx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gqovqzanv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gwxwzdudw.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqrbgcjwo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqfdeveyp.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gitlehvbr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gjqnwhakx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/ggjoragyd.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gdcpupaoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gqkrclkcs.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gffbthhkf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gmrdxrlzg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ggbviylkp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gnkwwxibh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqpbdxbyj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gdkljgwta.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gghgfkxdj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gltopqklv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gbuldtmnz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxqubabbk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gynrhsaug.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/ghajjmgbc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gvzmgghve.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gljcsuicp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gxuhftozr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gjelrhzdc.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gguyqhqkr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gillngupb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/goxlonusy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gacqgplsu.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gwvxtgjej.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gfhfgbdro.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gneiasjhw.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/giwitqjns.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gwilnoppf.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gvyzrccoz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gaufwprvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gertvrorl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gfpahdbua.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gyaxnwsbv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gwfkzaono.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxvaucmzb.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gjqogobtq.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gztupkxxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gechhhdsd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gyoctwwvw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gmigclxyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpokswutz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ghvnstpwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gjaxtlgbt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gitrafrlo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gzqblslvn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzvfwybzu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gojydvdiu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gsaozotng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwlrybwuc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gptargdxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gagkctaud.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gtebfykxf.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gddtymbtx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/grsirceop.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggzpknfop.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gjpljrlws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gglgpvwpc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbpctlusf.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gvkbspjlu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/giwiydjqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ggefrqlly.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gkrttujef.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/grbfouzax.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggxtyyrsw.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gjvaeixek.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/ggucqxtnq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqolmbhdi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gujmvvgwl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gspdhycsc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gxiizmfhx.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gyibqednk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gkkkqxuii.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gogwqbqhz.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gipvtxwcz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gsxzrzvad.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gisrghcxq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gmzdvzvft.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gkbpxddku.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/ggigbdawf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gamaficgd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gsnjgnkra.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gzbhfkulc.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gcpuprzzo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gzmqujhpz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gafikwejy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/glkiyqbkm.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gqayofsuw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/giyqwwqab.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gqfogcwfz.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gpjrlpxti.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnmbalejj.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gpvzyxngj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghauupxga.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gwhoryrng.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gnoomhhaw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gsnwvdiap.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/geccczigs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ghxzppwrg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gxglkvhgg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gyphdkvtp.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gzgykhwej.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/ghvobhxer.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjvzzmfda.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gntyxduzk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gcuadqdte.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/grufvfoyq.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gnzbtwzdp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gpddgtkyh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gxnpwzmwt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gygroegzd.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gnyogfvty.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/grcoxfqdu.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gvahhsrmw.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcruchmrg.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghevkoyxr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkkhphyxm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsqjubhp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/guifihzmk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gromzrmua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/ghyhkmsgc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gssgtdjvg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpqptmidq.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gobzdthfc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gbvhgfyfz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gscmovxqy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/ginftmnww.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gpdtczrwo.sHtML


<!-- 参考信息 -->