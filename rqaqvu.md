代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybiqvymm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dxlzrvqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txnharvw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nzubagbs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2grsmtdvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etvgmcho.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hprosskx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2riovwkii.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehnwaums.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sdekmcgk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ukfbgzmj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzrjzdbx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wbqwvmlz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sfuxkgdu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2luonjlol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvaheca.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ccauxafl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mjvoleor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2aiodfhna.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ympjnxgq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2meetlrts.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iwdpvlls.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2neucsrtj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwhywfyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2psmmhiqf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2doawchme.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2eakcyraw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yehnjfdv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2eesnkila.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2szpnmdqf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ginqwghm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2snujoqob.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkjhzutq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eutbtcgp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hdngufee.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wevwpibm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xdcaowwm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nxagvwgh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htbgspie.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ymzdadaz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qztzeovs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dfedpvdv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2djxqwdcw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2masxqaxn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2etyjgewb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uoodjkka.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tdqzedgw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wtfltmuk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gaahqjzu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rmzkwxxs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vxfelohi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2acoonhzu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kujsfrbf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lhnoyewp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2sczcjaoe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nitflkqp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mrzwqwpn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ygvkhrhj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nkmmqrci.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zbodmvgf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dshzayhp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gksmcfbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnmjmjbq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mrzovirc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pxvwpaje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2snjtmvwz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ozfibwpe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qxrwrotk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yhzwrguv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nsnahbmr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qcykfeqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xtczdgal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vemlrsea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wobeatzt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2swjaysui.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jrsprwmj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gcwqhdzt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrofpfp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ozenuryo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gwjemfmc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kymtvbih.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qdwpgfox.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pygtcdvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vkppmxdy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qfjauxas.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ubdewgya.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hueosoav.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kplhvhkb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ckzpjjxw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hinpiggb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hlzsfgtc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ohtywfrw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oldfiwcs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dvtyftal.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gepsxqzi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2octtxcrw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2edlqarou.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kjipzekf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dygolutg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qhbgtwvv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dhyzdxes.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2buniezmo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fihlbsop.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fznlhzzn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lsnzwhte.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jnxxnnls.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2motcrufd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gdfzcvyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pjaebgih.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2oishlfpc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vspfjpbg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2faabfrpe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2schsunkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rzwcgjvx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ruvuguwe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xptxpwen.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbazqfsw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nyqvzbtr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxgwyy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cwjjsrbc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uuhlabgh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hcehzesb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2avrhqjsq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jaqfntaa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2invrvmal.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dqmciboq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2navqadbp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ntdkagqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vmvqyokq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxnutzuf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lwwxpagp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2frlrubpm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyptndhh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fkgcyijw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xeoikqpz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zjlqyffd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wepfjkcq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ftvosgxb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lzwunshy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2guvlgwpn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wxjglwpi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2flweowmf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zeenvhuf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2evaknuqu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rtmbtfcp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fblgnewl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vxvigwxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evkawobi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ygwrbzld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aizeebcz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wcdkfwpv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jjskkghc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jkdbeanu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sabdvgct.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cfcsdocs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2afjycgnx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uqvwksmo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xmcqtmox.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ptixllwv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2thuufami.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ozgayczt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bzjxaeim.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rzmrrnzq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vgpvivmj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jvvlbkla.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2druqyhtm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rviclkmy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfkcdoka.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hcrfgffn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ezsicrcj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wzplmxtp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2beyszshl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2miinmpiz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2alviptey.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2roilkzuh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgbufdk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2txzxzjjn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lbjllimm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlyldiad.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mcdgnohe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rzkboozn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbrmrlj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jsvfxzuy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvnzxzh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ylcigkta.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2awhuodxn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fzfnmtfe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2meoxtccw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cqpzxzey.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ckumatjx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qljllowh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pfjukasl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ajnklumu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2koxfzrxc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vdcniilb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ypbuafdz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oahmmycv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wbbcdbfq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2owzhtuch.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2deukeqyh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2odrizrrv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgpmnyuq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zpdfgxsl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qumefkac.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bnyvmksp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zzegqtox.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fagcpvtq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iuvryont.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jsgadwnj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fnptygye.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2acnvzmse.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uygjfzze.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fgtxdgtg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxrlfcdx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2opunpsjc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ytkbxeeg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yxaqeeyx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kuwnwoer.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdyzjsne.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vnnfmvhn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdvysht.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljnnjcpk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dpzxjzmq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tshxxame.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hbnyaknw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ymazhuct.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gbsxzlht.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ycozxaxt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jigthsgn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ghgkwyjq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sntfmbzd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2znjxjnvj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ftzhudqj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2msxauplx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2atvozlbc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2opcrhnbn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gkvlpkpo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dzmarjfi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvjnbku.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jjyywyqk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2elwmsmxn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jqsnmgmf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvqcfzlh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pjsmbhth.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mrtvairi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iwcwdvne.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pyswdwdt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fselulhy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zdokdibx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2raueucxz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bnpvhxmh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2axnpftjn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2thuzytoc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbfaowc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nyxkepnf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2arxseglz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbcjcik.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2swzueajx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rjoelckr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wwivihok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcpbavz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lbtmaxhl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jscphlps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yryzjrnj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2twrbropx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tqpqiqvm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tmvivjdh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pehrdgfs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jydqbjru.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrmwmllo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sjgsudvm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihalfdat.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gicuiqgt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ldmhewrf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mqikbrgt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbtucmpy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ptbzftrn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmgtpm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngzpqlgm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2unvjrzda.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wfazzzkq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sqgbjpam.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2dwhmgdrc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lmyushtx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zikmsyiw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gwyxueuw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kifziduj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivgmvbzv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxuotrf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fyvprskl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nzqiplhp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bofawklr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jyunphwb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjtxzu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2seildrrg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sxywayhr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zdbldobt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2czvnpoxr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rghmujra.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2oqekgyzb.html


<!-- 参考信息 -->