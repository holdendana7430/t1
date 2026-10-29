代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gmnytnrbz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gsxbkuqtc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gidtogcyx.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/glseyrzeo.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gfmumcsvt.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gkpsadeah.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggyarsfyx.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gtmtzbnse.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gaoklxiry.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gyewjtraz.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gpltyoboj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gsptlqkyp.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/ggtgemzrw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gmvdhiwdv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/guyqnotuj.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gmfjeotou.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcvnowg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gurnjonsp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gstuvlyxa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gdgqlfqks.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/grhutsrqf.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gpretexdn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gqfrbmtvh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpphfcxtd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gyhikosqi.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gfdhjuuae.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gcejmfsfe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gjeocoscg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gvavksriw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gfboiaszy.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/ghokkwwiy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gvwqsfmqc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gkpkojepk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghjbkjvka.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gnmsydnkb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/ghjpnkqkp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gucfrrawx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gwzbscrqc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gvruypulh.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/genztdpdk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gasnwmqwn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gtltnqplq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gttiyjzcy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gvtriebqm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gkcaoolha.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gnbtcskfy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/girlnppyb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gimvlpoci.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gdhlaavvz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrxwxtn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gkvzydylf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gphhpvsww.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gogcbnqah.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gmqrhxgvi.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gxwqllazm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gffqppsbl.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gwzflhxoa.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gzaebsnnu.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gjmcvxhts.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gojypisxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gvuthgrsd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/glhetprtm.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gxibmwyzn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/guirhxlik.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gkgksucir.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gdgmoqjpn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gqdeddhwb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gvzsivtjd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gsdbegejr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gbwhirise.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/giahgnxgi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gwzsonoun.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gvqbjrbfe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/guirtlapz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gvvyukzjx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gakltmeis.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/goftcxnvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grlsvxywo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gbhmjtwai.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grfkxmnxa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggygrwiun.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gcswglgex.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gcfagpbgj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gmaifidhz.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gdsmeaiyi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gkfvpqpct.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gcwfkkpqb.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gavfgxped.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gcfqkajmx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/ghuzyrnaa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gevaiowiy.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggutuuydu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/giefotnjs.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gmmmdwxng.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gwgxsowhv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gwamnzkgj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gqyqyympu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gpogeoohe.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gxenixxkg.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gefvkjuis.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gyvjaqjeb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gvokgoyqw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gbonrkxfh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gnujjnjjs.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ghmpccmhe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gykjmwdbx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/geqjlepdn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gxkwlhyzp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/grtklkool.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gfosruauz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gbwlrkryn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfkrauamn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gqsocyvra.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjtfxjivs.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gdqwcnjlw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gcjjjywoo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gglflpoij.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/giallsayi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gzdhcjkvf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gddvkppez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gxyahxsgj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gnmqqeawb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gyuesqqeg.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/ghmqnzoad.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gwudtalwg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gidztegfv.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gavvbxrag.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/giienaimg.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gvdrqimml.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gqqekjegk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gckbvrifl.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gtwapcyxj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gtyxmrcfy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gdyfypwil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gqlyosrag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/grqtbouap.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gorjnscnr.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gchlvfmcu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gadrsurhb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gbotcjnbt.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gqhjbuvac.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gsfnusohr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gganbqona.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjduocnpj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gfjsfvqje.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gkfobtycl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gcsqbfsky.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/ghvnlqqot.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gsblfzjlx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gxheeatyd.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gvsswkxyr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gpazrmcme.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/grfsbshjq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwgackxmz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gpmjzrxte.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gwkfuebjb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grkcrmfjy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/geoucmpxr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gliqbzynl.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/grjpzhzzz.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glynlbeuc.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gnzvmyilu.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ghjmmyfqc.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gfoyyceel.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/grfxaqfgj.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gemwvtgvk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gcnkmdhxx.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/geegxaqnf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/girtyzptc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gxwkxdetv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gosizrwpt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gncozgogj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gqhijtupy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/grntxgbzs.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gguunlgpb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/glggatybd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gweqzekhc.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gpikyrxoa.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gmwjssmcl.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gurpdgcqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gnugdpezk.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gzrzeccuq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpsapxbmz.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gyluzxqns.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/glsybxfws.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxwligxmr.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gxvjvkzqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gsvxrglnv.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gcoganlcv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gwckmguil.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gggxdpzzf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gcjzspfbc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gghsvgolr.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gpddccbhv.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gxxzygsvj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ggurmliwp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gkcoitkat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ganztiexe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gmqrokndo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/guwltjqmi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gijodtxdl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gwvbcqola.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gfhxwcdgg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gsnqcsxea.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/glrpferwc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gssqaqren.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gmqrfptqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gscplojcb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gebjbjyhz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gjprnaajb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gichbjpdq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdfruprgn.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/ggqvoxolp.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gdwmiewfp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/giojominy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gswubygho.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxmhranaa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gmvktukey.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gdeskshzf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdfqnlaog.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gmpgupvng.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gbiososho.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gmgvzsusz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gguwhjmiy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gwbkczlwk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gisluvxew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzxfewblg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guzmdnrfk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gpsryvdrb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gzysaqxba.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/grqylwcxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/glupopsct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gctmkjtbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqjlunxcz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gvbqhqppr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gaxigjsao.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gxtruemdp.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gtvyzpals.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gfhapudlg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/giixfgyfe.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gbrurfszw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/grsfqjwpg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gpxacimbg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnnhrxfjr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gpiixhoqt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gneulaauc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gahwbqctn.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gduygfrcj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gkykpvvmm.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gfkvtfbvl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gciorqqvt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvsxbiysw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/grzumpmfp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwgpklnys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/glvdwnyve.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gcixfurow.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzvewnyrq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gxuirdlhy.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/grvzncznr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/grvmpulwe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjrkhffxy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gwwdsouxn.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gybfkfbsn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gfjaaiepz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/glmxqmmhx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gvbkrqrdj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gxsnpflpt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghkquugyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gnqmlswam.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gdfpqtysu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/grybsfjqt.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/giajmsmqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtkvppqji.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gdnqrruou.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gfzokmzgd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfzhvhzer.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gkxhgkakl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gmltkxqzp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gzehievmc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gvdpnlceu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkchcgqha.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gdzloyatx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gwwrfubza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gvcuaqpoe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gbwzhlenm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gurefydxh.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gqnphyokx.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gqhwkaiyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gbarxwrbv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gapcntzwd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gfyvrpwoz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gydinvpvz.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gewcixxbd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gujkvxdcp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gqahlmjqv.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gnotmuesj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gackktved.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gadiwxhsp.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gvvyjdkfs.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gnnuejpqs.sHtML


<!-- 参考信息 -->