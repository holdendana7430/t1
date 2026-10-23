代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3yocusvnl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wjhyxhng.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vzjhyoum.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fainsrat.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kdmacoqn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fljdwftd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jdndflsq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tmxakzzb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mkzbhliv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zcyfmgdj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ukghrfix.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqndorhg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pytqsois.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mpoysumk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxdhzqpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bcutuulq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcsfqlx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hludihtp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fxjwrvfm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dyriewzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3szbpcazo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sbeqjltw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eozvacrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rctwdqnx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lziffdne.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3igwquvgy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zomyhpvv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sgkfxufo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzholrvy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dclxlasz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jlohjuic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ocdnilrc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fgqtkuzx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3krayyxaj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3abofsdqv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bixnoaat.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3skawniim.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fdugmjqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kquehevb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hsqrbfrl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3spdsmmio.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nfdvjwbq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rekxghaq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ewpenxsn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qlsmvbop.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zkippwje.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dxsnqoxd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qwecxrfm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nfbnfocn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3djxdqbiv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vvgjkdxm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lhhxbmhz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3zzhfotcq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zdyznasb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3awykwtdj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zslbihzo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rocftwww.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bfdltlex.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3oukmyygu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dcgrqnlw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3coylmmtq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rzpyohwr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwdryvjr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3edypobbd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vqefqgbd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxqjnaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mqayxdkw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3orvrclsc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wluoiizh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vjsybgov.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kxoahvgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kpvpeltq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3frpzdgni.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zhbbmfhr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3agucoggb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mfofecbl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnuzkdkk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtkwftz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jlahzvvg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sztcfdci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vwrkrfbi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3learaujn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3stpkwhzl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zhohehzx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hnfquafg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juogwipl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lipahpry.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbzfqyhq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3siasvhxr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vozkcjcp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gfmkfsjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wdoaijav.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rbqrnwpf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3npwjtqdx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vgbwirka.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxtjlffb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tbbfjwpb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dqkjusyk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffgolbgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qufpqvxi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hwwcffsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rowsobmq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3choyawsl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gmtaowfm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vnnpwkgs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3oebrmdcl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ycqmdwfl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rwcgrzun.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kixfdply.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gtlfsgfk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3iucgcqen.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nloajsrr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxirpw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwzqnvk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lqzkfbhd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iekjfaod.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocqmurme.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wevfkhxy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmtyske.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eqasxdfp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hmjlrtso.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyswjvi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3slnyvmkp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fxxpghpt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3boihpsxb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rdsdiwil.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sfduafdk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zffeppei.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dafoqdxf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukgodxeh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlabdvgq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrqypllg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ywyskble.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3flydohvn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cjjezqzm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmwkgav.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dljauloy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmawssus.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uupfhykn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fpteqgtn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jvtcirjx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3axhfqsfx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uqlrpsbz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lcmsvcwg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pxofxykl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zsvjyvwj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hjbqwnef.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3luvqctyb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tedhtpkd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tkaxbere.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ltynghyr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dmsoyqow.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tmzwlmdo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqatocuc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cesoxyfr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3huffcrbi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mkknafjr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pwacfvro.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ulvxlqcf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3apcutoag.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gnetqfqx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gscpulrj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gfpudcoe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cqissyzd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mnejkxeh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qwcblegn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3klvhsubl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bcirtllf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lequshha.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdmopnlm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dularrhx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iseldbme.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlrgxoh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpalbquw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kmqefdho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aukajajl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nstlrgmh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3nffgihiw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3oufrnahh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rrlhqsrs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfovegoh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tyjvzyrr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3skqjqfun.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wcuqtnzb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnugdms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xeahbdsf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3axckqgnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jttinnkw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jkbjpyxf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jybvtequ.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rtmiifma.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mrcmahks.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rylqacvl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jyegnehj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uufzxyfx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xwfituwp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ajeaooyb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tiowmsty.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rahusyqz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fpnapqah.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rzmsrykg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uzyocend.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ibfgnnhd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzzbtzzw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xybewkaw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sulvsrfj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pwkrpkpw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwqhexc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hnjgtfkk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gvpqkcpk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3scgmxbzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zhbshbot.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tqjzfcfb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wcicszfd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqkgnxbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lachldlc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zxkqnwca.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gljjsleg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3euwjbgei.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hhpqkayf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zgohcwjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xenjndmh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kylhrdwg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcezbqqf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lzlwhxtj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jyapkmxc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwsiyp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltlkvjiz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kyvxokxo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whfvhrbo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jrxzlbhs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ckeochpz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vjidkuob.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bmxfpytv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tkfbvnpc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lclqbsij.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jminclgr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3frjgagss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brknktgl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3putmcttg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3stcceqqr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kvqbdwud.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rwpaieut.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wwcooibz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nqwezmrz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ajjzzfrf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jtmzazcm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kuobqaxa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bdsedumz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdcjgbi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyhjpyrl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kydyqxum.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpjbvrt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hhpjidep.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cwneceha.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mwsrgjig.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3peizgujp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pxcymqkw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nvaujxef.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qsokxvio.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hjlkeoox.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vxeouaoy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zlkfduze.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3twkyeehy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3otpokpvc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iselznpn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yjfoxkqr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xxcwcpgc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3otzqwset.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wiljfvci.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kpwibtvd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3epztljph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rbdwnasj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jbgwpknx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eguckowp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zqemyvto.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3epqqsngc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eldabllw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zwejzhcf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxhewe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3armjcwld.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kafcpmor.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fclozaoj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kfqipxvx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zvqfhsyh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncbdpqkc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sydgdpyp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jliricba.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3irgafmua.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrjmdadi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjtmajdt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3uuunxrwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkhqxxf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oizhpbug.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3txrmrtnd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3naxdpjxe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vhhuprby.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ofyhmosu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yyiqmrlj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3opvzojzj.html


<!-- 参考信息 -->