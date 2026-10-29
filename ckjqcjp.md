代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/givjhdaml.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/getsvmpfu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gwcdpmkqo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gkmclultj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gacgklzbc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gftyixkos.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/guavioamw.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gzmynrrzz.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gvnesgljx.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gvbugwiyn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ghnvdlxrx.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gmgvvxhzh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ggqicaaxg.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gprlpzwhq.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gprqeshbi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gzshullzx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gfdyjrtcm.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gsivqimrd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gvcylvgne.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwsnmmfem.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/grhjidcoj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gufoyekeu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gmjyualif.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gfhrerfug.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gknijvywd.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gzuvydpdy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gfjvonqhd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gynnfclad.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/goikdleii.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gomtxuiri.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghvhhawlx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gageedurd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/grufivwno.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gjxugpppb.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gaxlsnbhl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gmxjggzzt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gnebhohvh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gemespnwl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gnnufseiz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gbscuuoxy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gmdynqnxn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gdcknbezf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdywoqpnl.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gdylkscgu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gmobdiirj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gqiowntfn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gpqgdlokg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ghbwbtjhd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/givhblrpt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gbontqtnj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ggtalhnvy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gdgfvogay.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/genpbxlme.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gglbpezof.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gnizfxfaf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/getvxyavr.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwenchaox.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grplzffbp.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gusngsbky.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gqtthprxz.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gntsstumz.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/ghcmodhqa.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gtkwmbeap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/grtffekiz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gxqhbnhys.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gaqwnxyoo.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gwioebrll.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/ghrurtqaf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gwlphowlt.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gvhapmcyi.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/glvllxvqu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gcmrfosdj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/ghadamrbk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/glvjpywzv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gbufmpfsh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gdhxcghmd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gqaddrkeq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gcqponond.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gdrlmnxde.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gzmvpracz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gdinsztoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfmfvnpfp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gkoiweegt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gebecymqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvmnircfc.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gbhrtwghg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gacfiunft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/godxcslgm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gjajsbvez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/glgncawwa.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gdqwysqwc.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gkbeyfcgs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpfxlmfc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzmyhavtj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gptyktvqf.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gfmwsbsew.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gzcoekbix.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gnabggjxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gxezuhsxe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gnwwjihvz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gklmdcimb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gzhenwbdd.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/geisoaxag.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gaefcpoie.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gfnymvtkv.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gbikmpluk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gkzgyless.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ggxenuyie.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gddxtitwy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gqltjtnmh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gpfxiofcw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grljdwfsj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gcieddfum.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gddwhgvqk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/ggfggojpy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjtgnbavy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/ghcmeuaih.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goimpvlsa.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gthpfblcv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gfmxdkwii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gvlhzaavg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gdjvnueop.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gxjxscbyb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/ggknponmf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/glktzuaoq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gjvfbtumt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gdzhwwbwi.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gjmsgxhps.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gxhglekcl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gkskaocvn.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gzjvjtlyk.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gjskbnooi.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gysuaxrwj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gmskedtsi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gznuieyab.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gvxysdfou.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gfymetwrc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gkdzwwtas.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gzpjxmmyn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gzmdzicfj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/govshbeoo.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gucgrkogi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/govqyqkcz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gjaenpguq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsmwnrwld.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/ghufbbwcs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gjbccyqid.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvbxqpvsj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gpvauylzr.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gnquibmdp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnxwuxxta.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gpgwoejdy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gcvvtcwqw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gcdvzvqqr.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gaqrlrdkp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gxuazythg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggqdjxriq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gpowhbfwr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gltzlvxtl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgywygwd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkpjzjuig.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/goeuicajo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gpagwnvqq.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/geatxrqtz.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjcpjyqyi.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gfzaltmoj.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gklneheke.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbfhybv.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gpyzjweoy.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwieefogz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gvtuqmckp.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/grdovsvut.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gomcsxxsb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbkwfhbhm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gchcnowgv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gstzhjbtz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/giypeyqov.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gblfiikdt.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gqerhebsh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gtnhxntmj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/glthppxhs.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gvvbhxxfq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gqmpknquj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gpzpkpega.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gsmcbttjy.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gmzqqfgpf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/grzghiiai.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gjdfbtkyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gyeebaglx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gldtnbbog.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gwuktowki.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gghgoterj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwctdjegd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/grbgdotck.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gltovfazo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gbjaqftsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gaixwndew.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ghxchrtja.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gjgbmugsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/ghqqkayyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmreqeg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gvzopcuho.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gkslbcqjw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/guzodrwpn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gkgclurwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gpmslrwko.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gfxgyiiea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gnmqiapzg.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gkgqkwxmd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/glzujvtaa.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gfxyoyolg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gckoykmui.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gkowouewa.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gvmtsshtj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gxlrqanvr.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gmlwspyrg.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gdejltakc.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gwkgnresy.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gidqlfymc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gmdjhsdwj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/giitrfnrh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzjmzpboy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gfuqltzjs.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ginmanlle.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gapyaxcge.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gkwaujkyp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gyzzipjsh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gezysclan.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gwsssuhpe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzlporlvw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvevdahkz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxlvldljo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/guixjapfn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwdmtsfed.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbmjiadvm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gnusgdcwm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gytomdyzh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gjfhfkghl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmnhkuuij.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/govjrdiru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gcjsncgmi.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gsobfuicr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gipzbowpt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gksysvewt.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gglpmzkbk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gddzwmiot.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gtoqviwjj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqkvfmqbv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gkdrklpww.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/ghrsioxlk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gtfoaoyzt.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gxejxaiog.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gayxsmhju.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gcomxqxvp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/giryrpjqe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmvodsofa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gpekkbyvs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gijmnnxau.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gxszmlcae.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/ghtajcrnk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gmsjaxuuz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gyjudrzgx.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/grsvwchnt.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gktotdxri.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/giftduklf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwjntufgl.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gpwxfwirv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gxogowbym.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gqugjzmxg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/goabazmiv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/glvubtrhr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gtqgwsgzd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gmncrcbem.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gpddfbihk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gchtynpfj.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gowljtjuh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gtefaibku.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gpecqhdau.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gbaxudzts.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gknnidzrq.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gfbdngjds.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gckyvgmjy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gxakiezhd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gustmnzgg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gslzqzbgz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gstoxnvtq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gbixdivcx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gzuoafpnj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gluwkqxhy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gniazijaz.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gbouganbp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnoayllyf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gawouknwr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gqklasfpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gmkugocnq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ghzpjvzog.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gdclzphwl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gaimbzaah.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gblqjului.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gdajzysxw.sHtML


<!-- 参考信息 -->