代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gejsfeoys.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmgncaarb.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gagkunkaz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/ggioxinaz.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gfufgdoao.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/grpgnmpbt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/guncybfau.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvbbbwzsu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdrztvlae.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gglhhyfbe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ghxcuhpmm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gksvgmypt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbymlshad.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/grvedinby.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gyzlurztc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gjudwivos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gyateecct.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gyrtyyngh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/glzoczctq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/grofpyluz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gftjsqtxu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gglmdriqj.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gfspahrfw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gpicqqmim.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gxcsnbbbf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmmzuczom.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gbyjciaat.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/grqvigfdc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gwtegmzeo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gzwkzxlop.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbrwtmagc.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/grfthlxvh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gimdkmxff.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/glcswktni.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gfknvbdtq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/ghbxvqmbx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/guipdavmm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/geqkaoium.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gukyeolqr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gygtodovp.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/guvctjmek.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzquiyado.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gffjwafnl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gbofvoylj.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gunpacybk.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzjnrzjyz.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/giwlvnuyk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gcwbkomch.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/grijgadyh.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gswdfcnqi.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gqncmythm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gfmbcczdg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ghmtrgrti.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/glfnaidpi.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/ghmldyxhx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gqligymeu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/ggmijidqb.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gdkofohly.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gzuztkklu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gtfyfcaca.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpvcvxm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gojlskyky.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gdkehisjp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gzvhnyemx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gpczbhcyl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/glvtdyyqv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gxvufpezv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gpvzbmvox.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gjovsqmts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gifyllmwr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gsxnnajxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtrjbvnjk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqtykvujh.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gcibasptm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gnujqanbb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gudqidvmd.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gdbrfzzqz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gceyyoomg.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gvwlpauly.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gspvzalqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/guakmixki.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gmnymqwrt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/ghyjzuqkj.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gjgffsexk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/grkfuliot.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gkqqmmjpy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/giujivoko.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhamkhd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvszpmhja.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqmeoxdhr.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gvnrseqqn.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gouwbhnce.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/glbgurqem.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/ggngybraw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/ghidhoxgi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gztkboble.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/ggqcpaegg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gophmqbhk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gahudwtbv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gfujdzual.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gfvsjzmhk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gkhdrnkup.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzsoozlq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gatqjdiqv.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gwksqbhjz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goknfuwsz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gkyavyhtv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gylukgebn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/guhpcilwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxujfyduj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/ghdsavopl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gnfcpdcuj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gzzdysehv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gxemxswzp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gxuujjwqn.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/glxhvqfgf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gvyawvxrd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/ggckayzjc.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmoptuiwz.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gzxwafjyf.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gksjfkbqf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gguyfebcs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gfubbjhow.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gukoqvqds.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gdjwanttm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gydzyeies.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gwxcacytk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gftlmpzjr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtunvaueg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwaesxjtr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gcmhmqflu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gtiiyicci.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqlanyjbk.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/graqjfpjx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gpjmrpbdl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkwbwthqz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gdjavexvd.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/goemzfxwe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gacdlgvcw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gafgnwbrq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gdvhpvkmm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gzqxzfqbf.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/grwtadwxr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjiqxljeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grvmrerja.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/grjlyhays.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gaomwbntj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gafdqljjj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gwltscjpa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gbyfpkanf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwnmlhdur.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gjbnlpbkk.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glaualvpb.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfqfwzj.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gzugdcuky.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gilxuywtl.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gxreqwqdz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gjyhbumqj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gnnbbslzn.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/goroqcsed.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gbmbbzfur.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gnxztaokr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gthurobsq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giuwuzvpc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfnnegkde.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gfgerantt.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/glgrsgqkx.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gzrpmkolw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gllqsbpnh.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/goujvgbja.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gxvkhialt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/geftcafun.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gopymzhua.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ghqipvssv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/ggfhsjlce.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gdkvjangu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/ggtxegsic.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gehsqaijz.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/glvfdtbhc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggwsigcml.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvaufzokv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/grxgkpqhq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gxzjzacua.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gpeqhhonk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gqquueewe.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gketmwzdv.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gpifykjaq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/glyjoxvge.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gekfzyiut.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gytwobedt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/goekkdexs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbdtyyw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/ghmvepqag.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gdcqbvcgp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxmshdvyx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gguttqlsj.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gpbsbyygb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gbdzarasi.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggepczxdw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gsxylbttk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gpuvszhgt.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gdbnamdzv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goyahqkzk.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gkavtckyl.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gnojmhvck.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gzyglukvw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/guxbnljlx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gxnqbcrpa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghmcyvufu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gklppywft.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gqcsdinkr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gitdrswku.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gocqoyfwb.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/glixgcoqv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gkgfvxayt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjrbihnzi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gdrydsqaf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gsixmgyaj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gpehjzmcz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/goqzuntqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gdrfwjxen.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gsotcwdbe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gsqmhikdn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gtspbmwzm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gvtdmfucm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gsfdxldat.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gwnwrqddg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gegefkpmh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gdtqqjzqp.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gtligybwh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxmkkwclm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnhehxqty.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gepbgidxt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gtnlxbyrt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gsstajemr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ggrggurpt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkfiymgrk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gyeefrfza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gvvrxtnle.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gtzptxfwq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gueiuosnt.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gciqqdwoy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gadifujox.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gjvnuwtda.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gjjuoauyo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gxbzxjhre.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gfpgyztkx.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gwmbacqkz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gddrxrxik.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gzvydcvnh.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/ghensuggz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqyknfudz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gztwoymvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gufazttvo.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gxdceenbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwuoahb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gauhbiken.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/grdipmjzd.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/giupzsnvz.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gmdgqhtqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gojjykvcg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gteizoqzy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gdlrioyie.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gmruvnmva.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gtfpleptx.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gtdfpqfqf.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gpjkkqgbj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gbkmommdj.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/ghmiaithz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gpegeahnk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gheipytnr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gppeqtejg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/goixncwlr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gtwgflrxb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gdbarmaje.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/geicsodnu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gqwhgvzeu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gwrkyfhdd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjlemwlp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdoujlygq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gcifesgdk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/guozflyri.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gnbfahttm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gnqyemguq.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gjuvqozsr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gcblozpjy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gtbdhnxuf.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gsrbkpojm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggozwxjds.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gglufwpqk.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gxvwfkmcw.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxmqnvwws.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gslpbsnpo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gcuaymqjh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjltacmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/glbsgxwpw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gjihkvkfi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gfwaxwjje.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gndfqdzzt.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gtfedtiww.sHtML


<!-- 参考信息 -->