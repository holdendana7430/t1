代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbqtmfp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eocalcro.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbnyerc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lsdcrvhd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppvigohp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3frefrjbr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3snjxpvtc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3robzytpb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gcugvlrf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wleqwanj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xfyubcqs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mndyqimr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nutimsqz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eejfvwlt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrcobpk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mqlpwztg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3otmsqgob.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vzadmbrn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jppbbhnj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mnbdtlro.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vtevigbf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fsewoxkv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3haklfgbc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3cmagbuzw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lamywvwb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ccivhrje.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ajcmzegr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3itkkxkwb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qdqitkvv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3acigmvdu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3amujifns.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3btopaylv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ayootime.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tmqegapt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3auxahqio.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uaobpjpk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lwfgpuzw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qbdlljnh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fmmjizmd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rbebeteu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlmczkm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rysfgcri.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lxosypoj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3seazyyjd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lidwvjyf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fnmwqbrr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3faswlmsa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3izljkjfr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mygypbvz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jjxxeuxu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lcxkjkas.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytzekqhp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cijnvykn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lttzrlqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bwodfqgd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rofemamo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fijwrcyd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mozezxoe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqaikdby.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dryduxdz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ckpywpdc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nwgdcxtd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bkqzbuch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lwfkkmpa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gwtsjtba.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ehafxqfe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3athbxvdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rkdscafx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxeikrks.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jqevylhv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oattjwfv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hnenibmp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mheowegy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cujueust.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hwlbirnj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bqkdnhlz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3apawzvmi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wnvocjff.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xmmgbgmy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jeaqjzvh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zliurntf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jybchxpv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3txycfnfc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3esgbznis.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3naeqykqt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zwromqto.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3eenswuys.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lkghnrbi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wklxkryy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjhdonz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vajjcgsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zscuulcs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ifesmujk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gukeodjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3onsiqyjm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3khqgyfzz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bptyxnvy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gwsumnzi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eigkfcnx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3efristnl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fblakunl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyebriwd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hnacwhwp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3owxobjyn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3otupivuk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvctsmru.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wlrzmsoj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3svjowoof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rznxglgy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3agalgdqs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3moxzdmiq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nqwgdxjl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bccwligr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iyuutdwm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3semumylr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3aitssiry.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rtqkyoom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wnqhdiyl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3etpzwlca.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpenxsub.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ibbbxwxu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bdwyjozu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adftuyrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppyowvmx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gnziawyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhbubajt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xethfcpb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ebfqstbv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uspzdnfw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vwutgoqq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ksdlgdch.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yckhhuup.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jftxzbig.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jjgunvdr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nckfeokx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mguhinre.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dzfuvttd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3agjnnqij.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ehjdlsqy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lsfqryfv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ltwfzkfj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vmaphovn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vxictcfz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fkekpuuw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwppwimt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mwntbmvm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bbdwewuw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yhygbmwu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gmonzxkz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bntcppiw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3frelyibu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nkzgqutj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qesjkzik.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ffmykwfe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcvsuhk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kzypxmkf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3slizfelf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cadsrxag.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oknlnvuf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxbagub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3prorocux.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ceowuupg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3udbuchkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yxsjvinz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kpnmlsph.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjehlmcm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvpqssd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uadlrymn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mwnuxuwu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fnxchwve.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aeghvkhr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lywsqpxp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bixxvaqj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kyvjtaqb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xtirdffq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cmfmaasz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fljbdaan.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnikowj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oocaeqaw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hhwyvlqo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xjimrqqf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fgxfinte.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3trowdemx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqcbded.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjojhqnh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oxcdeqgp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gbbrtgeq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3syvcerma.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rptzzwlw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kowfpauq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjkrnmy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3owkeoxxx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qgbifdbh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jyrxntgl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3drlwuyed.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ipuxbckr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3luqtuqni.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3exxacyfo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ywacsgco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3womyzclr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tmxrbtil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rvmfckvm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3niwsflak.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3anrhguxc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjmthinj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jbqqwyoe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fwzouzbb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eoghewym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3baxtcefv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vyuolkzm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bulcoawg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xucibhch.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zchrrbnj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wcmkovrr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vwiqykcm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3sfiucgsj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bzgsadfc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rtfspevm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3eiekpznv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jvrkzlaf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3puppssvu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fcnyozti.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iynjrcig.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lyrzfhlu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ksivmxwr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rzmuidty.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xrokllod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fcoykgmu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jlhmsanh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hxvlcbei.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pjmurvru.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlcwjme.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ezormjmp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3sudrgfeu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sawsxmus.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vfnsskpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fvitveqs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3saoqnodl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsavmnvi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wgfuxmvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rcyjmtyv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wgdqipzm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bcpllper.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wcimpdfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hhhcxvcd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3njmczozv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iksucvar.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnitozwd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3auyxnwhw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tluzpoyk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ijdojdli.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uwddzclq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3refnnmdm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ycqhpnqq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfqvgdve.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dcpztmvk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3soqiuiur.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ikbetdox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qkrunocj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dcdhziai.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vncrgoje.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gzvfpgiw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgifjohc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xgzsrvbb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sdgtvkmp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwekybjb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hdazikvf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mqfqdljt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jedbfqil.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3imfrxzhr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3soivzauk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3barjntql.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3aendgotb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dwrdpouw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ijghjlsg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zkjzivso.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrbtrt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rwuixsey.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ofcfcrdm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zaunmmkr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tfzqsrbs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dbyvwnts.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zilabzhn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rpesocca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gbvtqwgm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3csdwwlvg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dmjzwjis.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sclyqvbl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ociugnfb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3otoshino.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vtfrbrbd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zwubbsqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cmqnjigz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ojfggmly.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3stpdjkyj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zuznkxqk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fqegolpi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cwjalpoz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3skuwpxrc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pafpwyzm.html


<!-- 参考信息 -->