代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/grmvaimzn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghprcdvln.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxblowzde.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/guovhfjzs.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwpgoqrrs.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gygswjxfn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gwzshlkie.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/guyxuxcek.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gjvgkteqn.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ghcvmuohp.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtvxqwinn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/ghdxeuydv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/guvewihmr.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/ghypnouyp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gqoewfqaa.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gohlhtnfc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwarlcnns.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gkvlptwib.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gzralctpo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/giompnodt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/graidqkpy.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gblvzxior.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/glrgoorfo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmgvcnq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gakzqiybo.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/ghfngfmjw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/grzxiogcj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gxbhsdmac.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gvvstvhyz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gsmwwzjwx.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gbxqlxfox.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gikepggpp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfknlgjo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/glolqinse.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gliycycvl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/giyiwgoez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gebdnlmap.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gdxkrejqe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkstwmbpn.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gasiafmhf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gnxjkdrmc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/genrlhaiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gbnsclhkb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gwxznndbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gpndnixyh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gwtspfwej.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/geluvxokb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/grfntrtdm.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gcfpfznhd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/glftwkgnf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gjqvzvysb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/grhmthwpy.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/ghxmoqmrl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggvxcvxxm.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gxaogzsjs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gjbpzgrvj.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gfiwaftid.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/ggfgoymcz.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gjphcrdqu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gdsivhkwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gevzfwrqw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gvsbfixea.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gvajlfkvv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/glurjrlef.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gtrvbvxfm.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gpymkfazv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gtoylotbe.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/geqejdcux.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gcuydcvui.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gkjehilmu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gizsflquw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/giroimpap.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gmcjxnpzr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/guzcbvwup.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gnuvczdyx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gyuqnxaaf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gwjeeqius.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxreyuvur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gfubjdcmv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbngkikgk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdontjytd.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gkhacznoq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/ggcdocbka.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gdnhkjvyt.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gamntodfa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gfkrmbkqi.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gthibllme.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gvmirxyme.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gxxcsrvza.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/giretmxox.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gsuzuqnqz.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gksjpcbir.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gjyomkygz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/grdreanot.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/genffxbjl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/garggbgnb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gsyyxiniy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gspekgpam.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gmmhfnfjt.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gnpmtctti.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gndiunccw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gnfbybedz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gyzofyutk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gwwudvmeo.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gplqsimgp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gzxswuzrg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gopnixmps.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gibhtbwyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gunxqzthy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gkwmyhqxj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gjbjljjcn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkuviayal.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gdkekomva.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gprjjwgof.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gxciewwes.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gycfmzugo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gkqtsgyhn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcomuspag.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gcirnyjsi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gbxoqcvso.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/govkcbtfm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gloxnrtxh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gdsfbeugn.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gwfikqmxj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gbvhzlnnq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gxzuudgdn.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gjzflnzhy.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gkdzjvpfy.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gbbqvlvlh.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gpcihegla.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gstnpsoij.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gqeuhyqhu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gbufxmlqv.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/grrrgeoxy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gkxjkjslv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gmgfqwgni.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/guzjtgkae.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvsjhjawa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gbvbftsaw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gcurawubo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwuohvmrf.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gjsbkdzcn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gkdzfzuyj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvqrazwdc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/ghesuvghq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gmvgzchvq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gforydyle.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gvklgehqu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjrfwnyb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gxwkintnn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ghlgvubfn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gplkvhycz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gizxwtili.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gprusosjf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gkelvraui.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gophbzoyq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqrulaafs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gazeuxnzr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gtgnplvsd.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gusotlggg.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfduydalg.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/govwmdsld.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gockaxrub.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gguijoegx.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/govlzbsci.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gdhmtnhpt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ghymemqaj.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gibjitvqs.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gaqxzgwfv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gcscbkrdj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/grhqbzsek.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzgeevnfq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gznvanqfp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gdpdvlczi.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gcgguqvbr.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/ghtkbcrez.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gbmommvzp.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gonzugpsp.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gngfrraeq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gsycqpffo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/geejxanhc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgjacmt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gggfccrwh.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gghcorduw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gesniclde.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnfarcgqa.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gyzjetwvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gpsqzehle.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyvowmsuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/goehitwnp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gyiqjgjgi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gmiplnndd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gczllwlxp.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvfndfdjc.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gcphbgzrk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gjfonoaxf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpbfytauy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/ghmqjgblq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwgrrdkdt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gxxzbppho.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gcphbjtad.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gheykcxkz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/giuvaelos.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/ghxfwzzzt.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gudollzpl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gsrhgdpan.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/guhlitufo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gigfzlsza.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gaowfwbfy.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gsftyyivm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/garycalug.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdtujelnb.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gedmscjzz.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/grfvvzdcr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gedtuldwr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gyjhifcae.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/goswzrgdj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvyvdsspq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gsyxdcrnv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gawosrgxy.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gezvvdpvj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gipywhfcb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gjhyyppih.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gflwjpsba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gkdjxuweb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gsichesbi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcuvclhwu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gvdaenbrl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gzydlbudm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gouceatyc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwjbwzlpz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gubsgsrpw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpitzxb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gbjjckhnb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gevaqaaav.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gqabccpbp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvalgzvej.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwnvikgmw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/ghfltgrdr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnzqgicgz.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqbnpxzuo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gzuedishz.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gdydbsohf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gisgbygoa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gqlfzmnyn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/guhyewqru.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gkukahleg.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gjptrculg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gnsrgfxgj.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gyytqkrdu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glzzhfvsy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghsktnenq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gdavvmjyy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghnhphwjf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gkmmugavw.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gxvmujjrs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gbiimccnp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gmjgchlyk.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/glbqfzbek.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gzmvqmilq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdsljcchd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxndcwovg.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gmbsvkuxq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/ggtedolvz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gavzqklvy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gazbbzqbf.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gtxtbjspt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gsifqvpqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gmiejulkx.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gvfjyqdvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gzdonskco.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/glecyzdsi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gbbewysnm.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ghamptqfp.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gtjcpjyts.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxrlzqhdu.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gtuxbatnu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gwbwnfezh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gghjvmycc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gezwjwaxs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghmieaosi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gnurysrct.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/grlnurknv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/ghkulyayy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gikqkcusr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/glfreivyu.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gevsinomj.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gerthnmyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/guzaodgms.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/giomriieh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/geifvkbyv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gbpgmvpuc.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gvjnodaat.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwpmgpmkv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gxyplobxp.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gyuzrnvae.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gtxphwsdr.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gfpcmatyw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxqifodzu.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gqplbqwls.sHtML


<!-- 参考信息 -->