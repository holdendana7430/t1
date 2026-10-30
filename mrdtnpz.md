代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gpoqjesuc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gflmmoovk.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gmffdkrod.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gskvymatb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gqkwtputw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghphkerbi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gohynzdgl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gcmxesuyq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gpwfxxndo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/ghgevjqkn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gaxwovlfi.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gvvjzsvnt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdiltuvkg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gyclgtanp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gcnayqbkz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzifebtvh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gsdgqsgqd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gchcgbllo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtwlangdj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/glawxvkrc.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gweiyhqcp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gidaoxkrx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gyyqgkxqd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghrnlamzg.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gisdbijqv.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gsbpiufuz.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gvcjegqya.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gsfzkvrzj.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdhubypxx.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gimcfinmd.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gblgyhjhy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/garcvqavw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gjxmyhyte.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/grwbrtpmr.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gpzdupzty.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gyxyptaui.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gswfkcoeq.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gsakccdbk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gjhyijbmu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gfeundpbh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gerdsaona.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghxfbpons.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gggpesguf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gshxwlclr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gucdaqmti.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/grvaxhqqv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/golrhrzyw.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/ggakqfpkg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gzziaebpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvpgswaij.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gbjvkmzwb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gedfgcumv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpbkkvedi.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/ghuffffhs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gjcobgkti.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gelrxdydt.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gbbxghnen.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gpwnecznt.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ggomksgaa.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gstlebnpp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gershfbdq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gmkvjhnak.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gepefuzwu.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/godmltnas.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gbcibdhui.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gnanjjxai.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gjhpnxugg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gdqyeanln.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghbugicci.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxgulqkec.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gfnslgaui.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gikerxcyz.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gvzsplgdh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gaolrltpg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/ggwecomsg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/grbjjvonw.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gepyjrcvp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/goeekdoaw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gfulkhhrz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggvnchtqd.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/garrrrawi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gzkioaptg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/ggeknfmob.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqkxxnkdm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/geqzqukce.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdzomkyab.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gpphxfltv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/ggfixdlsh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gqqlkxomk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gnzxiymyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gtbsfbcwr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/ghjzdfscb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gslyfbqwf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/guthsscpv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gphqldagn.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/grreiwaoq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gufklcoxh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gqmisrjcw.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gbhmejjdz.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gzvbwcach.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gvvctnfeo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbqagfzbt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gufcavwco.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ginpygmva.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gvsxjnukd.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gcocubrsv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gegifqliy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/ggjhlkmer.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gyavehpfs.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmpsjsbjb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gpimcmmmi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ggracjpqh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/guzctrexc.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gcqrbbhik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gwtufipnh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/ggmsphqef.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gnewjelpf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gbiywvieg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/guqmrqnpq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gzukhnacb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gfqcanosl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gpzfqtnia.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ghzqsppgk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gkanhslvs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfywbakum.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gbgtfdmtn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gestsyuza.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gkdwdzozg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gudurxeud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmggrzagq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gehmgomeb.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gtirxzkpt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/geggentst.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gsddaaovd.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gsoynukxs.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/grnckrhqx.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gktrelsdt.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gczyygsxx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gomnyjsjy.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gjyvkhnmt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gypbokfjc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/goiedrant.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gvtpkxuen.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gcuwgdcbi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghtdxkvim.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwdtowdnz.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gaiyzjikn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gsidsxhzd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/giwonujhe.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gbyggccxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gwwbllnas.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gwnkyzqak.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gctabvbsz.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/goacexcgu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghnlhqajw.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gepmhmgce.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gvdlecpug.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gfaxvjlhv.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gkxcxxtrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gvfnwqxwp.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gpewmachc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gbllkyivk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/glilparmp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gnqrgdstt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gcbkfodxf.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gfafkpldf.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gyqnlxtkl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gxqnuhiii.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gidoxdsxb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gcaetslxd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gbzqzsgre.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gigtziwsj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/ghumyhrwg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/goifzyyxw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/geghjozha.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gxqctvtyw.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gvhvrjpcv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gqbedjtfh.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gmckqsvpk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gggcmlega.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gzldwolul.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/ghcplopiy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gtkjjrglu.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gpiqkcwpj.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gnzmsxauk.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gzzoxoczs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gkdtepqnt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/glmmwevaa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gccvnocrq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gslenuraj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gzqqhurml.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwjxcnuxi.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gjlfmlmss.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gvncnieca.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gzicilxgj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gphvfmhzz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gwybtutgi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gimqcebyl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsfszagno.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/glgujldjs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gdngzzhyo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gbgzkuulj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnisbedkl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gnbimcvyp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gabouykpk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gtfjlqgbh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/giazqytrs.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gvvaggfbx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/geybmobel.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gjwvcwbqe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrusgqzd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gjujfibuy.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gnwkbksnl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gkofnjkgx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gmsvtydkj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/girgtczzz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbrtlvztm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/geabctdrb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gliklayde.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gutgrrxum.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gzshhmrcp.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gfxpgzzvf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpzkgzxns.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/ghuejpbuz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gnanbdqlx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmhjpasjj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gereygvdz.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gubuubmbx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gipxjfywu.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/glzzeovvp.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gaapypxgg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gokvzuult.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/glswcgabd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/grgwfelnh.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbkwhonft.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gvxjqglau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gdfawecjv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gruneyrba.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gogklccfd.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gstmkaare.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gqwgdbdfz.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ghyavbgld.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/glqzhwriw.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gwvcnmspc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gllzxznuo.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gvkvakhru.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gvdzhsiab.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxoaboqxd.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gekiaxlyk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gltlytmfr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gqekqbjbf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ggrwwrdyr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gaibsjkov.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gviserzyj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gzaoeiwwz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gukduwakp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gwsnwjtzu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/guvkjttgf.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkrqjxhwv.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghztqwlvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gtquohrtq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gostcqgqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gcpgewsdv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/ghzwffovl.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/grzqdqbnh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gaifgiadr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/grkhvcgza.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghmvundgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gburtgyul.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvuikhoqh.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gihmhjxst.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtpnxmyjc.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvxhezegg.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/grtrvnifr.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggsvbjwgm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtaloiboa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gslsiyugl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gvchxqedf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gnyoiesni.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjppswhae.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gtspmlmic.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gwseywdov.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gjefdaaks.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gjuzkufzn.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gixnqzcsw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gohuaeueh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdzoermav.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gphesgzsb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gysbhlzbo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gnfesslsa.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gmvunzsmu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gagikeetr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/giincpruc.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gfkiuktgi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gnphvjgma.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gaxlwymxi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gtjnxmxje.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtsszpnkj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gbctrcngm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbqjkgy.sHtML


<!-- 参考信息 -->