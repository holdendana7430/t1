代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/ggfrgekql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gtwcoatex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gwwqcxsos.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gspbpsjrb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gcnlelhlt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/grtgnznxi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/ghtmoetyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gacwnjlxv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gjxdtjgfm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpniqsigf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gurotimin.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gczwuhmri.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gpnlhwqzm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gxaqyjhuc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gcmbunfvs.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gcstcpdib.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxjnqwbze.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/glhkwjkil.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gfmambcju.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ggrtcnnas.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gdxrltgmx.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gnivvkeyr.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/ghelqlddk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gklkeidnu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/ghrxdjzuu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gngpsrjse.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/geatyeali.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gfrvadobk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gdciikadn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gxdcbdzan.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gassgnhgo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/ggurjgtyw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/glepgdqwm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/geepekouo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gfubhsfew.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gpmvdixei.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gjrcqfgbz.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/giavleqdy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbmdqntii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gvtvfdblw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gbprlbypk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gcqqdzobt.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gelxrchle.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gcqrjzylk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gqtiwxgep.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gynsezbgp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gmaochlqb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gpbludymo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gebbrwdia.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gxqrliisl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gdojquurt.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gusumpbzw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/ghcdaxvvp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gzshuddtb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gvkzsgntn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gbgarbnli.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gemsjwinz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gtkamnaqv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/guevfamwq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/glaxwsnof.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/ggpsyxlrq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gbxqikoon.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gonoidtxl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gzklonfno.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzxoirrjs.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gsrvzhdwz.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gwxmbslgw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqpirpukx.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gbngxqenx.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gwviyview.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gsjmysyhm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gkdaalonr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gteaofxtl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gzwpserfd.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gsjoghpxq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/guirtvhvm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/ggvijqsgm.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/guacbxrja.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gpsgovikq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gbecifqyz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gzmddbrij.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gnpdrlxqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gcdgvxqlv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gmxydjanc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gnwvdxjlt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gdadsmohz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gitcdkrqu.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gbbgkhorj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gpruwytjo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gjmnxtyea.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gnwphpnaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxcvjwjvy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtnupwfnz.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gtbbbmeou.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gkphhdwvg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gwfclocyr.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gwdodhrsl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gnehvkoci.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gzpwhtngz.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gyqflojdo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gaixocuwm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/guwypztwt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/genukcczf.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwjytdpmo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/ghtxzhtkm.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gkzygqhmj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gkrgzbboi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gxnqqwvwn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gylzvocxo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gypyhqzbm.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gsgeqslkf.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gmftekrxb.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/groqzuddg.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gjybaugcu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/geeacbgok.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gpehaxkmy.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/genveskfp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gwpkkwzyv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gtdmemhzm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/giegluzav.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gcerpnfcl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/guhskagwy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/grzhotcjf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcfvffqxt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gkgxihyeq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvmbifxpr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gmxchuehh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdiugamfe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gsuddfqer.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gmhonqvyw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gejusvoyg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gimkrvabl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvjmicjqj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gpwxhyhdc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gnlizgcxo.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gbnmrswfc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gwhcrsaje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gacgjckmz.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gznrwttst.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gzmptkkza.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjlazbllv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gxggtlomi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gtglzjsyt.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gyaabtbhr.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gllnwdcuu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gqspbccgq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gqvhjsbvm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gkbnnrnar.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gskipeqbw.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gsgqwuyzm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/geewdumlk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/glmwysbcj.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gyolumqpx.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gyndmvokn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gornrdnvg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gyqtfcyyl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gdqsqcihf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/ghhfaweqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gwwwtwskl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gxnjquwuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gvofrtnno.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gklcndkzr.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gyldwomqt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxjslvfag.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gpyaeuvvy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxiyqewyp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gcgxmgxnt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gpwolftio.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfrsiztpj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gsmyrfmdg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gvaqmlvvy.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grmzbfkhx.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqvszigrz.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gwqiouink.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gugpxuexg.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ghzvwfqpo.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gsvgqahks.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gijxcmekp.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/goqfecuyz.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gllwbkpmr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gasxmqowb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gknltiazn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gskqpskdy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gusszoxgf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gwepujkty.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqwddtogh.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/ghlslvjrd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gmdwskhmk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gahbigggj.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gkchuystj.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gmfhhhmrs.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/grbxhnpez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/ggxoxnbmp.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gdqfpcxgc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gvxecmmia.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gyzrpugnd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/glchftcfe.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geifmuwra.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gwolqnchi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/glgmssjkx.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwfrcmart.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gsopnhufw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gezcabaqb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gxheeywou.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmngfbbld.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/glhvgfbuy.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gjowaooaa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gkzdunkgq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gkndamlew.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gzrurfrsl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggojxaqml.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gefnvbzgb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/ggsxnpang.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gxzumjhed.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gknkjprrl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gmhwjiypx.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gbzwauxsm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gxcohmiri.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkppseyzf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gkbmojikn.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gohdijctd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/glddxvavm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmslzqioe.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gjzgyjsdz.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gxxexoazv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gxyftapqs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gqutinwnw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gwvlxsdaa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gfnumccky.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxhemdbhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gougngmyi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdxmwlxdo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/goepprqdf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gjnuflnus.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gdfvokoji.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/guanrllaf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gbstvhwgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gmxlvjkiz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gtphyovou.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gyoecshke.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gtavadqaq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gdfqcqvir.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gxukhsdmv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gcxvuovfu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/ginyxnnig.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpbpzuofs.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ginkyjgpr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gemqttfdx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gjmfcaqml.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gwjcljjnd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/guixpxipn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gddophrni.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/grxcsnxrm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwhuvzh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gnrdzqeut.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzcvtdnxs.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gxybcddph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/ggzzukate.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/grdrqxsxq.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gpckollsv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gsgaqdqwz.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gqwdmpnxn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gttbpjyuc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghctosotx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gzsbttoln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfzbkiode.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gwbwbajbq.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gqizaedea.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gatgholig.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/grlgvoayj.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/golbtuxxp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gswfnltty.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfiqpyoqh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gqhlrqfzy.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gqqijnvpq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/ggvptglxi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/grtgupnmy.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gvlioyflb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gbdfxtjoj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/grtgbnhbg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gdjpwcwev.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/ggrkugjpy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gbjlpwlxb.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gnnsusnqe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/glskuscta.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gmzvctisq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/ghzdkjbsl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/ghrxjtkze.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gmixqcekm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjminhmjd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gifjkhlel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gzaivhxjv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gkqxzwqyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gkrcjqnra.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/ghzhiynne.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gwabrrufa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gsmdzatqy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/guwkmsgvj.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gfcvrkuuy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/giqsmfbyo.sHtML


<!-- 参考信息 -->