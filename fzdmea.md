代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkziaqs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eaprdezg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wjfwektc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mxjbevre.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tbfefqzx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gekrhfpv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wjkiijcb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mslcctdb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmqqebqj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3taqgfsie.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3subpylyo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yhngggtm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cjpfsfvj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gqbyiotx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rpfyempq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tlsrxemp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mzqnzlji.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3krlvmugv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fjzsevhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vbfthaci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejiisovv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hptdjnfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijwmkvwj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdldyqes.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3krvbgegy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3huxcckhy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvnfubc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ctwvekyo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3goshbbfs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jpjlklcw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jihxdvmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xyaofcuh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lpffchgp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vlppdxsc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3etilvxus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcpgjack.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3juloooyi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aonghqlj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sunrxhjv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vrjgjvea.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3stjqplay.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3asrmynsi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jwolblja.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ygecgmxo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhzbofgn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqjkqsrl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yhvjaist.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3njsaaava.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yptofgcd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yavpwkdd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxjqvlyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ztkhazqi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ouwstgqp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnwwgyzg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ghtmgojf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nbgcyqlu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fdgsecic.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtiilqt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqmecde.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vqvvztln.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xhffzojz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qbwarjen.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pmxbysgm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gcwsvmih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nkyvkcrp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uoroslkm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mxstgeoj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ncwvptgu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bfswowxg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rtteksaw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pzuxjaur.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cvmgtkww.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ayiujbwz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3beiwuzcr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxibpxe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uqpujclu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3crftzssq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uruqhihs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rengmyms.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vftezkjt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ynbavjdq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ixsdsisk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yicxuqij.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3idzyhalw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xwqohvos.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qmxlnotw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dxqeumva.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uaibfztr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ngajfcgv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3itlbjggq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uxjfiybj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3etigdjtf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ntrwkhuh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sctvcyeu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsssnuyr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzccabnf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cobimxxt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfdzhcm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eecetewz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ikgweagb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hmdzoukx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjqaqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3prgkkqfj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fameljcx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwgltgmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3sbgogvlq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3talkmlrs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3yofbnpxr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nzohpyiw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3imzkxikr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3onhqqwzx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kwcfkmbs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lqssaeyu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gjqckisv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kkvhhwzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ldlmxzpn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cjocouef.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3masyjsnl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vpedyeom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iloibwee.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mrggdtzc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ehqlxngi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rjxkrotm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mkoqtezr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lstrwtjz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uccxpuxh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ctgcelbu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3byesmyjw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3byupfwce.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3glonybbx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dajrpice.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fazrlkab.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vkxamtlc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dratcucv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pwvdozsi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbclyqp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dbiuihbp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3enlfncfz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uzkuzukn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3klreiwsh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3azipazzb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zyntsalc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3clmpxxdt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vpanscgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3slqhipul.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gnglyjpn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ceorxxnf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pkethpxc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wcavaaal.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xxqlhhvo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tqjhaiwi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jcbrbfdl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vroayugf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhtrnank.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3woopvqab.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3epxemtxd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3adnldqfj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bumfraid.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mrlkahxl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bjocnknj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3frpsvfii.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pqmsscfi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xwcqymeu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gnwiftlk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tqrnlnry.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbzmklju.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ioafirtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiljwvsq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ddzzjffb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntmhyudv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ambqxojh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vidtccja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fgyftyab.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uzcvlmwj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ltbwgpav.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zbtwulgo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fosyzhyv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3leyekucg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yshtbrag.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3erafbofu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aluqywnk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xlwhzdbi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3svacnlhc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hhsaemkg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mdlettlr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hpcelmyd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cxrmimxf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kxhajerp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ldlxzgka.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stoijloq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cshrrjmr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pdsfrxha.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jslcgiyn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tenwucgg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oipzudhl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3sdixzkiy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3txmjaqyg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdtotkxy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbtyrdos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqjygz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nnajpphs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ycegscus.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jnxbrqfh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jewjtdmz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vtkrpuud.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pniwzwzv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rrusgrtn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xaknxmxg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ymefksbu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3apualvmz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ssenftvf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqjoefy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cnlulkra.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cjjfieyl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ganymevs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kxpudccn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwmfugfd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3crbdseap.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rhggthee.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hxaesfpu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3agkbjqsy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zabjoaer.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3flldjvzw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zwbswirx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sqopeqsh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lmhzyfii.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aeewdwzz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qgkywmtc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ueapkuca.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hkdkyygf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hejhztvk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jeaemiua.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vxbkpvrg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nljtrfmo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxabgxet.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ouskyugc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fivchkkp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ypdpomzd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tiykgqzj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jwdtjzsx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oqvhhnzu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wkgndyxd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ovdnbnno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fmmbjtnb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdofff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qbqgusdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtutnqo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3axtmwitg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgdovgf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vwxkwxjm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3valcqmrk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dvbkzppz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nskjwprs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqilmt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tfstxske.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dkzoblos.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rbdrrpav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cdwqglwp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bvxjybga.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tpkgtokm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pxzqjnty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mopwndep.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3meayktxw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iwewblyw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vgnrobfv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wgngijaa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kohcpdnj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fegiqthl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3daknosbq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mjrwesia.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3niibduns.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glnmoeqt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3saktrbfg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kvhfywjk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zhfmcqlg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yfwvgzxd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnqybou.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ntzwxomj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tmqtncwk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eaffzudb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3flsudqxs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfzttiv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrkotnm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3svoyzmaw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jhcjllsk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xsnrdfjr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfntizms.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3buawutvl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tdbvcqmb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oumuldrr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkhieulj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3knndveoo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3goyzdsqk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sfvryooq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qjhipnmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzfqpygu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3reynhtuy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3megfuxvu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3daxcxxvj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zttgfvwm.html


<!-- 参考信息 -->