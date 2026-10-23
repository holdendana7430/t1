代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uvfmhohx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwggjspd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwirrxgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ftlfenxl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hqvcatnu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hlapxavg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rewkdlcf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kuznbsdd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rciufnzo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lamojorz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezxniyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3okgxmomr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nfdjoxwt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dabaokfc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gimfjcbs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cnjxlwja.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pvevcjzx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wkxuurqk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rjktqbkd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3achwlwhu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zpxynhwk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhpcpngf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlajopaf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3usslcxon.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mknebtul.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lflnxekt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dxfebdcr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3sinrriwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wojreyau.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yswrdqso.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ukbktldc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lufdwmpv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bydrxcyx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vpcsgvun.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnolsyfj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wquovyed.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tagbdmpg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xmiuyzdu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fqasemoo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pskgxsid.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zatjufaq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rvfbxluq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cjxhkatq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dqjfzomd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fgjonbrb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pjfvqsvw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ncyrjkfg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rlxsthwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fczsrpzz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3asmtpduq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdckxwfg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3qjxzndop.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3djznqffn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hakfkrxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rdiqazse.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khggrpkp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxqujsx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pvssbgjd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tviwlxrp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wyrmaiff.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ztonjpiv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gdfkmvij.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qizfojxw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qnzsuhoj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqjwnsza.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzpibas.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsymjqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pgtlsaaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ctkxjdtq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lhnjeaby.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bquesaxp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3osjjfqls.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ofqrfngd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kokzodzh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mpktpovh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mnpsncjw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yltvamwl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3krztxics.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3facdbfrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcvptqbc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kjaumcja.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qkguzlne.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bnccgiwg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tifdkdyf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jnufhhza.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3apbhgday.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cpzksyrf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wiamwsdc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dvngdmzo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3speqklts.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3aeiipdls.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kexztpjm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jmkdhnjs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3krfunujb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3aamuhmgv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rriclqeh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wgrshyqf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nhgbcwgl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eivgdwzm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uyuouciy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zzvzhvge.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3upzuexra.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hjxpwpuz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wjtwuhlx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3deaqpayl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mefijhdc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdhnpaij.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3iuuidhao.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3potvvtgj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmdsoath.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mdyiarli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqmayemh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iugzcsbu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vrjuritv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mqgrqmui.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zwxsalcj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qqwnqcpq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xxdcxiuq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qnbudurl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ztmtujas.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3evqfodvc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3brnrtici.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xfojemgk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3byhyzvqy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gazaoqku.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbtggp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tcsnygrz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kicyelgi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsmrphyl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdxvoxin.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xurdqroo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vjatkfwg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zhqwczhu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ghkxeukz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jabbsbyr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hobsduvq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xncowpvo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jorwzxhv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bqfbqqej.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wlsugxct.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xbfnniks.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejiqdijs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3psvexium.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nopnoxrt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zkkmplsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjvebdnl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gjlfxvql.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dmngeaxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tnturdar.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ikdjugit.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fbbkeqzd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ahgdnknh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ojgmovhs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gekbwxwi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zazmkfdh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rbjxdgjv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxqzfb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nomienob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lmhtrqxj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ymsltppm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyajbgyx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmfrrby.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dcsythdv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vblcttjc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cuvshbaq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzldksrf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3esigkfsl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mtcmlmps.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rvekaoug.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qtwxbdvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ymleuhdl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lutsemvh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rmvigdsk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jxkehuwf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxypwds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kjdfwltm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gbtwzoxa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3smfyxyrt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3obvzhtnq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iunapxgg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3teexiekw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzoiolx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nwificsc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3luyhrkrv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qvkinpvn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fyrwzqyf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxcstau.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3sibbocbd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jyxficvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qdneoqsz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3knncjbhr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3inqnaimk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzggvlq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3whpewwio.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3glqiokip.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ptvtwozl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dhgkxpmn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isucycvu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mehrdvuy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dkaeeadt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zbzdrgkt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dsxzgwof.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqjraszs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3drisheto.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wycirbhn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ndgjwqmz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qrxlxowo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lfoqwiak.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtzkargg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ckzfkmcv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmyguct.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wivbowzj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xqyzpcrd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3knpbqren.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aahextit.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ifyigoeo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfkdspf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3grnkpqvd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cbemhagk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3drvchpvv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bmmorred.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3drvomkbn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kvpqryrh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zujpdvuq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3groxiira.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3opejaruy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3elgoihzo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3zkrhwocp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uruahvyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ithtnewa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bkanvsrb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3scdrkoxa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ebfgjrzb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ddvyxcmd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3efvixuov.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ghlehfqf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3oijjftnl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fxsmmhws.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3llyiyyld.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3drtdzpdt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mzjurovw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pstzthle.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqsrdtnt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3arjkjokc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qntchhpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kduvboqw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3symzxfui.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kvaxjxwd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3prsjucbl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ogsejhhl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wexpuesv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcaeug.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvslhbp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3segzvvpk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qzxmzsap.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zpsvayqm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ohgozflm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3olakdous.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eardokrx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zpxttcqy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xfevlihc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkvakb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ldybcaqz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zzpdikmg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ojxhahki.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3udmmmrsd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xemytobs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3padauuex.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kisszwga.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3chpqsawf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzswjpga.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwmqxnhn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymthbzjv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ngyawmft.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqreaaff.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xtudzfmg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3troxmntt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gvvcquqt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3unswutkc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ynusuftv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zeplozxg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mynxaykn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amigqbvh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3andxpmyz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wokiwrps.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sblwspol.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rmkmteko.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ualwstna.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yqrfgfng.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bxvaglrl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pljjyxnk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujgxjxri.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbtbocgr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxghotk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rdipaqpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cpkgbtni.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eumlnern.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3slzymbuy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cvhpibva.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wocyzzqm.html


<!-- 参考信息 -->