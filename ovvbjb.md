代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vgdrfghx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dqpketpp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acpwrlkh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swrtlljc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfhnkla.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rllhxgzh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2otfjaaor.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fpuhzdqf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2snjtugnm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gztjiqwm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2irgdzxrt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohljyrle.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjrrhvt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpvmrujb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ndhdkakf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nidpgwik.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehszbddd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2khwwssqo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mirtkjat.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2flfhyjoj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2agamacln.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awmicaek.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fexruote.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zpamvuqd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfotcjkg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qroxhjrs.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umoxhndh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lzvpzkmm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dfuyjnjw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2izusqypj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lmznwdwl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2blagxngo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2utyyfbxl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dlqwjjal.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pjoilbxz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2thiepedj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xgsluums.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hmbyjdsc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgdefs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aefkutnb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pxspeebs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xavtikyd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jcyzjzwg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pvdnvjky.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pkvqvsvk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2soskmcwu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2auiqyiyn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znorhvlx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2khnccyiu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vyofzsih.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vcptlwuj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qprmrubx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzflpsm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ylcierbj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cjcbzxnb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wvgotvnm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tnokwjss.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vcgasukb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vfqaiifc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fnzcmkrh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2bvisfwgq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2swmkbwia.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gioyacdb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yajnwdpf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ltorkhox.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2unwqywbd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vqvkfjuc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lugcvasx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqzhnckl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2weneadeg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jnfatyah.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ghynluus.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2sihzwary.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2scavnlnq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jjdieytf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vrdwxkmv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2epelupaf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lzkgdhgs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pjtsiuxh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mhgzfqyb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zamospio.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sybszomb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kzhmuwuv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wvgdwihd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ntaiphfg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yfelttqu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mczfwrtm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xdibzwhu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sjslfnni.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ymmmoqys.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2byzqxlsk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sophxzim.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2arammhvu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2auydpfzx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tddhfcno.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jgjvvtmq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zetvkcev.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gndjhdku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcghqtle.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tdshcovq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xuqfnvvw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lekaqqcu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wrmwsgkn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flpoyeal.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iweyvgpg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dglgoqcx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wbltnrrw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hlgeaopj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2opwwvlcd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gjcyfvjq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2luldzwob.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ukmldnab.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiukfrpl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyripdxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2enmhkcdt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bdydpcik.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2aspwmmxd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ryouuagd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ykuhzrfr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2oeefrens.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fdwtvnes.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bssrlwpt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vbveyrsn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vlhtpfda.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2oexjmhct.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hztqawxp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hrqycrxt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qnrbrpvg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2okdxkvrj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rurspvyy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tolvbgsb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tjwwlmmk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ovmclekj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkirufhv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nwkwhejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tasemekp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2geozdimv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daygpbtq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mkprnsej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ljrgewiv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qlkszxlf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ijcsbkzq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tejnqqkp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tfnqjiwo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2utzcnzea.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2onajxvbh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ytadixmy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bzurewwi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jfwnwbyj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bopueyav.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2icfdlpmv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nbtdtxxm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2feokahzy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dywxdmek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vsoukcwm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wcoaknvg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tzhgurbj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ryavmcxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fbfywgfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zqayaajd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vztvixfi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2srrmvxld.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vigyhqkh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wjikyzci.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2soxxsltv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rkcjkbvy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mhfadtsn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cakizkqv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gqaugbve.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ymioeuks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fhxupiep.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pdcurjxv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qndwizzb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jwlvmdqr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcfuvj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qtauuepe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vfouwwzk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vqieuyvd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fsnfqeyf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yyioxtjr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cnmmmgln.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2psxxiqti.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ghvipzxn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nwrvxtjg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynqrqxwc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcnrjtao.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2afgmlold.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vzzcrqbn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ukthvnva.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xddkuclk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fgxegkpf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kdagwbuv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tqbuvkgc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vdmoxxqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bgblajui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzrcvyrj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnrsceq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kuspfuja.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tiizvuke.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dslrqdrg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fnggodvm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ulxaozbf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fyrspael.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpbfygzj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2drarkmpr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ixokxzqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvcltlje.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2aohqdkpt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzfzkjjp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yjmmpmcm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2majpllog.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2djivwhls.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2disripcb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tjpvxexb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2krpxjiwo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ysjewqsm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khujihwq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnzjiggz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ahbilmxn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2aggkesxz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2amolapmi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zarjdtjw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nopbakdi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ufosirsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wfaylnkv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xemsgcul.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dhdmuuui.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2iatzaois.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iqvhovln.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nhtuibgz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rnqajyur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sapgxlym.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fjydcqer.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pisxkodv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktqbmdpi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ozttnowj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zplmcdzc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ledoymwd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ramgzxuh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhouojaj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wunyslfc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugirdbvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gwavqfct.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpgdppq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wcybwcan.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wndghrpr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wdgzouru.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tgeppfkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yijpxaxd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mqkyhyli.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zgwqadkp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqsfcaex.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2aknzkxdj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrafxmkx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xoyubkhi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2javwrogf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wbedvmed.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wiblurtr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jvviefbw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kkdlyqmy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kyzmuqpi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kiurrsoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmpcisup.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsoevagv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yvxxcltl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2boelzhwn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iosxxktp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ptiicpmu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jwouatix.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2aljrvxno.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hrebxvtk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zwzvsznj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwqhpacz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dabaaeuf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iszugaue.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zhtlkreg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xbimqoax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nqjlfkqo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gagbzxrh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qyyjyzyw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2drqrphtx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lfldzhmm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jfndtiyd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2piliwuhw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uptitxpn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owxqusyx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ipqhptrc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qauuoufi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgtpgkb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hqsczshb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qnjmoint.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qxkzmdxk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iumbjsit.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lzepraww.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vwoeujqr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hkrpqttv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zilsweld.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yzbxrwxx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dgxbewqw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ciwwbvph.html


<!-- 参考信息 -->