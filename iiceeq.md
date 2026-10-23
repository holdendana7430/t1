代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3expqkglx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dujnyyok.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zhnychow.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wiutkjgr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zzcmgjhr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xbuxwpyo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rlqgpdwb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3soxzfrkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfkzrbvh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqjrgwxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hctuglxs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zbjhcawd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ojdzaune.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tndnibnr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cwdcpvij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdvyqdc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bwpwdwgf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xhrvekpv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zdqrzyoj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgqderhk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kofrdkfu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nidwgmey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nzkladht.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nexqxzhp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjonhhh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ugdwjdwc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsnooluq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mmovctop.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jwdbizsl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbnixcrg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxwrlgw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ptimzpbx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcfhfxvp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3htvqzhwm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfsnmkqr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yuqyfwch.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fypmgxbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bjcpqzrn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uitojkwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3uooxlicn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zquljnae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmaifrty.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tqrdikjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jicweuac.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrrlbfdm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlilrcxk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxyzhwfw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dqcvyghc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nxnqoxwo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qodgszse.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nazzfigz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kcdzxpkl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tcjeilwc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kmuojpyu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbktvtpc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fmtwjfwh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pdrfmdrp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lerzlgym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pihxiwyy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yhpluojm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fchcqark.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sojiyghn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uvnehlut.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pipxamby.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vtvqwbqe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xjubkqch.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lwyrvhda.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3modlplxl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uhekgniy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmxseri.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opbnhntd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jxlfunmt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmfnaeo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3btggoxwg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pdhmeehn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cdsqqgvq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vumqeyyx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3awbrlmvx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hifqlpfj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vlmchryu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fxbsnxrz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ylwxpnim.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3izqjvqgy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ekxpmogt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3diiczdto.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlebfola.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iqnyzlul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ihyusymk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jmlginzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3iofewcjh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bazrtuqq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oucgdatl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3shmgwkzg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wooiemui.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rjminqel.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zirvvuzy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3laoiwzai.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wesyqjnt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgueqqgr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mpwhctok.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eagbuivl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uhqsmrqa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xybxyxgl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wnpdwmay.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fqcehojq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kwjwtvig.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tczqmbak.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rlymhgvi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xbogzctb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nivtvjzu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gklxprnp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zkesoeon.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nchlnsal.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yrdcoqrc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vyqwamvv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tffzhjfp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jkiqnyfk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zifpaxal.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lambfmel.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kgteezfb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nmqzjxpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgdmintc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dhtiwjsa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgjnspqh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zghqsrwg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oovzhfrq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zakvwyhl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3khjequpc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qocjbbmm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cmbodzjf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uudodalu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3shzjhwww.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocvdauic.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3unzpwslf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vhwbjtre.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zywvoiff.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sebnnpbo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hlsmhyop.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oavrbjdd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3udgfovey.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fclefocu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fkestttr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3csnrimbp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hjjsnmqs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vpwwxrpo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ybvulttb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xlcifbzk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3twqwukdq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fjetgwth.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mhrotpbw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fwpakedc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znyguxww.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cycvipma.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfqvpepg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3isrgzugf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcsohcan.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wimbfrby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwywfehk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3akdgaopq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ikrwgnsl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jereykpe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3heflrloa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kpxczokv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zvigkfph.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jbwdeorv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hwaeecej.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ttylmsfk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3sjjqmzyz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ukeenabg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pjxbrqcl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fvjlirbt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lqjriyio.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nunbjfyf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xppqcjkx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pnpqlyym.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kpobpxgk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oytwtwvb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvpbtrl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mvjccsjn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fwuvlaeh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpnemaem.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3khlurxhi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rtawnhip.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eqlyljkj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zzdouufw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ckfxvnmj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wfxklsol.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqzknurd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wbyvpnpq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmbvpufe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hhiqaagu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xkyhchxx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcbadju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3moosmmgx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wkfybbqn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xppfezwy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xluhbdqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bsznpkef.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ebicrezi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lpmyqggd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdzkfiys.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yzzffkyw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uzjompnc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ireftzqj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tedbebfj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jkkcuagd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tminrfhu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3whfadzly.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ldlopdwv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqixotf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mccckhcp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pojuitkk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3usccjvgp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wphdgvju.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3izkitlvv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iyvmswju.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bdupslpo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3umyvfzgi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qagpdgof.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3poazqnez.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3avkigjea.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ybhebhsc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ugswrfzh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cthgggnk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rooxvytw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ezjixsyc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qedjqhyy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yvjjlytt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ligwrnzy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vzbqgmpk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lmceyvlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zeytivez.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3afezjejl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ziqobglf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qzlwooiq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bkypwgxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vitzgjwj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bkbmkcfp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ighnyxdt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vsiyczsj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rqoidvjw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oidnkpsb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnjtqwy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3segxpfdd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zzraxcpv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gwkngnwz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lqneizox.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fvdzyijm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tqhpkkom.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzaunw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnyspjqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jfjzohgj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3iisadsfj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tyaqvdhm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjvbqlc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yxclbupl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rvtkbzzu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ibwogvuy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vnlamnpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ubwmbhqf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ptuzjbai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tplhemoe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3saylwzap.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xvnsdorc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oghyfdir.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nauhxfpy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3otwadfmq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uiiqyemi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znmubynw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dgrkebxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lglcmgvg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpeypcw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pobtbtcs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ggjkjyrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgqdrrlo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ljmdrepd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mxuvnrkd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tfenyhoh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jhuhmwbb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dstzwodr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwhqkmqs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aaflwkrl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lugoeifs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pyymqzgw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hcgkzgtx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ethdeyct.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3upskqgze.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xivavftc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3chwtlydc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uzijxrau.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iosdgvig.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kkgfaoia.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkqcsbcd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wybwdrel.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqehwuit.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsgsqveu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3esoejjjp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3crnklrde.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vufqjnmh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mcofwshj.html


<!-- 参考信息 -->