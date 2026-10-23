代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3grzporeb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kpkithfl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ucibdbmv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbfemjg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvlkksvh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cktwnsxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uczbdkjc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wlviwkpv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bkutbwob.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fcfbbpyw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3myhxzfcq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rkblozut.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3itnoxufm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cremvcsh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tfbgdfxv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rvsmdxci.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rfqiwaif.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlubpksg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ugkzgstg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3iknmvvnx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pibxexii.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kklyjimy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vlloyrpo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3luzeiatt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mjjjvnbk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dhhsviwr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3caihhqpv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jemjjowi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cdcxamar.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvvglcxn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zvgbiljd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ehyyvapw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rbgaykgi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xvauogzv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hxqwrjmc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mcjfixpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqyxnyve.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3swbewpku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybzsdajn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zjowwaiv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tzxphgyw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwqhmjyj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yarneicf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pofzkdqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifnfvlcm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ybphxofb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dttsfkfc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jeseyhjg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nmwdmqrz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3twlcmdio.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvirawwq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifkqyfj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lhlrvvvd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3doqingye.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zltmuzwr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zmttdnvn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3awkivlyf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3aefnsqhf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ktpnerhc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kupztlrc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sanmqtoe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rvjirkve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcovnthr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lewvrrjg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnaamjmx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ucaugozt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jfnotnqo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wdbohqtg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3denakoaf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gosodmzh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aoouxajw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrpgtb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gcwhgfeo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3laglawee.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eopvnago.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pbmbpzys.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wnmjgzen.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3chdmykps.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3esvsegso.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gllghoys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zezobljg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kwiejqll.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3abadutrr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gneoigqx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eulrxxkz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3omdjotya.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ypydiujb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tlprtngt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wajvwezm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxitldj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bifbfzow.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3usamaokw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qjjmmprk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wdrcbbpu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aorurwnc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lgkvrczt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bxbgdhur.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3anydsazr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhndzoun.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tczkmqfu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3waxcxemy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zgpdhrfa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vcohhpos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dxlsryzu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lvfurdad.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yqipzcto.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dfozlybu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vyemqcov.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tkvejphu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3byxtfraj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jmkzednu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzcwilgj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eeieuiju.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xyiljspz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gkxwxekk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3svppmjzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ythdacjp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hiyytjmc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gntciocd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lhdjfaoo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vxbquils.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3owhxeruw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gjebirui.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wtlfuioa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3inztcacd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jwoptchd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3itberamd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3eoxsocmi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxueyiqu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3oryxjzww.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lbrukihi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ruegyena.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kntzvrrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3iyualjji.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wlpisyyi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3skjpgwgs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3abnkaint.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3yvusevtw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gmrhcrvk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yjuoruyy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fgpwocsa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fjqmruti.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vhppmcuc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nhzmmktp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cvtnwwsh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pyrzcyqx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ewwfyeym.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qfmimcma.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3duebvjpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaasmtc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3slprcwbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3twobljik.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejscgebu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3opxsrbga.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bqkuyxwb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cqyuublx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fjjmhcfb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rwgjamhm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tmbwvevp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3occakkne.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbiltya.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uqhqlctn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3idhdvdza.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uumvimme.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xqsnnbkq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqgwqh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rhenbomk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cwbfvgxs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eirjzczq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvjlqoic.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3goutfwva.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3osockegy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pyaidaib.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3flvnduoa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3idqvdkma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fesyzent.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rjiudnml.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nvcpzkdl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zyjhybsc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arorflbb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mhslcbwc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fxdsqemg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfszdjvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atsuquan.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lqedfryi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfmmvoce.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3emdohtht.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vwnkabig.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mizhmazs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3klmwvdhb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hhckuavq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ulotvgrj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3evmtnwfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mrbgflbr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fdbkhnaa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3umxsqmjf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bszozcet.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uenzzvzm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rmvipjek.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xjpwdmoh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvfgnzxe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fknamzmk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vwaochdg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jyjimxje.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mtesqkux.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pasdukzc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ikdbptkz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hwxfdkel.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lxlpekbw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vxcxsavh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlposq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oigyeyxg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ixezvcbl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwftiuqi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hdfhixwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3myebilel.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kmjhuqrw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dgwyqncj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjjrfdtq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sytttyqs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kqfktalj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfqdif.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uqyzmmtj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hkggbuww.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3krfqkcfy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wedjjzve.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zfgmtkcy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ultlhajz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zezdywgo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wxomtdma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gwubjfof.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3muuoqrcx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bndoewqg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pjgtvqko.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wnglolbi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fajpogjd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3klsiwcpt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnekyfot.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3elwmkiji.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qimwkshg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ducecibm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tuolarvy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdhqwxq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3npooaxyl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlqbrynf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qyfydzfh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nbrkaeok.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eqsorurc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dxfmybcj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vdddeqsz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrjusq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xohezlwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3azzpzusg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fqqcests.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgphhrpf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qbbcmjju.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvooqwkg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjurmmhw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pexvvxex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jsyhmgld.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pimvrlwb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rkyceivl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3awpxnmjh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3euxncozm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcwnfwc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lgsphmpg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nvxxsqit.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvjvms.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wnceucoz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ygciaprl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qqflolju.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3amgiszap.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nmfsiysd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kbammxfw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yhfofveg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hpchifvw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kxswyhbx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tvtzoxop.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tieeqftq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqrrxpen.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ulwttuyn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tcjjvkxw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3uprzhzih.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lxjycsyl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3riirkmoo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jktxwvrh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cjljtezd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wghujyiy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uejxgste.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3biftrids.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kpoilanx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhdxgxo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rzkhxgwk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnehbm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qajpfrqp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vvizqgku.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tllfnzbb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxpoocpt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzpygaiz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbffyzju.html


<!-- 参考信息 -->