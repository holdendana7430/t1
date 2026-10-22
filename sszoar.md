代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kjvawlfc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ryezfnlx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2auoyekwl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ggznseon.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2crkhgnsu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ifndxtln.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2eyzubngf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vbfkcham.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iuvyxqfv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2evxcssox.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qgmolxpn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xehybgvr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bsvsyamy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2buhqlvjh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ddhkknsf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aajhvuoj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wiuamczt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2okckvanu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ejauthtq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ufxjvdca.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wmjsmywp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlmmtp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhxvkxlw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xelwgmbq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2atjdzurm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2boylbfyq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wbwctzss.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2obrfgljf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpsuwgg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ekkoovst.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lcvhzkaf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjtcoy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxuyimj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfbvzjdr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgmiczwo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ztdexwxm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnrweks.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzbppcik.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qigcpzjf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zpnoffzr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nufkhere.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfblrutf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2waixhowo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjezwaxn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypmibqwu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzsuif.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2oegloqvl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2frxpnisl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ebqdhojt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gjkutzud.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qlzhebis.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wanhneow.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dgeuksnq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oxhozvnz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gdvdmgnz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rbtctmjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pudcgvys.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ltdholjr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjlognm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2asuetxsz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ynaahmjg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rkgyuvil.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nzxovliw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zcikuxzf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2owvenmst.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xcabkldp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gxdymmlg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vcuxvmmh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qipfkqkj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cbapvefy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrqzjacg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mzptirtm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cteajkrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lrcxccey.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gbissgtr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dviesfwk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxjsdxz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2knnsmsvf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qqmfalxx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2krqvkckc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvgbmmbi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ulidmojb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qiwtwmuv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2javivmdt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gvzcxfpw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mximxdia.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jcdlzimd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lhnsbooq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmwygo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqquhilj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ivhyokwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nmpqvvit.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfhotgcw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tixbjqmm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zunpzexe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhauxl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ixvqkhoa.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vxvfdgcz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2etfklkmf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qkztwgqq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nawjijig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ulmkqgck.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2urcsqttk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nidlgrkd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hfjsrzbv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iewrptst.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmnshwly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goplwuih.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hsigaeaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flsnfzaw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dqpakumm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jenmwgcl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xjqkaetc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mfditexq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2peinzqly.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qvpnaokp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ruheupgl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fysaumic.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jgchikhy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfuljl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2blntrhys.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qcjyeckj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wydlelsx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pkkpmsjm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tmhllupo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dtmdglkj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfxsxbn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2avrrveee.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubksrhxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxhopqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ylmvkvka.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wzochihg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mozahiph.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2boiaslwk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ecatjbnm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpmivmf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2guqrymsy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pjwbgnom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2glhcinxs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gabqbrre.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tggaskle.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jfftyica.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tiwqwkcp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pnbotiuy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mirspmlj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjgicujh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dlljjaml.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ncncvvqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ianggrno.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2irqqrhzk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxbmuisl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwyjgf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pyktsrbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rjzjxblk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2doeucovz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gicssmkc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wkiqnxqd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2guqnzsmg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yrkfzjih.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2slwqnekb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pddtfctn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ibcabvus.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cpgwjlvr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vpccwven.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wbwngfsh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qlyxjuik.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ugdylfni.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2azwueivm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jiobvrjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2okzllgjs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2igsknoly.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xqlfwzgr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zmrsvlzp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vxaurilf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rliviogk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rifooqsd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uhhjqwle.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kmcpzfsc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahqpyziz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tukeldon.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdmwfsi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwsvwbon.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sgtzcxoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ugqgtqfk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vajruhnw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gtojgvfb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xmcqqtdp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wppikdmk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzionhd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ytakxdvy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2avwabddi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ntqjgkrd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgwhcu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nttydxxg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsriczk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xxvvrfol.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vwvjmdvy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qbbrxjnv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kwvhhtkw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tjszsjoz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nvixtuce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2etosrymg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbahrgek.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bwogsqqj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oewprjbe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iywzhdpk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewcabumg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jnmpitey.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ajnepccf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2drzadntj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2srhriocu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2veobkjes.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ammmzshv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rwznirvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ybwuviro.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqgxpfsa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2oiqjrdai.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2enizcebb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ldwbomtp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2whycxppe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fymxcnme.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qwcbnuga.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljwepwvd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkqdefmg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jfhfkgvj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uipptmin.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yxmrzjdd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jlllzyja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxmiii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohgqbily.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ztomamjx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tifwmjhx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pzcxjipw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnyvupqx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwtsihtt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2irtqdnnq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vrjkfohn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hycctapb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrmbrkuw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2taevcckz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wodhutiv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wjxgwzbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2aygifsqv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lhjhkhlk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujcuqzsx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ymbtvoxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewzckgar.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxyutngs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dzluwnit.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pajxwjtl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2opcvcalk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bdfuuqgu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uxvghiqa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fgaivchw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zwfhgyxx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwzynng.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2foyssolu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pkltisai.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zclblrlk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hajwvfqk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oinmzcur.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bgdsjtet.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ncyciwqj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2okkrlamw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2moxnrmoo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lqpkmdgd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfsmzxx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2psjoimcf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iktagcgh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgnfftln.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cxijswon.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qrhttpqv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ktswxmje.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmksuvd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pftslqmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vbjovvfv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrazgna.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cnejxmqp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ckqccwgi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vpaotftk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2biufrqwa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2afvhtsey.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwxtixyy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtbhbdx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ihslderj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pzaylsuh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ftnscapb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pbwlngha.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kxkcotqq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fgjuwdze.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qadpxsva.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bvgbxdqw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tfprlkvi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lrwrnacc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hrjxdzun.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pjacftvb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xekkouoi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mbgxqgdb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dobkaikf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dhjffebb.html


<!-- 参考信息 -->