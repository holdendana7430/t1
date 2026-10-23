代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pxsbaarc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3diwnprvu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ehggfscc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vtjmdgtx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dfyvcova.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qpznvimp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ypwiefcr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qkbxusht.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ucfsinlo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rjqewsgg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fhoqabin.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dkkgnqrj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjbdjjdr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jyjxwrwg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3etfoxnck.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dopjgsas.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fvzcdxrm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rlraqiwf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ncevrtqp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqquccg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rakrvjcu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfjtoya.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmjhaktz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nrnoiwwl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hyhrkznj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nkubaiia.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rgqyjmgu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oxjkyskd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3sbxodjei.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqunrous.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dzbsnyxd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dpseztjx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hlvpuhrh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwwzxbnd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ddzxmmav.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zgnihxrf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxeigxio.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nmjyyiwa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xeshkrzq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jyzbqspn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3awrndbai.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3syggebkn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ptzsebno.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jubncnqj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qtsvhqxh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gsjknnja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vwomjicz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fljpiipi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3imuzaoof.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tvmkwupz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3slhyccpk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qpoghvbf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zgbhyxau.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nqmygzqk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3halrxswn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vcgutmhf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mgrltobc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3aizmeqof.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vycqcyvd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pvhosqis.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vafuvrjo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zyxyueib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oeopqbkw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hjnysvbx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3srrqoivw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yadkmyyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pnsnorwh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ixuzemfo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vljwolgh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3giijahzb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3edwngthr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fnroinvx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wpkovpjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rfpdvyqv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lbvbushn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdebvdm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkfvgle.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hfbszgry.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dksmqptz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jkusvsxh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hkegnnlj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3emfccgms.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xmlvybra.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ckcjuapj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqwxfqjz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yqvyhmvo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3paudsnxr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3alshzmrw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cqmrnpjn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vlnhctwp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ryfocqtj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rseopzbg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ighxfobr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xkhqzrea.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ttsclfgh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ydfutuep.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fqvxaaou.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ymxknuhm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3opjobcab.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3oodhdqnx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3odefwcpj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jbpvxkol.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kiosiwkx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3flfmfiqw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sifcfrup.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hgfqpdgc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rvukmbox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbtupncf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dnlelueh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpytptgf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zkoylbmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kozylrmg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3udwwlbvb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3afsgclij.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3irrerynj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dzyqoobt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pfdxmgkj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3njdabgzc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jgqwwlwh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gcgzpzth.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qkqyuwbh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3exrlifne.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bajbgwdw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ruuabkxs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amhewzbr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fudcutqo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3stgepgqq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uuefhzji.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3azjhogrx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wejcmidf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jsehxuxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qcelrypg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gidwcecs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fqireyey.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnpdkry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pcvcunwo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tddnjuro.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nqhciydo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djcddhsb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uoidsjoh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ywdcxmxj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vleefuoe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mzboimbc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3udwdmbqf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhiynfir.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3efkxfqvh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kweasxaz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3afnmtwyl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lroceqte.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tmxylber.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpulzqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wvbvekth.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kxaqhiwq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kueupguu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lrmujjvi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mgjccmxp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3znjrsohb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ruwtxmnb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3myytppew.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3riforzkb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3akyiukxt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdrdgyax.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rbbkkuzv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ckjzrsxq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhdvbzzx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dgnvcjzb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3llkbvile.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dlylyoft.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zyrvrscu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bgfupeiu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zyydpzxh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hpxgxyyw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ogtjoecq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sxjrudnj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ikylcikb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ipgtgfxb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ovbvatgu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3obpbtfnt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3udnaafuq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3niabbewq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yiofkccw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3katpzjsj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eihnljit.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3owsamncs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3htcusaeu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vzguigja.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ezytkfla.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rqapqiwr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cafaunzk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bawfoeaj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fdvquusm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nacbjyqh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fzudwfgu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3byjcgten.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3thibwdgy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qvydfjgl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3oiaxrzej.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dhzimpdr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3opnzdnua.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ueebigsw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wdjchypg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uoojtphe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxgknxbq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rripbxtv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lzuobkeb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tkfnqjxv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmkqtzpi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dunpzoyd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gtgtzhix.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tmcigqew.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gymxugpw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnegpbjz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nrazuksp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqfhjvzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rzlluuqh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sizbrtfg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pnramhte.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ahbrhtzn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3asokpjfb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3anyjrldb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3padubjss.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3duivfjgu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvuepbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bchcagtr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wvkpwwpj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvxxkkgf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3thrjbpqw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3njtomgtq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hmalxgft.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vydjwuwu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xdzhpxmj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3spzqkesz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkryljfa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3srbmzgep.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nilxrbiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3swszcyxy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wxzghxst.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mmismqwt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3annvdwxo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3afojkjbf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rmghkuar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3eanpdfch.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wdhkofdz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xoelfiqq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gcivyftr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hhrwgljt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apncwvms.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymbqwdov.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3krcwroeu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jwciesia.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ljymgpvi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cdwmhtxc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3celemors.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sofppntd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mhfvtzmx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lnuuubew.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kchxbguy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsloddh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ijpklmez.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fxtqjkec.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3btzxpbte.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nicvybld.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ewkcwwvv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3njfclxgm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xmhcecyd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rigtrfif.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pkwpvmqf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ltzsjszz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dgpozmwd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fslmliii.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fovfcsir.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wlvvfxaa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wwurjorh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftktqbqp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kkbygjqr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zdhskshi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xucosfif.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aqnognnb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wjukuwmk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hxgckhme.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3krswtrbu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3urkoifgq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3srrrpuew.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ociuwmrm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ravywmmu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zlouzemv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kcvpfmrv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hsgmsutp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3nmoyguvb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vutrbzzc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ssebrtfn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3axmkrddt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ftvblutr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fpfmapne.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vryqabub.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hljwrbpz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vkvtyhde.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ujtlxdji.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dimzcsmr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bgjnrqwi.html


<!-- 参考信息 -->