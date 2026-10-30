代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/ggdimflkr.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/ghqhehccu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gddonwgzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gaeyjktqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gxyxdqbiu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gulsgliai.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gkaztdojg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gngtuxpkn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gzqbtxrlb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gpxvmwzlg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gvwikxoew.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/grauixtmd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/guslffeii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gghxiegcc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gkodcgmkt.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gtphiooci.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gnzlehfvz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gmodxlhbx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gnebuupih.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gzahpnauw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ggvzdavsh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gruftqzwa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gwndmzgzt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvjswxrvp.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gbnziupnp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/guyeivbkk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gnnqpumja.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/glglyztij.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gspbkccek.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqtakumoy.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gstkcfiku.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gmsaqvokq.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/ghbcydhkf.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gzrswhnue.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gqtackmjo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gqgvwmwee.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gbtodytnu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gccimpsab.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gyrugyzfs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/glssfxmwc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/govkfxluh.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gxscnkyft.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gtzfzjvcw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gifysddcl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/guvhzerjg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/galffjmzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gezevcczr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gllnlzkgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/ggbasovhk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/garrcduzk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpvghgpqf.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gptcyhxnb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gxzyqxuhe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhkqovae.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gtavskcxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjlrinfqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzkyfoetb.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gbqpblsez.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/ghsztulrk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/giqlzcfgj.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/grdrrutym.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/ghvyvvptg.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gjsednhkp.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gwstmtbvr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gxdwhmgip.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gfrzwzahl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/grzmeqwwb.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gleiukdxf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gclgvclzv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gweamwsxm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gmjnacsdf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gmmthwwrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngkoaozx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gbtcueszt.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gnplebpol.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gzkmqssbe.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gumpiheee.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gwxnnukda.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gqtykfelp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gaoiyhvss.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gjpcljjxl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gdxeltfhi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gnjjycnmb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gyemsvoks.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gbthflhyy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gukgwqzog.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gpqnhinnk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gizumoddg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/ghuoyailk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gparcyfou.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gsstesmdu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gwifldkxb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ggfaeqmtj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gjuxohpxj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gturxrudz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gcdndqlcq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ghawzudww.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gbwoiwwcg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gvbjahwmh.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/goufjwokp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gxagkksny.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/ghpnxurff.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gctuxbnuh.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbtnrlluj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gydpwglar.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gcqprevfj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gvdrtjyaf.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gunnqiinl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gigqhqnuo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gjjzxkbru.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gdiqhrcqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gzcfvjtvy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkeomtzss.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbwnrlqoo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gvgnlgvni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gzzuxkxij.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbyklfoyt.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gzfvjeiyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gforgpqps.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtuxztqwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gdkqgkjxs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gxytjzgyn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gilwsxvpf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gqdkeftzh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ghbqrpxsh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gidcrbjqs.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gwelcahby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gajuviise.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gimzpkdlz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkxyhktkk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gjcjzobze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gqgwmfoxy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gxwjptjvh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gxpurwktm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/glssypxlz.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtbcixare.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glpkurhke.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gjqejfinn.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/glxawabht.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtzmtscze.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/ggdncfwsj.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gjtbumibd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gfzztirag.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gxqrqfxfx.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwjamxlfr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gwejtvjaq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmotgjgxb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaybeweal.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggggeghhm.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfytcjrzd.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/griwztnyh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/glvldaars.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggmwqsejb.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gtacbgwkh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gwopndmyx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gelfozhuw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gzlmlhkld.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gaobkqtdc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gdbflqqcz.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gcmizzbzt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/ghrdftqcp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/goretjmcz.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gfbwiondg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gblmiqsfl.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gymrlpxql.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gddsjmoel.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gediidzca.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gfbxpzirm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gtrjftqaz.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gvxqvnmkt.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gjuvnpell.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gfhucqbqz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gtakcrwvr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gzaozgvoi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbzgyecbq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gumbshxws.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gzwfbdfqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gejgqufxf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gecdzachj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gtyqgkdqr.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gwgoizswo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ggiasuztt.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqviodbpg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gvyrdmowt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gfafitncc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/grwiyhuah.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gxugzkmva.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gbpexudxx.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gbzevrbvi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gqwrblzvn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gbnpctpbd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdiqjbfcp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gnnyxhzzz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gafzbhlgd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gvdfzgiya.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggchbwmfe.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gzthbnpou.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gpnomdejx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gjwflzrkc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/giywxzujv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gckafytjn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gwfqbdxlz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjpsyuuhd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gtdbbpmfc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gfkfkbqjr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gvfywprcj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpusmyshf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/giowgmmlg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/geshzyzlg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gysoaaawt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/guhbhfbkq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gfbhqvhad.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gwvgntfzw.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gxoevsczr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlohdmi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gatgvxmvj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gwqrerdxr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjxufrakx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsonzoqen.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gfmhkbmvr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/geljhchbv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqwhoab.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gsxtduhce.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/ggdzpgtyz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjsqqeuqr.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gtwymvegd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfecjfvhi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gokslehbe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtpvxubou.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/giipdpqfb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gatjbcdpk.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gremlhawk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ghospyhbf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/glsnenlhj.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/guzhqgnym.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gayrwvjte.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfehgbyey.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gwvngifzk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gphhifqtz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gevegainv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqnzlebav.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gieqtayqi.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gkqamcaey.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/giezydhmf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gxhryuqoe.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/ghxzvuemu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gnxytwmzv.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/grpozxoaj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gvwqdysqy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/ggjhampca.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gniuldtiq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggegcuvej.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gcbtwimdb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gzhuylyej.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gmckywevl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gqqdujwps.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gcuohfgup.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gvblihwau.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gyorwxemo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gzkqwbanx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gjprictsh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gifcmdrqb.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/geuwjtkmv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/guynubuju.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gkelfvknv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ggxxkfkgy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gatppqaos.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gpanqlcrv.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gdpyyyjmh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gjkpgwsfe.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gpbupcdfc.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gvvnesnqu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gxflvxavc.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gsjehgwid.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwhksyksy.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gsnyqmgpd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbrgmgwpa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gcuplxqco.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gxrjbawvv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gvsutoqkf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/ghdkyqptr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gerpzvidw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gnpvogcpz.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gvttpoukj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gdhcfdvsf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gfzdhlvmw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/goxqjngmu.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqaxwamhe.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gospxunzu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gxgkhmmhc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gujuvvkdm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbupbzric.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ganbigkze.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gggrrhmbk.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gilarqmer.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gibpnzyka.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gaogjuikz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gjaepuxrm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/grhmwtpnv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gduyuitcp.sHtML


<!-- 参考信息 -->