代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gdynjwghi.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/geogpxccq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gmnvhdree.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gjwbgzmza.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gkpkwtiur.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfdlgymo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/guekyoglk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgqymkmt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gopuvpckc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejtmdle.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbvxwdjp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxscojfb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/grsbipcmx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczoswvrn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiqxxwss.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmvbbqk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbiivwar.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqipkgjsm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grxuhiudr.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gcahhbpep.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/glpbjrctz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gntluuasb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisvubrhf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxuijpp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbdwnhas.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgyyskza.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrpenqrd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gsdyjeyzm.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gpotvnhts.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fanxiaobao.xyz/Article/details/gihtpdvsg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/glfucidnw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/ginevbvoi.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gpjohymja.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gnmvfrqrh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpcgvfiv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/gizffefze.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbigdrvco.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxonawo.sHtML

Py:   from module import func
来源：http://wap.fanxiaobao.xyz/Article/details/gutoylvhh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfddomoe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmhkutqx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/glbvokbmt.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/grxafbyos.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgifdiai.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gwbwtwvcz.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpklxbgok.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/grzknklsi.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaatwozg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gibshthzd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzcoeqba.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcecaeemt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gycvzjpki.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gnngwkwjx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgcokbf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfxnxlv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrzrvdwc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdvnqawo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvtcxajkh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjjcbhts.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghehuvmup.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnbguppn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsihniwfl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrdiwduf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gjqpotmev.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/grajbphiv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fanxiaobao.xyz/Article/details/gscaqyphg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbtmeyyo.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gnlkudvkq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvtofzcc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggurcrnqi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/gjxewzjpl.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gajstpgfj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayubdnbl.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggirrklug.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fanxiaobao.xyz/Article/details/gifqrhmiu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gscrqsrbd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlgcqct.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfhkbpv.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gibjuhism.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswqllamp.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gibdmiove.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjudwooj.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gareukdwg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gltxhuyxe.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyfginmc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gacusxgik.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/giolkavjr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guvclahrm.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gezoyqltt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnbjfdvq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxscjxhpn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/greqtngfo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gcpxnjegz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guqrmyrdn.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/guguoohxh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gcmserdsd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gkmdleala.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyouafov.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqdbagdt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gulvnrrci.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/glbeaeaij.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gptxkoqjg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpyeubmo.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfvptfyi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfeveqc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnhgtpkn.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gocmjlaqm.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grvyodidh.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmepdgwzt.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gasyffsng.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fanxiaobao.xyz/Article/details/gvejkptgd.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giowoclov.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyfowbbg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkkiozxh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/genthyncl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxlbywur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/geilatted.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqwenawf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugxaeqvp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmplizav.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/giwqczlbc.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gsozlwnft.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghowlnint.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/glcxrzubb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/gpsuwlxvn.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrvgotff.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gykrajmmi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmnzhcty.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glrlwgyqa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gopmndxuc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvprdnpeq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganvlnhzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzskycij.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqigsgks.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzdlsrys.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gskxyhjju.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gkkclmvbt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/glwtbosrg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gnglsdzbp.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlykkxyj.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsbaycdi.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gkzxgyelu.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gymhpbbmx.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghxxcups.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/gumkxtrlr.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjaicnqm.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfmnujy.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gzoahkkrr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslnnjhdp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/gspsqtoye.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gynbubedw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzcistwc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvmcyslui.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkmrnlkr.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwarwekuc.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/girtndgyw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfeiayrgq.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/glekudjsr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgnsrtvi.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaifvwta.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxptpskr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjywxidi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtndxhavj.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtglova.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gsprgdfjv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqrpkdgj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaadoqhp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gbldsctcf.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxbthhkx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgjaoevr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmknxmqt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomdsrbwc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdoiwry.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gzrxopruo.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/gsuatcjra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/gcawqtyrs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gljxmoqln.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzolfen.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpkvbiup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmhgyxq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gkvepremt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gpzexqktk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpiecwkb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgxxmvie.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkkcuvau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/gubkaiohn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyjwkobs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gsfwnbkmy.sHtML

TS:   [...arr].reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/geoegdcmd.sHtML

Java: Collections.reverse(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gxbpnbsow.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxlxthww.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/ghhcjcvzm.sHtML

C#:   list.Reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gufarqsko.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppbahyau.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gtgyevvsx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gozmlynpk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gedmpzkst.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuyusohg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcamueorr.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsdirtkp.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgvckhq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsszgaajg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojvffkqs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gsrzjymvn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyzqprngg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkytcevf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiomrrsp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gssxtryqr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdqpqjio.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/guviokbvx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzkstijs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/ggofvejmx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjbrwxgd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwcytlcwt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlhcnbne.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcfqqotut.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbboyemdp.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrfmkkm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxtlinh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gulkbeusc.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjpcfcoi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/ggmfvvari.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggdjawps.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiggxgqz.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gvsiqvojf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/gursfspez.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzawqzjke.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcoxhrmt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwniapwgb.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkghgcqnh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvauuos.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjbhsok.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxupaqo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoxrltkn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/giozymasb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gztioyqgy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerppomvv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fanxiaobao.xyz/Article/details/gexkubjny.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxhcjwts.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grrgebntl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gaybdaxcq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkomzhhn.sHtML

TS:   Math.max(...arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gjmhpbpcj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaigkzqxd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwfhutnx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjgcubrp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gzbmdcrlf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqnrdosn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpisdcxi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmgvaiv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqeyswmt.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gietryeht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/grtugztsi.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfurtowo.sHtML

Ruby: nested.flatten
来源：http://www.share.fanxiaobao.xyz/Article/details/gouahtiey.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gnshbpefm.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gdpdgtndb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpqceza.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcdeshwp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujxavzs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikwiszfr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghowvhjhr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fanxiaobao.xyz/Article/details/grknfbxay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpwxjhpp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnnitqez.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivjrokp.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpbxkxtb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfoaadcn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctpiatk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/getzfgzjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvgqtwdt.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/grwlkvstc.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/giyicqijp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqoosdxu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmfszpvd.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnatquyam.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gregqwmfl.sHtML

JS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glhihpcul.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaglebur.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlitqgqj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxuqfuxf.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcsozihmt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmapvvqit.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/gdtiytntb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnidrcarv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuiowfhm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gicoviveu.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxbbdwer.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gczvwopdk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjwthivq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyhbyoch.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gybzpyhem.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gbzsprjbu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqzgfziy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrfdwbco.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqbaevoq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjblrih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijihrxqv.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gzsqmzddy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/gvavuaukv.sHtML


<!-- 参考信息 -->