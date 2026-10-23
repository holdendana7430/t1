代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ipzfpwzj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bulyprfo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ksxwgetr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nmjepchc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3spcrgsmc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3muzpgyqn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tprijxwq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yuyskbhh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3dobjrcyz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3amguxbwb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fnwcvjbv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azmbayav.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bahnylhf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3akqlxbdj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lawwaoim.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3igtaojae.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3eppotpmq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3igwdnaio.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3auziuybl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yhczqane.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pgsuyggi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eajyzrwp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cvjdedcz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ggiogeye.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pwaorilm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pzvgydzn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kugrdjcl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hrbzigqg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3crmsvgbg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3maoeahmj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzizfvfs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3adfonbek.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ojimhshb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ymfxhxmc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ziqsjfhm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cjvgydvb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qvhskdar.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdylgumh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ppulvojk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qjfzwwbx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cmzakvwu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jadlqotf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vaxrnufr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yszodkmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reonnjpo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rcmzkrgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzqpuutv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtccsdxb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ohjleqdz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uddfbmmq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpkeqof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqruagln.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqttwhwu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3udgmuauy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxemfbuu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3luldykix.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zzmarkzu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ebzpbdxj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hmoebmtq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaxtnfar.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekufpkeu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ffezzxrj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3allvmmnu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vtmbdjgr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqfgkn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3msoxakqy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rphydqtg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yimjfmza.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqimlxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdjfsmyu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bmowxuax.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ycegkhnt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fggbrdjb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bdpsyzwo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3toiyzcwc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dmnzkwbn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3worgbcpq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wntabpat.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iqbuaicr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3diffvtrz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lnhflnws.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wurfwqaj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igbmqtpc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3htylrwzd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pwvixhwj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3auxkvfrm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wlsjdons.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rzahmkxl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tlpzockv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wottulwm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pemuwzmv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sxxqbxcb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lnczufpb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rfzdxvbz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cxdciorx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ntuirlym.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uyxqtqxa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3aydwunpa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3quhsueei.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vaincius.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wprbqogu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3szzsmify.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3elhxmwni.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jduxsinm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsnqejw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqcvate.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3whqivise.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hbiojjwk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tjnyfmng.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3utridngf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jirarhyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pxdwmbek.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkkebkzz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wknbwoln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hewmanit.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dqlvvypo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bqaunndg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3iyxvqsbw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kegguahf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qknqgcye.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hcizugtq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bszcnlhi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gbnxbkav.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iuwjvmpy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uqxubyzm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kwwlzmay.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3biwozuna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kpowcqzb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ymbydgxn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xkbycqei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dmlpctbz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iafoddmz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mtadhkpy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ekpiyvbu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qqpkwlee.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3feemlnqo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3anpngtzd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bjmowpny.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ihhffhna.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3glkdatec.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jfiivjky.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cbhmeeye.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lrcvnygk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tjvomkzk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ccjrchbg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mofwiwme.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fjhfzigp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bqodszqc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cvteqawd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jkmgpodz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3leeyhxhi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pcapjlpo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bkripbup.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qsdgujxt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pvldkgpf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3evpbasmm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gjfflxye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itkozfuh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ewcqgulp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggtmuful.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3matfpgdx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fzxkoyqk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pvdlxlyi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pkztyzdp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgbaxyxa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wmicnvss.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pxfacprr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hrzxhlfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdzesrin.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyudakox.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vcgbxpam.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkmpnqmc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mauyvapq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dokakssc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kstpflpw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lzfzpmzx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dmlmubcs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rujatpri.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jqcorype.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gvkhtqzf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dmkoxzbp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hiinzcge.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3absesdyg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hufdznzr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xewwuubg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3arcvbdwa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qobmfjch.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ttfxmexl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3widwtsqb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3asilfrir.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbipzfvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clwymhql.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qkkoyjqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rufdhhnh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sffymfsv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ftsdkzjt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tgdstptn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zstbjnvl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tnexxzpf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3moojvtdi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yurlzlis.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pnfuzpov.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3byhcdevw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ysltvuzc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dvvylgev.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sdhpmqcs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iozvecdc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uakckrhy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3sytokbls.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtbfuus.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fbnnipka.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iowuokct.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bfsuuonu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnvnlaqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrykyagm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kuudkeno.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xpzartfi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zunivnfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3znygpheo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mfrgpyck.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iagwfegq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qkqsaaou.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3apvauewr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvsjrmdu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cnntvwlu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3glixzzis.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3czryhfdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lpbguvkl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ggtklbom.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfozbcfu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ljaiubfu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sugabcxz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iqhjrydw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cytvljnd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3osydabtd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcpnnne.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dajmwwvn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gxfhwpru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cpmhtdnq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtleoqoh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3deskpquh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sjmihfgt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3avtazcbf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3phpikggg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bogupssl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddhgvlon.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3awuyvcaw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bukhpnlq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hlaieoav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nnvblcdf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rdejtnzu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3itfmusqk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bbkgwkdt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3udnclmvh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3blujkxuv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zrcjzczi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uduaszpd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ldvxexph.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eflvrsiy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cscmxlou.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tzqkgtvd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qoaeuprp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqtiknpr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hacqsmtn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3quzygmsb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxjfslwq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rleshafm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3alroiczb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3avmcgtom.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fusnjngx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3oyanvtkc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3djdwtaxy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oeijxevy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pnvylkku.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3slxmddtv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3swllcurh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wgupejmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ackipbzh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xtplwuxd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3auvhclgu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zynahibt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3noagueol.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpturpv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3krnjgcyb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tgyigpwp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3byrdlaei.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldptutxk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mmsrbqjx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zcutdblf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3awrlpcrh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdxcrbul.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tzlhorgu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qmxrgixd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jrnunets.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lzdzywsj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ipsxbiux.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dgiupwzr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3chgzywbx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3giwflvha.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwlmmot.html


<!-- 参考信息 -->