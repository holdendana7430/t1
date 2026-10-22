代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfmwgpcs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2tcifhxxp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2czdnpjol.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hkztlpsp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmutsnnd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mklwugnp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tdlmbwen.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fcrofnis.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdjxgfzq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2owmoutvq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hqygaxmy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kkdtabjv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zhctmalm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gvihyfsw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oxmgaxip.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ilalxvkg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2axqaezak.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tefhvszf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zsydzrcu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lykifgrz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yiluwxxs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tsizzhfm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lpgkxyco.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iwwkwrtr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rpxxvzcg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yptvfoqs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iabhfquw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bdndgtxp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fkrdkjic.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jsspoyfo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hfhocgsx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbqeqwtq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vfuldanv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2abgldvla.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxtcoitb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cvmotxur.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zttrritn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xzfvddbd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2blikouqf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ldochpaf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jlhzrspu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvivixck.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzlruutd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ecvbpbka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2otidttlq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pseyijjy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xcdwyunn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ogfntyda.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2helarjlc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2amxeddgo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2npynhkkl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uynckpdo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pqblultn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fiekykqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kvdpelrv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wqoawjgd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dqzjrjbk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2repjsjko.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hiefqcst.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ijturtcv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hxktiscx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruhrdgam.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekpwiblh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sdhuhegr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wbknrggr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gbbzsyep.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mhexapgv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bipqagvz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qxrykkyp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xwnjmcbn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vcnuydfl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cajjmgnj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kerwtdus.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2iewmfrho.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sepkwbls.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2idjksjmn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wnjkcadd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vmlocjlt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hmsyrisq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vwwhpbgc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2oxpgtuel.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ndjjcazd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgxwowqg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dslbrsvg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rbldtzfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hbebclzc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2shxnnsia.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtbrjlmk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsoffkfh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2onimytcb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2okqruowe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ithbtqxf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xxxrvctg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2huixqcqg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qzvwzqff.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dsismesk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lzlvtftw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2apxaljkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2istwxwxq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2codimphn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fplhlaus.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2oxxciupi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lkvdwldq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dcwdbuzo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwfljx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fujixblo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rpqcebeq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yncsqnxf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rqtxwfza.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zjnbggbb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xzoivyqh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2baugdwmz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ndfrkkhm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fpluxmtf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2otzrzzor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsnxgbah.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zgnmzujq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2woklizjp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2aojqhgkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awwcnseb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bcnuklji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhhztved.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yffqbjti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ytkrowpx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dzxhuabp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2teawtghr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2koicjlrp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2unizgqju.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2euidgsvn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ikhittiq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yrieqdft.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wvnsswuc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zdlwanax.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lmmgiokj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bnkdfrou.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwxaidzd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jlvhxkba.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzkajbj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uikffitb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vdghlbkr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uiophpxf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xbapnvzp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2iyguembj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2plhvtalg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dkiyympr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2asbbejmz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmbiiiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwjatpp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2izdlnicq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhxksbxb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxzeeoew.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgtapyye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vnncuwmn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2thmtdglf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrrlhas.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yhpazfxb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qaywnmga.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zjrezwgv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2njisczcg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yyzoloxg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vkromibg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2shgndpqw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2quywyvwx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yknhhanw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vmlncoxu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2axakblrp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lacruilc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2udlgmkel.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oulyoqdu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtbnciam.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ggerjuxb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ccbfqkhr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2erebxvdu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtostnz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pktigqtw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ftizdqni.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gjxkrvzo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wsrarttd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwlmkufx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcwgqrcp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ajwqkynd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2agtvziyj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zbummcvb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cqbgxdzg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwjwjpqp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pzeunrav.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yiulxvgx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sddatrjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2uiorpaue.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bdywtidr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ogsijjpm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jxhyssuf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqrenim.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aztjnkxp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ncccswnp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xqaimbll.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etebvolu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2btwazjcv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fzqmtutl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ovhswwgo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ripzcbyc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nftpjqwn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hsgljtwd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xucfdzyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fhjxpnbw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zohohnjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2smkkghve.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfewyod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2njjxyvay.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cumwujyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcpxfcn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qlyhpyip.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2aixexbtp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2spbwqxry.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2symajcqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pkvrbhkb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tycqoxdu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rtijimvp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djoyuteg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ongogulb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jjwcazjd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gwgvbjcq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ygyxximy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mwuhikwo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fwtxldow.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rjgypcfm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sqzaywfc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tobqqyha.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mudynjdx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lcvvsunu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hlbfmoyl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wotsezxx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2azmhebla.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yeosxpmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yzibdlgh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2odowqczt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xnahoxgu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pargjurd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vtcexfuc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2imcdmjvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ieqnxjmd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjgmhjvy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oancokel.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khkvlmtn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ayvvvmfb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykgjifbw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pnuijnni.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nifnijzj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jfzrqyyn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kuekkrpa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2otycvzee.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qansnrpf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2snozxywr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2avfulpdr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vsbidaie.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ihmbfmtv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ueqehtxx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pwkpnhld.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnuevqie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2spbnwtdp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vsfhfnnc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tyuejffv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vvnczsbx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ydafskoa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tdzhwrfm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cezawctf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2eddrigtz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgmkfuun.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mauxsuhx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iwvsovsk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wesrqchn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2biidvavu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syawshpj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sdyplvyt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mfgysikt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wjmshzka.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sezlbcvs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vhcgkevl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2aortppcc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oywnoncd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2agsoirhh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihupqzpo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2urygpaoy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxnphtum.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rjzjdbag.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qykpkolz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nghhkdci.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2afwuzszj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vzrayvtg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2setiagab.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hzccmsrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbrdati.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ywmgvflm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bsljzcuk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fitpzsov.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lawstank.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2quklragk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xbqpzwqr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lctivekg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2obqdkzzt.html


<!-- 参考信息 -->