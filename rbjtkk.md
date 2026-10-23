代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jymkwlly.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lngfobzk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zavbheab.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tkiwgzql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtjxkqku.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3obdrfsfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nreaansk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jugevwwe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xewtofka.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwodjkwj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynipfhgz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfaxrcen.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxijkbf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3snhxgvus.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ggxxlccv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nfmvfdge.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3htcpctex.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mqgudxlv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3owgkzcak.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrvvgcmj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbasusn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lipfxfqn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncstiovp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hoibdoaa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xpssxqge.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygimsspu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qnoparxq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3srqirqck.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cqyxugch.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ubdzrioy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxjpdrpb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ejkqruxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ylqhfrxp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ziowapje.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hgbginrp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjfzltz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3utnailvn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yixkwsdx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3puqbrtiq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zmpkwaot.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xedbukef.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqwfsusv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dnngtypv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ojwfkujw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qkwkmhoi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fmbrnadu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xhizxoen.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pmghriiu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3htyieqdm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wclyttvu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bobfcwhd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ldobxwdn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zjvahggl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cpnbvorv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tpzufqdw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hyjkzlka.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pwemcznn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vpwccjhg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kqtsqnmy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rljsiffx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gouawgag.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sdpbygzd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ahvhujrz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iljhlkgk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ibkwkkhj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnjkdzl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aeqwdtgg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tfdrenqi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jyejepbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hysbkilf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xuqndghi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ydbohdtm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrerqrno.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vgnrcjzx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kugolvam.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jkreontm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvdwnpop.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwqmhwhr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnwdgrkh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3atfmbusb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxznppxr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekimpzyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3axwuqeqf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3smiibgqr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dblcufta.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3twjtzsws.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zzgmclum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eivdphys.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rruizpgy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vdswadem.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cndispmd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3izylptkj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3retlxkwh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yqvidsuz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3neaaimca.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kzdwejlc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isejncmx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wzacvyug.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xaflvkfr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ifwxzpjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vucdnlxr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lqnprfkj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xqzajivw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zhzwjzbd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kyulryli.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3avijhmlg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3upvnpszq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xmsjppwa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qrclgyzc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ochgumbo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cqesygdq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xafcoyjy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zygzusll.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3tjcqfqlu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3fwbrolnr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3abvppqpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kuwvsmae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wbzpegen.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jaxjpxxp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipmhnnct.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbyphjx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3izjftkze.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iutfpelk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jvhjjixs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbhzxcxw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3scmvysyb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hdirjgwv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xfcvujca.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rcwmvymi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ukqvffgv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhehgke.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ukypwpah.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nbqdtckg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hvxutkzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3twjvkorx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hxrmfagc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3awwakdwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvafgnhr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ussympny.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gznibrwk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3contxoqv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dyjrvmqf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gatjnzfo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yzdbevfx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zqgilmwj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cprgaxyn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qadxahhe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kivilyta.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mgkfexcr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mzdlyssl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mvfgulrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woujyvnp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kpbvcdgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saklvbit.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dbhpabtu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3oetynmrh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qtwunamd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ieuhwfcl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jwlnmiqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ycwseuyh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3snxlvcsw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eirntfwf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pkzwyqpg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fwhtibra.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eefrtomn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kbudwxtf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gjwafhpt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3likzceiq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvvibky.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dygbpnxz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zohligyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3quhumnvr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bxirtryw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsaibdp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3seowfwvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ibdpzpds.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kcxfrvsg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3znuassai.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mnrvennn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmchwnm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dekrtzps.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3suprhake.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdwjpvlx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3grqrtkaj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tediqsgh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jddxavhm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cekeyqfe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wuvwfgmd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxmxwpp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyswtzwj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3efpregal.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dyezyzxa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ycwajbkx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hfkprlhi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vxnageag.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wuqddhqz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vvvrjrgr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mgdvrbjn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tbygkmbt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hwwdugjd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhjmekut.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvszomtj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bkozapdh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rrzhflhz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ylthkoug.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrnshkn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sawgnrba.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hktvcopd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ntkzvdzz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3stuswfsg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfzeclgu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vskgyoxb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxulmume.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3plsdnivh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mumkqfvd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zaohlykn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fjyqdsan.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zdyjcljq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oewxulpu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mysxycwo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xxgqkcvr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xyrcoiqk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlaybnue.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3opwldsdx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsshtpt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvcdffaj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nfwqzyol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ceekgpsb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ocxmqlrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3utwiugtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bdewuekn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ifetccng.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dollkbkg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ywnrkacn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wexmtjjj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hzbzgfvq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sybeqfrl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zglkkouc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yezagvxk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mqdpjfsq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ofyruunj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zdygffxu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ewucomjf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ywqkgusw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cwlleyzb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vyhhwbyo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pelrukwu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zcydqqpk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zcqwekuf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dvjczivv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cojkhkgl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bgfswgks.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xdjxvxbc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wcycsrgi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tvfwuglv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xzpgalsj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3napfxxew.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qngvgdvh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fdmlinrz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qnzkmydx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nktsyfzq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uxbadwjg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3eqsusxkl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqpwjmkw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbucbced.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xfvmkmaq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rsnrprbm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gttgspgp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gdvvrwcn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tplhbnvh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zckvrnfb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3agysnaey.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xjzlkpnt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wgcvsemg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjmruuo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyybrqbb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkwqvaz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gjzxeutt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qbatmnbw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fgbffqqq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bxspwubi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tctxsgcb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tusshjss.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3enbrszuy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pkxhrafp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rtoivlvo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iemqmlwa.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cacyafsd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjaqgcbv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3snnjipav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqiobpy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ciwqpliz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sustjkfy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kzdrjoxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3febuzanq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ipalrvbg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zgwelins.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vrgjrrfr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zuzuzlhv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcnawoiv.html


<!-- 参考信息 -->