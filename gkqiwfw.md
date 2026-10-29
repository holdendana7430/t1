代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gyoynyqlr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gueptfbto.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/ginpetccn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gresnlkau.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gkxouceel.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtpeqmamn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gqopkaxde.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/goyubmeva.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gkkkignix.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gxesbjoty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gzlsxlivf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gyjwtpkmb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gytvhphsv.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gbgkxqyed.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gztyxccli.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/goumrhnuv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gepggpxor.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/ggjdwctot.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gmqagvpvf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gtzslbrsh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/glnqrxxdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gezcqiafc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gonbipguq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/garvydxvl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gdbwjirsm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gpafvbmfb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gzpcutiyb.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gjyokyngo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gjigobgpi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghmklhynd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gocnwdyyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/geqkswsnt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gxiwqjgjk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gbozudgzb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdqipbjgq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gqbiqlbof.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/guntrbmkx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/giirshoyp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gxssjlsmq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmnvsirro.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gustxqycs.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gfbkoxzot.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdgwzkivv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gcqxbybby.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzddiilqo.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gnvwvdtwx.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/grocdjiif.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gximsxhnp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbamcdwep.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gjehaysnx.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gxhovmgws.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gaunmvoqv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gvuaufukz.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gfzictcrs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ggmodpsmj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gimvkbako.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfaiweb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gomghezvs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gtthfxchv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gziqelffg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gssfedvnn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gttzwcasv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gbkhnpbia.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gwogqnziw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/giehrcgsg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gmqmoklxm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gffpynzxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glfcrgwli.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtpitrisf.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gocwzfejf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gssyrheow.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gmqlyhkig.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gptxjzyin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gjfdmrgyv.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gohxboexc.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwubpmzgn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gxgtefzaw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gugoylhge.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gyhshxhrt.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gvjnebiof.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/ggjxdqcnt.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gjufgnjoy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gbresbdds.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gsrdxfbtd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gbqfpjqha.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gbspikcvp.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gqmwxdxvt.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gcqniagae.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gbycrrswj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gwmakixik.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gaphoyoxb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gbodipomn.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gqbzzzzen.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gnopuyrkx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gfuxtwttd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjudhzzuw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gyrsprbne.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/grflxsexu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/goidjvlit.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gisvjyyep.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gmwndsukh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghjosknvl.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gegwwtxyj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/glqmmiymo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/ggkjknyzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gqvcbavjf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gfmbszgas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gxadgvdlx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gaqlvviis.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gsibeukmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gukbuonkn.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gikrabghe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gugvdewab.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/grglubanp.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkcdjninf.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gggxfbpmp.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gxspmipoa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqhmewxvn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gfwwrnpul.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gunwshyud.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gkaffjoti.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/glmkdzuff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gotbfbivn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gagfxwfgx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/giqpxpxyg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjyozcflh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/ghmxqyuzk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gxqhlpubi.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gcirvtzca.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gbdtystci.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghtvnzmtb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gywqtkwuz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gqhlropzj.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gdbwkdxgx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gvdaebnxy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gjbzrkazn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gjwveabke.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/glycpddgo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gmldwuobc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gredbyxxw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdvexgihe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkvgxzxof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gvicuxmwi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gkfkqcdwe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gkaslttaf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gvaqdszsd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gycwdmdnh.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gzlxfrufg.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glxrblimk.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gfjwdxucz.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gyejogvzu.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/guqcyszld.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/grbdrjmyv.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjjzecark.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/ggtrnoadt.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gyjltcvxy.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gfusbnixr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gsarmfxll.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gfuaqgmcm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gpnnvlgqp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/getlxvbtx.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gndkbxtla.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/goucjwzuc.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gubzptgky.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gzkitylwp.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gzsomzmcb.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gtejxqhbx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/golwsjgbj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gdsfusnyl.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gbhzeylbs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gwphygrks.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/ghgsvlrzr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gjytuahcn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjrflbgla.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gcjnvolsv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gjpipmycj.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gobosvkca.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gprmbreva.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gwsmeborf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gqyrkmqcq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkdkgasre.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gpedbdpub.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gmvhclzdu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqjrljvwa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ghzramapi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gxnjdzopi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gmxiscxze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gzsvtpyoi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gyzsqzvyv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gljklzzia.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gjczmvtjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/giwxopmms.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gcqxnahwk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtrjvizjg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gbvgmmycn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/godkefagg.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gmdsbezuf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gvuzxqsfo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gyrrexqbo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gtunltufw.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gsmwnccsh.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gdagwyctc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gcckalkff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/giamigfqz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gyccdkzzv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gcvynkhak.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gthnhurgu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/glxgxahkq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gytyzctdp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/goqgwuvyj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gqlxfwdrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/guetndcsq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gvtyzaztk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gocxpclwb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gxwhufsba.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gezdrqaqe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gbsohimip.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gujdnfkgf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcbpveetg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gcpufxrwa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/giwqmcyvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gawrwilhh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcfokkpmz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gozxfoomk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gckkrgiwp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gkjwrxqwm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdbkejath.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfbxtygdy.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gncvjynxl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/grlonguvp.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gjuluzrgm.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbwddzxwc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gyhfujrii.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gpngxqhtm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gocujsuru.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/ghieukjse.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gsfuzbsfj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gxjipnivg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gywuwymyn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/glwxlybae.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/grwgyednx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjlskllaa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gimdzhyos.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gmfmwfmqf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gzyxufgcu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gdddhcjcf.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gtrjikvdg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gatnxcvxg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gzmoidyjy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gayxozduu.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gklbgqwuw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gieokizvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqpuwitub.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gpzscsprn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gbuybogrq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gqqgznunq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gjfciatzn.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gkeytmpwy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/glhhrrwjf.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gdldixtrw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gyifayfdf.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gozgvsuyb.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gswmovuos.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gurxrbysg.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gejqkcprd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gekqizlvz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gkyykietg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gwmzabzmx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gadprvagf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gdsafggtn.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gjowtguce.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gxbczsomu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gvamikdvv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gwgdrmjlj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaovcfyaa.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glawgmugl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gbjztifzk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvbgjyjgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gqadriaxy.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gfmuodzsa.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/glgxvnvwn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gsixowxty.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gasqpyabk.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gtskekknk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gtbeapnrr.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gebbwngkp.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gmbngyxcw.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gefrrcyqx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvoqrkxri.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gabkpkcmf.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gkpzrncjt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gzayjdsdt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gaokkhdwx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gtabnfiqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gegnmixxg.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ggvukvhed.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gzzkdaasi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gejlomeis.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gkttslamm.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gvdhcvmfi.sHtML


<!-- 参考信息 -->