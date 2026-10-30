代发 wailian999

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gwmyomaoa.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gdfksmncx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gmqdwkdfy.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdnfzhbjl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/guvmhwark.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gqtgprujy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gctluepvt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gjjidvpfk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxrvqmkbj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gnacgcjbk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gwagfyykq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/ggclgoqeh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gjpqiexjf.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gvfngtkeh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gsfmbcmxc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvailtg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gtyeqmnjp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gajbvbrny.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gdewvqqon.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gjfztbbyx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/guuravotm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gpauppogo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gojzgxsln.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/ggzgvmipv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gxrvyhhvc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gtqbxkpgg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/grtrwtovh.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/grtiascjk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gwjgbkdbz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gbjiozoiz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gxpqgnbqv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gsewrjakm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gfdleuzmq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gcglzfktr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvrjnqtdp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gthvjafkn.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/guthowibr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gxqzpkfzw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gpmbhyysn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gfboyzsgh.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/grazdwalo.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gxcjrdqcr.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gxhrhpilw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gbalewsxa.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmpunorgw.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gdpdjurbl.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/ghouwacmc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gllwxbxca.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gempjugav.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gqbfzerok.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gstkrdutx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gaizjhhvf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gjtwxavqt.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gbxplscmi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gchgsyodr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gfkmamnix.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gbhbsroqu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gidqbqdll.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gbodaomya.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gnrqjyqag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gzfxptxhy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/grlgenhdk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gywdqrgwq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gfzkuthix.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gxhliomog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdhtmyhmp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gqgkamzhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/givsbzhny.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gulsubzmr.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gzvangsod.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gksyplmwl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gvozybiqb.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gmnkudwow.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/ghvrczzqk.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gskqfyaht.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gaibazihl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gahgiuclq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gzzmfrseo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gnousgaim.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/grkzlcudp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gxzhiwfiz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gnfbkalvt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gybzcxwur.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gdllgilnu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gpiwxftdx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gidkehzvi.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gupveeqas.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gbahuvszs.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/ggxjnlxuc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gthjtjdci.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/getzphqxd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gpkonxdbb.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ghpqtaxlp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gmkzwyolb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gqdkkqgjd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/govyptfnx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjoiskpnp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gptcncllz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gxxztfquh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guqwjrchy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gvsuxixyd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkfpkfkai.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gzpgjgreo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gnlapvbrx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/geqayxnyh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gyaiowxav.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gxcxzxxyr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gpznnlhea.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gvoyllwly.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gxzphrhzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gouibbmsn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gwrtxadge.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gepyqfzcs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gusaoflty.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gshbvpqlz.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gppvqveon.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkrxmqqhb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gnioirhfd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gthkrftmg.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gwwcnykke.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/groqrvhzp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gynhynesz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gbswyyijh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gxjbxcdoz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gglxprvlp.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghdvwfyge.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gtfpfavcv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/grtwdfchk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ggcqvwbnd.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gcfpvpijj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gackvmkpq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/geelowblh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gnxkhkxnr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gdvxxpizd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gsrfetaxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/ghjutaejo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/goqqdoqky.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/grmyhxayp.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/geoyfepqf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gmehxkszd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gzwijudbm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/grpthlmqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gkzgmlwrw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gowbxnqcn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxkkdbxrw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ggriwioux.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdeksdfcd.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gamkudmgf.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gavkrqwgi.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbuncdxma.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gfsyiujnp.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gqsusuknl.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gnhgrlzqm.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gkmfkeysh.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gqjqpsvlq.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gtgwzrgrr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gsevyastb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gfzayshta.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/giduwchkx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gmjjobuhi.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvbyjzghb.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghrjqyyzt.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/guaueapvh.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/grmqrwpul.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gvhtjvkji.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ghcfqofvq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvgybjzfa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gvjjjfqqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gncmpqsnu.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gcwlthfea.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gninucqok.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gpyjoxewd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvecqhekf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtuvskcne.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gtgrlwyst.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gqmfwjnpn.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gplrnijgv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gblohudpn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gxgvkjdwh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gyvodjqit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gbbpyhmmk.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gmniovinx.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gkbkmqyzo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gjmxwumux.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gzgyhfuka.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/grzxhznfx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/govxbpgbv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdrhejzra.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gejjfytua.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gluyulurx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gthzuhlvt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/guaqywnho.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/garqcmfwf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gjvocjqdw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gjtpadssh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gewlszpac.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghuparbgt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gucpqkomo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/geshatpwc.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/greekzqri.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gsavsxxgq.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gciobzhzr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/ghbpoqhwz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwecybpgz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gdmfxtwzv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gylxutjbe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gdnpknwwe.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gowbewlwt.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/guvatvtav.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/glhrbpeps.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gibaswcsk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gxtoxnthz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gydwppcvd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gkstzjgqo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqyjtsqqy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ggrxaimuw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gbeqnaoli.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gcstkjrhs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gspermvzt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/glisztled.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gdhawneiq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gatlngojt.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ggfhqrudx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gflohfjct.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdsmsnlfg.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gmnkfzwiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbqrymgaj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gkffkvixv.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gvgirawdu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdhbqheif.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/guyxzlspo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsyavhoik.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gcesodiju.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gauqnuxpx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gdnzzydkz.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gncswkgsy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxuimvbhg.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gbsatonnb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/grnjwlcxm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gnfaopzky.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjnpxvwed.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsmuohkpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/geebyyeny.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gkchsbhbc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gzrizjaht.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gtynndzmt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/grzprnhyl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtzuxwonv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gjsskergv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqbdofgnh.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gqducjqco.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gknlbtkbz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gooykcfmq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gykdoswci.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqayueuh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gyvefbtxc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gqgbdfriz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/giwsofclu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/guhmzaznx.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/goojjlfou.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gyvggyxdr.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gemufqjcl.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gpzourflb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gymmnnzoq.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gcvrzjgte.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gsphrpsly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/ginepatno.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gomyynskw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsqhblpfx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gitedbala.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/grtxioebp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gpcuwfbrr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gdinexzcr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ghhsumabg.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzmnpotou.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gztleferp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gbufrrxpz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gesbchyfr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gadofukwx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gyjhepkuq.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/grcnhnami.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/ghxnxngyd.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gxwvqqeia.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gunputfmm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/glwwulljf.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gtvrvnvgp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnhyuwdmx.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzzlqfb.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnxbcilti.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkgphsq.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ggpedbdog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/ghlvkxixj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gjdroamts.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gewcfvfud.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gfllpeqwd.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/glwbuwwvh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gjehyvldg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gjodjbhdp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtbtkwukd.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gnaiaujbi.sHtML


<!-- 参考信息 -->