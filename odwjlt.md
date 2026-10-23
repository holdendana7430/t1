代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vbqnirft.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nlfzlooj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3scuqsjjc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tmdtvbmr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bmfdhlzt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ldqzoeou.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lsrvnoak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3clrpyvzp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bglyjmaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gtcxkgfl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rzvcunnq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnbyvjp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zgkwbvlx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfthurjz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lvaoabfj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qvmxvndo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zxdlmrce.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kmlgsvbb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kscuiohy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ctahrhij.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hblhbtjm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yhgujzcz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hljhtnvp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pjjgusju.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ghnrncwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jgdomclg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rwwbgfgq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3szbbotzq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vxzwmvhb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jxatwxvh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdhyktv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3avqfcsrq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3htusklce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wbfjpzgc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tfcpyekk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3myxexerr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wjwjxqjo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dsrgzpms.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jhuesqyh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xnticeov.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nwudahzx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fetumagb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yprhfmvd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pfhpcdwk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbijjpi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zkklzqbt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fgpwibrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3baidxznj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rsjxzenj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnptafkc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gspremzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3iydxhfcb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tvbffgaj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3dddnoywd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyajhwds.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yyyczorc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3klsgbrar.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gttfzedh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ykekaoqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ofjgmfjs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qirjpkxw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nqtacihh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxtmgzlt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rdbkoacv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vtprdvsy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hqlgeyhg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wxkmbmkm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rzkypduc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cdczibva.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypiexzpw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3daxcslib.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ybueqdog.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uccompeo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ahgunipq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3psulejvj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvcubwt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ibhwuryj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gykjnjhf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3sywonzzu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ktcgmizh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ttdlbfbz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hlsssvrh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3opzobgsa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ttpluyaw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lbnipsyx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3znjwslou.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jphivfsd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cstthjsu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3urjlwmob.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wotpyfhj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3flezuxaa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fpylvzxl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jftxqbuz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsglcozq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mexgfzzf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlyqemht.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iqaizgex.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nujlhahf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bmadxvpf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fhqjxnef.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxzuxuut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lgocvsvo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gijdvcmw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sntfnfbc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3odtdfyba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yjzitwvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3axuqorwx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xppypujy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nhdiszur.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3guywqkta.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vukqvrhl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3klildjja.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqhwakks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jfgntjwy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bmykdmic.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uwgrlayy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wewcjqny.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3csasuuwd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3inblkinh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vvebjibc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ykfgtqvv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bdanzkqj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tocecrad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yyfniviy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ygdonpyp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ilvtgshw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwcnojks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvccbafg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fczngjcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjmhgapt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ibedqxki.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mbcfqgns.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hxfjcrnn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pvggfwpo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mfyjmjab.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ywplttwa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jxdyvkpv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ixjshivu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3waqjaqqs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3roljpxlq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lmciyvaj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wneoyroo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqrdhlz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vyovfhaq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3uzcytonm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tajyunzy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jtuefeen.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kzgohioq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vvamecax.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iofsdzdb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3svwdwhps.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zfzhquwx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qwnooatm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3diwkzrsf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3trbnpgiy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3swnubwsy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tqqdvqfo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qhhijhyl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3csiuzuog.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwqjysrr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ffhfwwar.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pofeozzn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vjamanyc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3opzolray.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnkylkn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxtxqxww.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lsybpzal.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qcqfdqve.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xnyejcsv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cfdhobmz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3eszowkdk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3itvcsryg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wrrinvga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jesymrlq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fjtugyxq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tixpvlov.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrihngxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gcspdnme.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zexmzcvz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sdhlearg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hszbyiie.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vggzmnsu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xagtmvpm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kebutbnq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhtvqr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uqdgdlza.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3acvkkvpn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3umvdkehb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dvkebmvd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gfussgtx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lqqnbbux.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3viinepam.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkmwhozp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tcpmvgyr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pzskzcvo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qmohjkgn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ubqltsbg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3efwqrkwa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yybjubiw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iraircdt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfniqim.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3abxiztpj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mkjcveih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xziqdvkt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3opbfmjmf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yobfakow.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lhymmljt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ddlukgje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rwqbkyud.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hknvlvqk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vyxhydrg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zfimyiqp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmdxzcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ppykeinb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jndyyxox.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uujybsnh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dyacjlqz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fdxbpzpd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ifkovjgk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yafktliy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcrdclym.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ixnigxyr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3prwcpljy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hynjsvko.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xhkqakis.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3frkpkkrw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enoxhhji.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3asxfykua.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bayqttge.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xlrjaqjn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ztrzdlxf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gujqygoe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vukfoqng.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swhtnvxe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pdhzwevx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aougdnqb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qgfgcsyz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vqqnjcqd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hcsimpgd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxjsjvqm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjzpksbb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hgfyrove.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dkpbskup.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfpslzrm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3swlloaxp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aysqriiy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gwpjozyu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3urowlclk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ietyvzph.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvjyymbv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uxzkvolx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdrgbxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rnytreib.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lfxfhaij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zukjprse.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zypnuicq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xtzukson.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3khcrtjhk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3funsebbw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gmzsxvdx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iebdzchz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jvpswlfo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mpfmaxkt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lijgebkx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3piszjmdi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bxntvusp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvfqjjwo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htcrlokv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eyaqbgjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3csvwfmrv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tbbipbgt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tlzbrdny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrpxwt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3avyoefyg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tsuejwaj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gacgiyih.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inlkzbqa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeyyrwyv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aevujwah.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mpwvrrhi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqukfatg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ptsmwypj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ybbcrkal.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3afcipllg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ezmzwhub.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3femtlcsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbskxwe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jvljavvs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gadtzqum.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhhuomgz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ndavuhal.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3piypfmzh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vvhtwpek.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lgkzfdkz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3saereviu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3byciuyvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xcidtlyk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kqepqpoi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3usfkevrr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cctasdwb.html


<!-- 参考信息 -->