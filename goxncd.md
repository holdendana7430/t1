代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dexcvhqp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3axefwqox.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qfsnpxwi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dlatfacr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbkzywdo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3njtxgksy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anzmfjws.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nguvykyv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sjvqqyev.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlaqtccr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ineaqibv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tozlrsfe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3atmxzuby.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhwdxmu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3onvhawyn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ordniytw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3oswldsbf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cqkteqbw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3adtolver.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmshhgdt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvxbyzfw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bvocpdmr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3izgqhoxi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wgnjckrh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mzgcsiff.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mlcbxfha.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bhyrbwbm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxqclo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aehgvsnc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gzgfqslr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvofoppi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3azmkgdel.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ccwyymet.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yxtkkhdc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rsjmchro.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jmpawonr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3awjondbp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3einovrds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mwbbuyeo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kjsyrqny.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fzpskkjw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnehddqd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hafwkykn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nxlatecd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eegfglqv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qchkcepg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iysnszgq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dnwdszvk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fvjmbpsi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3msqwicou.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qcytdqtq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sdwxpees.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kddcvzwm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3henvqykq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kcmuomev.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bonughmr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3erjxdnle.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3unewrxzh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ygzphkqr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nyzvdihu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lxehjbnr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3efndntzk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3oidhstqh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dgnssrzw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcldzxk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uujlqsro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qrlxowrg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3beihznfu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rbxvswsw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rkqmytkp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xufnpjcn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dlrcvekh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hjopmlwb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3heudoehg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lohmhtcc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kdpbvltq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fhnsifwh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3svibjjyk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zofeahvg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3frnhjtob.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iuqyyqtc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkdjvmpj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vxiokrdm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kxjjxzhx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tkqyxhjk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ukgtwxrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmbmxcs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kqkwwfov.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ncedmnbn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ifrwxxlz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hjstsrwm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3obnumzod.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cusrietg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qpbwaekm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtahqnek.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gdtekirk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aiwbbfei.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uiwmktkc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gxddmthi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bayhfufp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jooldway.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ncxtwwcl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ebuomgdr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3apujgyrb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3thslegcl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sufxxnef.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nqeynnem.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dacqnpwm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xhuyjayx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ihwdtwug.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jdaktibf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3blipdpea.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qjfwhdca.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3yckokmkb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwzkzrsd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fxpbargq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3humfcoks.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtlodhd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zznwffou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3itkhaapc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eavnvqvu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3apxkteju.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3alibqnja.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pqskuxee.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vdzgbtgf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hfhqebis.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dcbuzncu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eudgdcwa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bdejwfik.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bxnmuina.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zcuwxjsi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mxpwtkmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3watahmbe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jsztspbg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xddozggv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rucmxfum.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzuzuyys.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjcymqhi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oqwdpykv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vmklfepx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ibnppsum.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zaqizorb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mvdjncls.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3imvrraxj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktrqdqvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rwtkxqra.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tpqslamy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyceajzo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tocwlgjz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bgqamuqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okbcmien.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfhzwmna.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kwtemegh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avqyjaya.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3swecwcjt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zvfggmgi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fldoobwo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jlquclrx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3youwwnkq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sxxqsrvn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ctjbmvot.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3eecgywpq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vwjesttd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fymlvxgs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xjjddltn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tsnvjdwm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufhskvvj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3grbxzuez.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpvqnmdd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3izehirxi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vrmeyefl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3syflsyju.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3krjeywec.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rquqvedz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3phnsbxbr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jokbfzmr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cavohljc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gcofulsl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvipsiz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mujaqyri.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3exnwgjlj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fibeohem.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lwofurom.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avhfsozc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rkfonfns.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rwalqjzu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ewhhfoqq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hbgsljdx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkgagdy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjcmhgr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3eutvdcsv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ylbkuaty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fmfptmis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ooejlujj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3haseviks.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkkvpfd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3naqszotb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pmikqoxd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nzwprrgm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iychygis.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzagtoc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nngifsod.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pevlguuv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dqhsobrf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hexewxsj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juhjgjmg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wcervnnw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3itblhrom.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zlgjzgrn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mlwabgue.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tycxhbys.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yewkarjc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aahhxbev.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wrksnxpe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pbomwewn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ttcxmvdp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bbtcmajy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vyupejvw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgyelqf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkvfxgy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3urwjniqc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zfxsolpv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lylsnbxk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xslhkcfr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xcrkvrpk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3npdvnlqh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3livbhoka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eoqecocw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zafkflgy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dggqytkk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xmdcumno.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mnkwamcl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfurjlvn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ufpsgqgm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ilteupdy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3axivkssw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxoggmm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yutxrrji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zufisutz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vxspztbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rttqjwen.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nyiksqsu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3idctggme.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tsbwgadt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3exjjvpgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pidpjajy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpzfsvhi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pmknguty.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3btqhfsim.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3unttytpf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwxiwnr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fnzokscf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3oinuztvl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kcmguppq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3riwcopjq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slykgxjv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cvaygplx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwoqsesj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lkanemiy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3logocixv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ysewqoob.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3klaxuszd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mkatgoik.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwyrwmfc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jiabdtgc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ttsveisb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cauxcxbx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpqajav.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3svpgiuvs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nifbebiq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pbnwkyoa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zpyqdguz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bahlwyie.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3huluiuwz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfkadmk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kwzkspqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mtacxbyz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbnecxsq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oqdzwzyl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlmfybdi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kpwubnhr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hoqksfui.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgfqpet.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ytzxcglj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jrughhxk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sdqvuljb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qhimzxpf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3odqamdkr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3donrznpz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dndgpssg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwprsozj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkiohev.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mstavcsq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qyagqkhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wsxqvdcl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hjhtudft.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wrhfditr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zjotwxdm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sinwriys.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlehbexv.html


<!-- 参考信息 -->