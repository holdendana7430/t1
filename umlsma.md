代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kjvyzyml.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pfaonboq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhlfkvn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hrpzrwio.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vuopxlue.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qqezudrs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ckuokbtl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sgffejym.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2nvzzbheb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zcgsdvbr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wdziekwi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2skvyquqv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pwyulxzq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rbeeltba.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hwwfabiq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ujppgbfm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2turrxonu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mouingzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jquprymc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2uotaozwi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qykifuqi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wbxgvdvx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvpmpsw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raysdjiu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwkwluw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wszxutmr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dafchqgt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dpupfspi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nwptsvkr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2paaasanq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dmfnksav.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2byxprsot.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzamusoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fopwbfff.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ixpsnnuq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2tmgzbepn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2myzdqfko.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlmybxwp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdsdjhvl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ilsjckwh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oknzoaes.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2olnejdyv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2encfxvrs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2slqqhoqf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2indagyox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xaoijpio.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tokvxerk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iihqgexl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cfaepkhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fevekgvg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jxfanmlh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kdrygdol.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kfwglcfh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qepmpywm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qblpvcsd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2badwquar.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dgdspney.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jzuliemg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qcsbtkpn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2afaoumxa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2njhniqvj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mavliebm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gsfmhxls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jyywxaek.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zjzmfoew.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cedogqgh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rzjxhiiz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tccuzykj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wyqkrkdy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wnzhfkvy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uzvjmznf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mmfjmoeh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zfclwbhw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2uipymwsl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysjnrlts.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wdyevoso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rrnypwgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hjenbcbj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dmawehcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owomxshj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqkceadt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ahekfvlv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hxmrlucl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2aropympa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmkpxcpr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ghemzjyd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ihrhyinb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kgndisyv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rezzqthj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wnlnypzy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdchngi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2smxsripy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ljbrxmlc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zuaqbbnc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tavyqjhr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zytxplnu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ynpzhiwh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ckzorimo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2algkrngk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2voknfkce.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hmpjjeet.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2chvlqyzo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vrlxlkwm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yxgzzdin.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mrzxbbuq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dydwpubu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kmtonlpf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqlqgkrr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ibvgomgk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ggloujsp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ovmvotln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xttrypit.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fuzzfkkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdblbupe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2apnmugyi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xscmfxkz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ijggsxmr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kfuquafo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wsoocjpp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bnccnjpu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gytwjinq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2iqmbttar.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fxfqxllc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2aagogngz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rkecvwtk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qpyhrdta.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hjmcqibx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpmsaagm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ybaaisxi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2miesnpkl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fraqlnev.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vibkvynv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dylaoefh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2azoxgqqg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ykovypxt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vilgrauc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ziamdzdt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsicwmpu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2etqahdud.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2opfxiziz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mrtgmfsu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xhdxhiaa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqmgxax.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfnlfuz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cmqzuirn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ajtwiloe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2saxzawep.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jdgdlkij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ivpxkjgj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ndwhcwvk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eduikvsr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ttutfnmi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qudfdijl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tkgmzvld.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rdsadfyv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2aroklvmh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pwmnqpzd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qbfuhkah.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bvahzzcj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tsaotovc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjfnfvqg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xcynifkw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmuqyfzo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vqtpwgmj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bbhnpkza.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrrgjbfk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rjorwjmt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gjqjbclu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2njjnmcgd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cnltourj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ppsmlnvk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ydysrpil.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nhcwaicd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xezenhpl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pottjwrx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gkzvttzb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sfleecnd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kirtcbom.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhznhtoz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xwebkssi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ynosckvs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zbqmwrxw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yefnjexk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmttipsb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjiipgq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kdpzhayd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lnnaqafx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2axboxaas.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sirwgxzk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sxonnmes.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rgdqtcfr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vfrdzxwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2exmeqbhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xkvmfeni.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2brkxtoma.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2plkcpxwf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gcstdzym.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zrukiyeb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyauapo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2voevcauj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2holbyulc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2chtfchww.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2froncruu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bbbljquy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qjdcmnro.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lbkuryle.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bkootidn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uxybptxe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wwfilnvl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kbmthnmg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntkuaxqz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pakgitce.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2msuolopl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2okwyneta.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cnztazso.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcfeygzq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yjineiwv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dqxoxsjl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jmjknqvf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxnomnh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzmrucmx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fivpuynk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2teirpfpg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cyvynsla.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2thbopvhk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sykboblf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dcplxbxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kmjgtgdb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hgxsabqm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgropbfj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zevgopus.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2slecfvtl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fsyyaqio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qxkigxhv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gqackebf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmkdobr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xfbtepjd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxqmrlao.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2djnyooai.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2llecdezw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xupumrys.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2psslgmir.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2psdceyrn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ndzvbjru.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qbmcvzfn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2chtuezkf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ddeyplvo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zvnvqwpb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2koujohnh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oshncbsh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nowjyqxc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aujlzayr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hiciyayd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfniulte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jbozxtfn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kuibgwej.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mbnjqzjc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rmghuhtd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iejanjmr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyscwun.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrfexvtm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ertilvui.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqxnadgl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mvwivrmm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yeyhenhd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dplltrse.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ooqyzngz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujrkkffp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pguhqdqp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zhnxdkxe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tkmzuito.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ufvwezwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rylgwvvd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixeiktli.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tfnbzwdg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbgzjmti.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sbysjprt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohetbwln.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nnxkjbud.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2centimiv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2paahkhpa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2yajjytjc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2umelcxai.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hromgwjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gfngyxkc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rnlybzui.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2szkdtoqx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iveqyxcl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iqanbtrd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2inbezioe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ehhkrxnu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lazljadu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rfygcipn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gwlwdwvc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oysrwify.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pffqnsah.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wqisezdi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2molvdaii.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vzdpfjtj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmwjfwhv.html


<!-- 参考信息 -->