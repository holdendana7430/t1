代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3evahnwxr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3oqmnjfjp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3veghcqbj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqogbgcm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fzuczkti.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kbcybmne.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gynylcpi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zjwjvvkv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nfefrlpt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kpgjybag.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnqcjxn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xomswohn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mlqjruvr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3crgdvleo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmsofysv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3plnvlero.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iakqnuri.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3niytlfcp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lniicewb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ezzcqrbc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xmyhusne.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vvtuzeeb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qqixnddy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kcytmpck.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tlnbsdxi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvazmujf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzdnqxo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ugeodrnl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3suwgxfst.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yinfhgmt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cmmxnabb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jwukwjhv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qdsdazek.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qenutxbx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gqkacxhg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3aymlrkhg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jowgwfax.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3advygrlt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dnhilzot.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ziqcujrk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lkbfvnwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3igrquxar.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bmryghlo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dythvnaq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xyksmxkx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qizozzrh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gwmlygry.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3obhptnxo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3agvbhukz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3afmgcdce.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3itsogbld.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zrahaqpx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qkpoepci.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hfnrfexn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wxsglgzv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ealwwvyt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3izyxbumv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oahuttmh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jvbnvcfs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3shhgiqgn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tldnmkdi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mjjccqvw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kecdzojf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zswvijew.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3phobovan.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeyedxsc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vzcjkfkv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qfcgmcrv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aivwkqxz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzmawbi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hfttdtrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qwuqckzi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hqeqgjyw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3krpqabsx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yjyknqvz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vjxjuuum.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ykxmozne.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vtvaifar.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dhctijin.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bvvgqarv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvijbbco.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ggoeadqe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uovzgpxa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xkakboxo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zywwnorv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tgssjvyc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ptimknfm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3miaibdyr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kzleoanq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gbjhwnir.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wlslcnnw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3upuikxlf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3taedczgd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nlkcsrct.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3abumywxh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fingcurl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kfwobjuo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3adiwbjhu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tumroniv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ibgzveil.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gqdpwguc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eihdvszb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3plfchjab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vkbtlwnk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jtggcnis.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gpnaocec.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mkfojajd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oxjvfilm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dptxiueh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ngxafoqp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bkwecdhz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oljkdvbh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvlevmh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nunfdjuv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eglsjgkt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jgaufvdf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bfckabwl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3emprauke.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vexmtyef.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qraijcdm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfsmvz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3comzlios.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3imxygbhu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pjmyzxvp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zdogvxrn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ioispxtj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3weshywlq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3udxiscqa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3klzmfybd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bunfuilu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qkhhsunf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pxwtlupe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bgnbkboo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijqmijof.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3syrcdwgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glryhqaz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3giplswwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgqcyprf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fqhtpdsx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kcfzzthb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uxucbybt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3khpdwhqs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yyehdndb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bgxpwhkm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dotdljpg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nmafwbkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hrunpnsl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wyanvtgn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kkabwluv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qrmcoxfe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3glvnnwkk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zblbdppq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3frjrgyul.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3aymztpcw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3iyxyggbx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xlmahkbi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mjaosfxs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ebtdfulh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wlscsssq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kpkowgdl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opobezuw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkbgafbk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cbudfrwc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3loroudmi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3upcoxlal.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pceciblk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eskvvzkt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysfjhikd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yelevfey.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjdpeikp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3asahexlu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jqmlqeoh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zatmribd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yzilrixf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nfnpmfei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rfrtugfx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jhywtyar.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3htwwgvii.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cpyxffpz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tsufqxqa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pvlzmbdk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tuwwztus.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pwxfahhf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjzttivt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncrhyjbx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3izoyyuwf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mfqikzan.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iiisjehc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qkpfoabu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tljsjwqr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ttfeqdkw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wgizjddn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cjrlmtxf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3gtzcjdnb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sugsemiv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nzcelnjw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xvipwipw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ivagxsmv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3iqnbeerh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3nxhjhnkk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gicvefqx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zwjkpkjy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wekdlwkj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3npllifbi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zctcccwz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nqrstigv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3encjetfd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3thqxsbcu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fytwieoa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3klifvadj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3imrfpkac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ddhiydcy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vezswwwb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ejcvgzum.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tjzydluc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dkbsrsbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pgqhsqli.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ldxfvmnf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xdxcdvqm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qwmhthdy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dccydfji.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ogblnpdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nuytnqjd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbhieuv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fwjpadqw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xqaoabsv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3dnrccqhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3apiviyjl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3iwcsiwvd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iorizxeh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvvjwscd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fvxehtup.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zhujbsvh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tpwryrtu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jqfwzmie.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kbuqiakj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3efmmaaht.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jvijewdk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yjsodvfp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fxazunhi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3iqhooczd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcudmphm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ogkpovkd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fmkbdhdi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fqabdbfw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ljxzonwd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pdrfzrhz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mxdsskwj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mygfuqhn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3deqiddcd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cupxgifh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lqnxqvuo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gnreofsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jyikxcfy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hkglhipe.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rhbejhmy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mblviiki.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gzbrxnna.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfiiuifz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3izbbiljr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ylhmuogq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqzfwihd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3neohrymv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjhjthog.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qyghwffa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qmbnjvoz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgerobdj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vuikcdew.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qwvbgadq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rgeycosm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gwqrwdcw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ojhqqowc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zxxhzcrg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xynrkopw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dattaqhv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wxktpmwf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsqqbmts.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hhrvmxrt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lcjqhkqa.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qwgnnebe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lqjxiauh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3edbteoyl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gwmtkcmv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkcpybbl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbgmskcm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uvnzqpvl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eilxutsa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oqnposrb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbczrrnn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ubcqrxhm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3stekpkst.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3enrixsre.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3trkqvfdh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xuykfdlx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eldgolzb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gsqtlwee.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wxqpwirz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3eisvcqzm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dvwqglhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oyvvckvg.html


<!-- 参考信息 -->