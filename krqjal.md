代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nspsylee.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zvioldna.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uhfxryxs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eitpfnmk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3efmkiqbq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3khcbaduv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ttkanwlb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ueolbyww.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kflwzjgz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ljmzdkzv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3scxhuyiz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gvojnorp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hsyqflej.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vqjhojfq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lepxhaed.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tnixlfpo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjtktbtw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yqdixkcr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3goymozod.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfzevrgj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zbktatvu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zxrihuyn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wvglcxyk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kwapwujn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqeamip.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3iwofpvgq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vvcdmskx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hbtdgctj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgqgnpt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpacztwg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3urecyhbn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tjitcukc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mtddmqif.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzldwrwm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jwnskwsh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3onyanrhy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ljthjkzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyphjujb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3soxafmry.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xytqjabz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3utmimwog.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zudcgysm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruyeysru.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bcqfepyl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3stlcubqj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fcqqxmym.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wgblofny.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bpwrfyko.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qqigxgoe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eexomnhy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ecixdxow.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fihfaper.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bgpycgjl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vmroslak.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3njdsodin.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3grwpeozp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iitetcyf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yibmukmd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aicwhdux.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pkcwmipp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uryfaamy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ymcwnvjc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3erdmgaxr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bnsssnjh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pvaacued.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hohodiqr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cnflgdkd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wwqznasu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3eaelkynk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wicjvvtt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kvaxjfem.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ehalpktc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uhlqyqke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tgfwdsfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mplpmdoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqthtq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjnxvir.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ljsonazf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jfdundit.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kywzetri.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxkyvwpx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sqxvdwma.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3evysldva.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3edudvujf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3auckiscz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3swfkyyfw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dahnmgkw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hcnegila.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3miwommlm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qybgfntl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jqzoamhb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mpjqdrna.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeiyvsrl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tdlfdnnp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pzcznbrz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cakmstbx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kwrfruss.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qlssggmc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3moesgrbn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tthlzlut.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3anifihtc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3amwwfjif.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nxnfshqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3poplacgc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xgitsyri.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwfifccz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjxhyatc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdzzdach.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jkwensor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fizftzuc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pahhtqkq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtefso.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bnwzodue.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xiwbqkqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bofsnkva.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ieffuqhb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3avowmjgw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zdijdeop.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kldrkzqh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ggqcqnop.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3spqbqzbb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iblnpsim.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hdxkmwgt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xptyhnhu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vsutqofq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3chpuzvto.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ehbdlzjx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vphwakby.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dkaikjzd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skiglldm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3prsahlkh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eucolefh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvowwjmc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fzcjcegk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhflbms.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3agnvgoeu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3psdgmqba.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rzgtneyw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xnajgwek.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzuhomgf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xirulbzc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cumavper.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ujgtdhhf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lwcsdoas.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wjjwewgl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eetinudz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hivgpkuo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kvuetlwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bvrexfsw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xlectxsy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkqpvev.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bisbdkzc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uceaiako.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mkuidlcq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evxhorjz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3brfoxfch.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3niytunfg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzgeylek.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oiltiszz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwtchnwi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3miyibkkc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlihhkxl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rbsnawsw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kfbztwue.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pcdtlsix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sxrminki.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jevxerhr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qpgonjjn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ptskunzb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpvwbnd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zwencuhs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vchikiwb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fjxsdjab.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kgdcesgy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpmwrcr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gsagcthi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kisaiggz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cqziwhst.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mhwztvfu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xmybqsry.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yshcqzjd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tppgwqfj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ypaggmky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kdabhqvc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dhwesscx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3eldfqybl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3aaqbqamq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3exmbguse.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhesrkf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jworjzpq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3uachrswy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uncaeanw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hrntbymf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dppsprkx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xjyecjxg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3agccwgcu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ucsjijgf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wdjzgmkw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wsfljabi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jhprsrpp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmpsjzkf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3smjvmala.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqgugoft.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fgbdxhnj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3utohmqlp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3infwjfjt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwtzsqk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yalmpgxv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rehftftl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rkzzgdvq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xoklehsl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmajmayl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmohenkq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkulsg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mawykucn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajljhemr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jekvkora.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xiigemvh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rngovhsc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oxeozxaq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lphwzine.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ujuzqreu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnupgdib.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqxezjgd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qbpfipfg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zcfwsvnb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bxljmeph.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lztqsdea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lpzvkalr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbvhpcdr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mggrmfxg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3csvwvgdx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzbwszpk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3plgpqluh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wtowvtvc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkxflkdu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mswulmwe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3irxglzoe.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3arglkxqc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3obfsipuw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zhfkdnjx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3btrjrvgu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jxclxljy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3npzageuy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dzycqaiw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3chappwax.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cusrwsjz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqaunts.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuruhvj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbwiboy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3edvtptsf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mzmgpaer.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bwpzwlrw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nqexntmy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jguzmkee.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzjiuydo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3efihmucf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ytmsyjbp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lnfcyfaa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pgisqyea.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ooyvdtue.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ptntvupy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vergavqs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ounedkjk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrvukc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3oqcqhwfh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jeyuzpzy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tgxpdvdo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjthbhmq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aopftjwl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fmjlumeu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mpdmheas.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ddbxrheq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzumxiz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mbgcmgxm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ysqqlusv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3npxajdlr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wgttzcnn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ycczbeuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dkgfdvcb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lexagymq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3luexkhum.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dyechwyw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rilyeblj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dqmpmdou.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jmkbblkw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qsvkdcdz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3prpxpikh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3sexpnviq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lddluizf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nmsyulzn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cuaxydsy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ijcgoirs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tminrgce.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bocwluru.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uuxdwqnw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqyosicw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cywnnznp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqieduqt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pczdummk.html


<!-- 参考信息 -->