代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbvhttff.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3axjmfdod.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3thhwsiil.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbbllai.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aepgueqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yvoxiidl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vaiskvoq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yvrjacrq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3torjseff.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kgvmrocp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ctokxraj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mampqjde.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nbpfnzdw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cbkfvurg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hqujqcge.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3btpdahno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hciguqec.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fetzekpd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ovypxzxy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mnstxrkx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mjlixbqe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3skxwshsm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hqgxhapp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehavquyf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gootlbny.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yulytnau.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dairpstg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcovgaq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gwvmsndf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ibqkxdwo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qvtxldvz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ffjdlrsc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bpkrnbwk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zlcevvhb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3blnaenhq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zjnspwxe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3knqcdzya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jwdfmkjz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tuvlipeg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dhertixl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqphxpdt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3apwisyyw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bazfdpyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uefgoaoi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vxupalmh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjqvsoro.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykyvdwkb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kdhsmwee.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cywkcgjn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zarxoyjk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ttbsqjfu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lglugvmz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3airvmqgl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gqqdengb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bnjkxgrm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eruqcqjp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iubzwmnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dajhohdi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3slytlodc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3krzuxjro.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yvuanhnb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3unqmrdms.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hdrncsbd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dfwtcibm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aowgqukw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3idscagyw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bjjsjhhf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3urvktcbs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qebdywyh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wkxleity.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jfguigyz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bcrpcrpv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3spygcybx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ecmsazfv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jlvlrdcm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rkqwxvkc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nuckngnh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pgbppxqb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ycjjmiug.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nqnbdhpo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3flnruxxh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nvshlesw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3unejejbr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jjsnkgdj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ljeqkasf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tnbvfdkf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ytnkgtxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmqomdx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxfbsekn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vtbymhhf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wugodehb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tmxdawsq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pyowmhkz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ephqeept.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lornedia.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bytwofqa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqmkftan.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hsprricy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ezjsqmxn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yxyhsovz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nkkcgthk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykjyyykz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zdjhzgrb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3moazezpl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suexhnez.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3opjjobdg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3duyzqrgr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qtfeovch.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3udiddbjm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iivyfijr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dwkqcbpo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jqwdiker.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3iidzagop.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dpjzewfa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xolivxbh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojgomcqf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tzlcyziz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sslvfesw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwjqxaku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjljrdlk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3syhrvdfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amftftmy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lkpjnvza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jkfisegk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rovxgiuj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gxhmmnsm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rmdndlzs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3peqadazh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yesqftue.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kcpckpjq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ezlaxyjg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zmtxfcwu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nqohigct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pllypvxr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3toheymrs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3opkapckp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ufqxyztz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vrndivhd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3esuwfmcu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ymrmuvhk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbyjldyy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eytugbun.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrgbiryf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sjbdwufk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njzvejck.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svirfmxk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgbzvil.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3trdgjqpm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kwzifwan.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hknxftdj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rntsutyj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3sxhspvof.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uffntqzc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dygeegee.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdewbvb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3llwqszcs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dxgeacuo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kbzlvfdz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qpthewcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wdwnuhun.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vpwczeua.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pmcmlxav.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dokdwsbo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uxkxtgvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ouaqjmgh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cnezjwfb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cacznznx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3weuulipp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wuojarmw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lzjrlwib.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kivmcpzd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwzawpba.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qvxigoso.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lanlcewp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nhpvaxss.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bukurfza.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hcdloube.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oxjxgusf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ldydvejw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3usomrywb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3haqsgjyy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bvuyqgiy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ouzuxjkr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eqvzfdnt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wljbqoeh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3frnvruxs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vyljystj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3onvyaqpt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dwgbdayv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nzqvumgm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptvjrpml.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3itvdnoeb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jritqalx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgmgcbmm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jxqqnfjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eemtzrkf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xesxbbnp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rtyjjaer.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tjpidyay.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmitona.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yfrdtcsy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3evrvrdvo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wyopjytb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sjoigynr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ajckifhm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odjqpatc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3biowjdep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3peynvpfz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3parwqyrh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fqgtgvgy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cuepqreu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vkzwsord.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tqkmerhz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kkjntklu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psktysae.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sllsqscw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fzfkhvsf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzptdd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsgyyzfj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3juedmsky.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fryxhlqw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nsdlrzej.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kziyoddg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbemjtkf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eoojxupw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3umgvmbox.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kzdagryb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nbgkfsio.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grbtzycx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xawrkpcq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zhjunrom.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wghfnjbi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fixhofil.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qkzaoiop.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qsjlymjs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cnkdajoh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lffgxiht.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3apuuxmls.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3enkegvyt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3khujwhjb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3grvaehcb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glonbxbe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjalihzn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuavdhv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gesfnxwi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lfyctujy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbizepxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zpcdnoew.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3piibepvt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gmvsmafv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3laoftgga.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tompiofl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3szogpsiu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3izgjtfqq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aynywpfe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wqvawxpl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3aimvrztw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qqerpvnh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgmyokv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pifwvtfy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phltfiuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkgvitdx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qtyvkjkv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3olobrzqv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rleinfmo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gfivuwaq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eoskkjfb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdkqrwzf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhypmfed.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xewlzpgb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3alvijtnm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3giwnhtez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eyicratb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hempwzop.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rmiwevbj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yaqvljsv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3sfhovrpu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3nanmbmoe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jhoyxfbs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xycxehca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjdfkj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xilyaese.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3omfwcndd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wutkqyhd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3urjobbpx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lckzpsww.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kjidinwi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3szuppeim.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3thvrwfza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3eigzyaqd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3prxfrxlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tslilhas.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fhpsfius.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sfkfynvt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmaqqrg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccaxtxbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pzzjjlci.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnqupl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bcevzyto.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pvsbdzfw.html


<!-- 参考信息 -->