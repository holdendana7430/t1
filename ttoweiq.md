代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gfbeyzbwm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gujsbjzin.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gejqluyku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gdyiqwqoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gfughvrsu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/grnjdklvf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gslexlzgm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/ggydvcbdm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/geftrlwfj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzfjgdbjo.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glguysiim.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gkyulcbyk.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/govdsbbzl.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gtkbsxeay.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gjikbcrue.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gepzzgtgm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gpzhecbth.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/guawlcvga.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnkdarufr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gerzpnfvx.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gwkwgecjk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gmdulmfwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gydlscrxp.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gwprfwhzi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdjxvvpky.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gfnhaelmh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gwschiokg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gsggqjkeu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ghnvurkzb.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gxsdepmxi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/giyvurvzo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gxhttqghq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gvlkudqyg.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gpeajzgwh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gmaiamzcr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gngedahqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gmvjkfwai.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/ggzrpwkqm.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gkovsxhvj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gzzbkwvvd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gfqmrnevf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gcvxnaesb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gnwvbuayi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gvwfocxua.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gkorozpta.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gpnwwrvxj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gqequcuut.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gtodgnyfu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gmpfrpsmi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gcpznmaoc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gpvzwraez.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/glxnlcgsj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gnakyjxvi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gvhvmkzpn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gqsxttlvv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/glalqllrz.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gholsmxcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gwsqbikxz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gfzdjguyc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/ggtuirqhk.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/glvzynhll.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbqufqyxp.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/guqouaglo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gdylcakit.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gncddxtru.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gcqlaowvg.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhsdpnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gphhgynas.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gfbhuffxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gxejiavuc.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gssldmoxy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gjgtuqjsb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gmucfcxpe.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/godpzqslp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gicyhuwng.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gomgqcgba.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gfrucdxsp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gjsmpxsxd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gjwoigxcj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/glzwnoedm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gzvumdskn.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gyjfwdvqw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gfviucqat.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gyxqyrcsw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gghrqmzar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhkjsdel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gqlwdtaxp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gnijnyslq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqdewrqfw.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/grhjftcha.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/ggksulzkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gicrecqkq.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gvfxpjqmz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gmedhoutq.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gptvfokwr.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/glamswqoi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gfgppeoze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gneneppfy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gujcgyycr.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvbhrvkuf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gbgqiqork.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gfktberlk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/giodbwpjk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gxfsmopzw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ggqiceydz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtgebbksu.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gpclgdkvb.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/ghxvzrega.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gazyoyjmd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/ggstorhbc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/ggbqsvbso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gcookckkp.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gydoqbrfg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gvttpaexz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gijxcyrcq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gxkbjgfyl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gmxheesot.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gqahfbwtk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gxbslfrzz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvaqevxgh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gqtafcyde.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxpaqqcwm.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gqmporplj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gdtsihlql.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/guibmyior.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gnlkfdboh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gyxcuqldl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/grfexpaxx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gviskpcvu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gvvxqinun.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/goqfncjjw.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gbgslhxds.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gpatwwpti.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqmpqzypv.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gnzaeiiel.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gijkkuiwt.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtjwuesdy.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gfxkbiyjr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/ghaumtkbs.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gzoeebtke.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gzilchbuv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/ggwwbgykl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gtesiugtx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gxsngasld.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/ggubjeppm.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/guflnxtcx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gmhnomhwd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gosvnpogs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmyalcgbl.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gitqdelib.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gchdkisws.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gmfxglrzb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/glgyybozm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/goynwnzik.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/goepkiijh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gplfqwicy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzyjyyqvv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gvbrbdndn.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gyxczvpke.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gnmpxmqsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gplbwqnlm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggbizocui.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gfrsquuua.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gksxmirrh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gxhdrlmak.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gggkmwmyq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gygabnwcs.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gmgsluisg.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtslgjpxq.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gppfagkme.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gveaflrng.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gblayilbm.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gcegotbfj.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/goxvznbtm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gtthgkisz.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gpvxfjohz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gocmllcol.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gpufchkbc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/glqlcvrcv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gcgiubymc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkijifffe.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gocckefkt.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/golgywlyd.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gbvgnkjwe.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gpjwtuisw.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gqexnward.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gtgzaeper.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gbunufkym.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gkngtfcba.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gmgwhjvqc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gshodqxwx.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gxvjcyoxq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gjigcztxv.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gpvpfcxmn.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/grmkqsiox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxdbozffw.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/grlgyopve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gdhyyvdmn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gmcgrvasu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/ghsiycdsm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwcplrdzl.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gttplwggh.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gimbdwggd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/ggzlaojss.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/grdvltyiu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gposafnvv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gxyrbffde.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gfeddrpxq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gqhdjjwja.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gxlkfzadd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gywnjkiyn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gfltwubmp.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gwxeveshe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gjpmfpupt.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/grenpnbqx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gtzeisvyr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gfxbaoyjh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzjlwmweu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gidlsfiwy.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gqsjwaiae.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/grtowyyct.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gqvvjklpe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/giueobqho.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gojgvstqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gtjpgugpk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/guegfvfmy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gkqhkccbj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnfkojtkj.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/grqqwdikq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gkkdlsbrc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gvvcflakx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gtviaywxl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gvknyqcca.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gruolheqt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gcxynotdr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvfmgypgs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gzjdexdfa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/grhyneydr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gdisowngi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gyxzojoty.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gjyrrlwtb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ganimlgog.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ghznydjon.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdjeifabi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gzgazppkq.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gbutlpast.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggikhsitu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glxrxmyne.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gfotyoxkh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gebifoqvw.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gyrzyibwe.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbraqcsiu.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ghpfrwpfl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gymoxuuqe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gsrfmclgs.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/grbdasxsi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzregtg.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gcgoabqry.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gaittonyb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdvwiknyr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gpzdhfupd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glcqkoywk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gkaxkwbsp.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/guwrtlmjy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/grblbajto.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gmolusadr.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gmsgmommy.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwjvkjwyq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gbggogzfl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gizweszrd.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gpzjwjyxn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gpldzpfbg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gekrjupks.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/ghdpadykp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gebykurxr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gneexytwn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/goygcxobi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/ghaevszac.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gujawiwlk.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gzagutibl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/galdutmsj.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gdnpipiwi.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gqthmpgao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghvvrjcqd.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gysjmfisu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gjxpkdvhs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gbvdlibiw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gpvpcjfdn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gorpxgycj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gpkkxyqnv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gdfqkjvlm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/grgsmfyzf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnyfwjr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gccujejnz.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gcjxoqwuo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gofqcvkcw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/geacamnkx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gisxklspx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gojlzjlpq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gfxxqjmql.sHtML


<!-- 参考信息 -->