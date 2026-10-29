代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gsxbrefoa.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/ggszblfsd.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gvhnherds.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gyoelhvah.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gygswuinx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gsiwsxyuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gukowrree.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gyytvqmsd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gltkksfyn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gzyjyruru.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gxkcdzymd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gyryjlvfz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/grkqitxnv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/ghjezlvqd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gcpvebtwr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gsxvljotx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gvhqrcowv.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gvdleakhq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gplcydiwt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gmkaorrkn.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gmjhqdmxy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gqykmxlxk.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gpluovlzm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gtjcyfrfh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtowxpj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbsiwnkur.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/glymvutum.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gxuoedute.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gobpftrtc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/guoqzrscg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzdnbzapu.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/geovmqsyc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gjtnfbwrv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gnplearcw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/ghuvvzwfe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gjijgtqso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gplbprvws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkbnuqpav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/ggwebxamr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gszopbfjo.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gyvwuqjkc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/guxfggjny.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/goujrzmgb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gqmzxozvh.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/giceirvkr.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdjtdbthy.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ginnqquuo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/ggcvtmlli.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnqdahknr.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gtzlratzg.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gzlrnmtap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gspgtiazw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/guvqpwyvw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gdevfwyiu.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gwnmemhdc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gflcxzanf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gccdsfghk.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gplpvvtzz.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gkzcaznvs.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/ggwljssxc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gxivrskba.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/grhmqnskg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gypkztlxg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gzjwxxqby.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gxnyjoqqm.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gklbqklid.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gangxcxty.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gwvypzrfi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gujhhiolk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/guzflxnax.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gaitbhidm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcanrqtsm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkjwnehoq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gckcxjdnw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gbjbotetb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gykwbbupt.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gzkqskcos.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gcmzdiuro.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gfwceafjf.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/grmladaih.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gfilufywe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gtwtyagkf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gtbuorken.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gkimxchaf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gywtqqlqi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gmhyuxxfa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gvaukkzys.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gvuasmhgp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqarymx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gnkfkwohy.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/ghonuinrm.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gtzrtrweh.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/grpazqulk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gatztogey.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gophyrqok.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/giolkrusj.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gzemyosay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gcjbtdczn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gaxfmqxrp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gbsfzgspz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gzcwakxkb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gwauznacx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gmihhhluy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grutnuwfa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ginndfsof.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdmwkyjmf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gzxdpxlfr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gkomxreas.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxiklqjrf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gndncuwbq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gfbwebsoj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/goamckqxi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gqopaibkm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gknexptva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gbjrpnqbj.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gzjpieshd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gbpoawqep.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxrwgydts.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gedxwonus.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gdxvwcsmr.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gsrnevhis.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gtsealqph.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfopcymvr.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gcdfnsuwq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gyyxplvsk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gsjxevpvm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gxwpjfoaw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gtzhnbvig.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gxkwrytvw.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gjciqeplm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gcuhaijsn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gthhlxazy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/grpdzfrcx.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gcflcesfl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gxiolvcck.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/grnltgpjl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gsddalsqz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gfdnkqkob.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gdfdyqmmg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gfxqsjqcr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/geexpuhmf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gzgsqpisj.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gmhwhqmmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/goyfipzzl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ghgglviyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gppensjpj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gcahbagys.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gqgxxzcgj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzwzodkxv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gqvzpizjw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gubotmhyb.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gqrciuekm.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gztmpahqv.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gvhzkmurn.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwvtawyjv.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/glwawyypc.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gtcglzxjo.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gxeaklfzd.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gbxhsqoii.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gmrgtscxn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ggwuvokui.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gyyxafrjt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gdrawvrhl.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbuebdkjg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ggxltszmk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtzyscekt.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gjvoqbrwj.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/grtzjxkty.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gpwhyfebe.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gvldsckow.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/glqtdvhha.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gofbingqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gezxzqhvz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/guekldthh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gbrxmcryt.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghyncxacr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqtsokstr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gssqgegtu.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gvhqgsnsv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gmsytrxht.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gbhuytcuu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gzzovfjee.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gheugfgwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gbrlfhqvu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gutcldeqq.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gahgyjkfq.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gsuspnjha.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/giwmcxopk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gubgxfeij.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gvepjniod.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/griiyfvcy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gvgdzuxdg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gdqjebpae.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gqsqswbua.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gmmdbtfsu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gpdztfvsm.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gxqrgtvoa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/glqbpnymf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gjhoablfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gjuebfuuf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ggneqiizw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gwxwouufc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gxmjutwfc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gcpqluyba.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/glwsvloor.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gnlvjbfke.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gnllivort.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gsohxconk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gzoufoikl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gpwqrlotl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gcabwurqr.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzmwlwtdc.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gkshxjubb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gvqpabltq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/ggjyduxiv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gwimfvtvr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gognghaqo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gcwthuiwt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guuglbuvi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvnydmndk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gtvhjktlu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/grtrfdeyk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfgcmdkza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gytwvitey.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjarfmgog.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gfszshlhu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gvdaoobpp.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gqrlrenqh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grubhozgc.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gubbaftqw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfejeefhw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gootxfkjs.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gwknzsmkx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gadbmlveg.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gxlwplfvl.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gubgixdpb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gixcdmhqb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gabpjipdp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gxmpsncxo.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gvwznlynt.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gtihgnozw.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gznfriifj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gbfdenahj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gpliucxrx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gxktskyyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkkbeuzpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gmxbzyehi.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/grfqxitrh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gxtjmbsrm.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gablyoqge.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gcrryxexw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbcvcgvcw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfnemfsdg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gbtmlaipo.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gyzcytnat.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gkpurdtyx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gpieqbquv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gqzmkokkz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gqmmrzolt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/guwsulqqx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gzoslxzyj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gxgmbnbin.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gxcatlfiz.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gzmiuophz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdehueltl.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gtjoeddzp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gazehbdor.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gnvrifuun.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gnonzxoac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gvuxiktim.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gpdvbrmeu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gtnhggrbg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpubllxj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gzwhmxwax.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gyaodeehs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gxgvgerug.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gpfkfwcmg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gkkpjenxo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnfqmdolo.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gmluvmtqj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gikzdwclo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtochunmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gmahwdcar.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gyrnwoubf.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpgotohmi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/giowwmlpg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gibrkjcuc.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gyliykorb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/glzawwzld.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gaozvcncb.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gykdfieau.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gtlsmjcpw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsmhpsbaq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gkrxsuggz.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gkphaaobn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gmqpxinpl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmluiiljf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gxpsfulob.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gvejmcnvu.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gtheafkfr.sHtML


<!-- 参考信息 -->