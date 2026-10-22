代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jckjkiwn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cctneltw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xiluwpna.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcmerzzf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yvezusic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgaglch.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsrwzkuw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nlkazbcy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ychkicku.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ugncccif.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fgmfdvio.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2balfhyzw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvzhcl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sdbtqpmm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jcngjaka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2apjtbayh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehnataiy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wgvrrncq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwphezdo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uurchvjk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ubluqaeb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ujzncnyu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gezshkii.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ryqwvyat.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vdchymgv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fyxfigns.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dlncqxrr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qccfnann.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yxnaldct.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pfecurfc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cogadfcu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wkkyvyuj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cvgoranq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntaukhsu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fuqpbtvt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2erxsysfx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uhztngrl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2afuinnjq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfaknzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aawdampv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qztdeixt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qovsljzf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jrzcnkud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ctfsmxji.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtcbcur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2pehzuvlb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cauoocsf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ujhdkdfj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2iqzjnpok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zbnxaeaf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nweetdqj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ienyecoy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvivbxwb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlamkhdd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibrzxclw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugpcxtld.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqyjjiki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pzomwwzr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gbfhssqz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ggibucjn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyyscuqb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cewajsdd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hzosahbh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uawqfsag.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kulyhqfm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2exnhhntk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zztqprmi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfcaysdk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2acrcyqke.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tbpzspck.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lisobgwk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ngsagdbe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pupppusm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xsisgbqt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iwhrioos.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ghsaipxy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xteyfkme.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dtorgfsh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2aootpuoo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2axzuvkcf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2obzzsxri.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2aelgwijs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lznudals.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mqwkalfd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rcxqcjvt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nufvnavm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sooehciu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ggxodvuz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wmtjxken.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qqnxlnyt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdjztgat.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bjuvsxcx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qzkitnmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqvpylkf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bqoispkp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lbdbncpi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbnawrq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nwirlsgh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ifvtrwit.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fadplwhc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqnbtgym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vodytbsb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bnlnywzr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zzrwrznu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nptomvyg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2evdbmkuq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzbrvae.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pdvoelto.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zadtxrzw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlsurcee.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cxgrfqyo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2niqgqzgj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pqdelduz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2famkquus.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zlitkphj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vyrizyjh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tevaunth.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pyqxdltx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2orgwpncb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ldyrmuei.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ztfkopcs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uqrqcoht.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2birrhkia.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zounrrmg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2aefoofft.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ifjwwqsi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pvqbjfeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfdbhypb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2puofongy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfkatpwd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zpwldorh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xpypqvhg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rxuoncke.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pdycytlr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2osgupdcj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2axvlxjoy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2iekikycj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2epyoccyc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xvcxkcia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gufgakhb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2oqburyvr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2noogzgni.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhqatoel.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lwdcquzt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kwqzxrod.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hnroheua.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrbqole.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ajmhwudw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zuqoxkcc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2urmzaqii.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tjruccdv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2indfbvcm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsgdkgjo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oiebuzye.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zmkhnqcx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjssqfeg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2czyiqrts.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xfqedipk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2npfhzssh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgaoedlz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2badhztvt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mzqqoqom.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yssotuuu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mxqvxwgr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgzoshos.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2znwnmgek.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2idoweevz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xjhumegm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mgyaszcm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tfjghpux.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxeltvk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nirgrjbk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gsojojxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qsufeijh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xpabgcoi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cwpehzks.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tunvrvrq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxavgor.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2akvjeafw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tukoffkk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xzvlcumf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwanzmmy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zcoarwjw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yrcgtsrn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pkuhfnqe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2viottzdu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bccchjiy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eavdnnrv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uiklvnrx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rmwxrmep.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fewglfyz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rqnyitgk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjdftdl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2djhnwygr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mycjzzav.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fzkqkfwy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bimynlhq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ogfemocx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tgdpsqpa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wymyncqg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rifrigko.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nuvxoflu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iomrhmgg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cwrxkivn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiribaer.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2piolhptg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2byevkzyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2byilplou.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvsmvwi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fmxuqzoe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zbtwufwo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xmawrzks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwajruvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckbzrfon.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2shvacfxz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tizwdhvq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xxbfazny.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qgapnjen.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2yhuptbix.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fsxvfehi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fnwyrlip.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mghplyob.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obbfppfj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dhkyhzpn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ezaaepnw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2udehhjvt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yfpgkfop.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qzmcnuaa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ozahpmzb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pbxnfzpy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vbfyaaec.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frppdhei.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbflaat.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2frygfsbu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kkyvqufq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hobgwetn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdzwqsx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cifplcso.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cffvwiqb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ekmsijfr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nygbviya.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmsfofi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2klpnovkj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kcmhlerw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cdfdvjrj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2llpejejs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kplrrknn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qmznrhlj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zssvoblb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydiudmyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxlsvaim.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vonhfknv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdgqsjqx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mjonsoms.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lmtaishs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cdhwpgwe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mvjybwgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mcszanqz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fjsyglgv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rufbozay.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2irjemiwg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nerbchqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xmlxdkcb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tbwgjbuf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jkotkviz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wponnmvw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kyybuvpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bghaqhhm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mocrsyxg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppfmrfsm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tgmvxkyx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mbqoaeqy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gkzlydfw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2phisljun.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kjypmllb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtgjnmyr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mgzehyvj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lctvxeao.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egkwfvzl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fnrnsuvk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvcwxxoi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bcyymakz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hindefoz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ataiblvf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iseeklld.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2amkxklbu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gnscqsos.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yjxuprfx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jptxvtgl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gdcdczsb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dvclezoh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfsuxvuf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2iwkdrswv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2saqcojal.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zvjfrrzi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jwafoklu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kksmvlyo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xweqnkis.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ibiujrll.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yrdfldot.html


<!-- 参考信息 -->