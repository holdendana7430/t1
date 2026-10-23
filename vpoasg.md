代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lkfbuhht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkahsjom.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tzzrmagt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3egrxetzi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3isbtvyud.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3liiiogcs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mogfspss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xihifdwi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vspgqnns.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lzhyrrbm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rorubpqj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vjohczgj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xbixifhx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dpwfvqsu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3feukgfsc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vhohfomw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfppbsyp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vpqgmkkd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuputihz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cneguhrk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lfsvbemt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jqugzyxh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3agcastkg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mcyqirlp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3szgmxxnd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vmcyxffa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wsgvkaqf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3etdqnubc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eqqotvzw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amqlgcmv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vlaapswx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hktpfwgv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ysihowhr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3sdiszwkb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mwdmievz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hwtiphbz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3acfqnqjh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3swztylsh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3djepldtq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cumriuex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsuhnrau.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3chkmjlpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arskufsl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uftehuvk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vygcglpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3waxwbapc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yndhbsuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cuvpptmz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bbtzwhoz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxgsrdvg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ernfohpw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nncwrtsu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xafnorvd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jqgdjalo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgidkge.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wixkhfsx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cffmceel.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dxvruvoy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tvgsydun.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3phdxkmnf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zyougiyg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pyovhfjf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iqqobvfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmuonkq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jauwoyyx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3joepikdt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3arvgkqec.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sakuvlxe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypbojdju.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xpfbwgnh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3unmglfmp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3stuuyqql.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hkkphtdg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzzfqfke.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rhcelzwf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wvfzbbbo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gemuoeou.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3trngqgym.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3syekxkpi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ugdvmcoe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3glryhqsz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qtkmccyz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cnobbnku.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3huasjymu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rzpuoyvf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ftwabuyv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3naxuilaa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3chyvozwv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ycxhienr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ncihhcba.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ajcdoxia.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hccdoxwg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xybszrnf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bekheibc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ncogmssv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kbyenahv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3skmvfigi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ptgxqvxv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3khucybcv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxovmths.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwtcmcw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zoxivtfu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bpxechhg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3cqtlcxji.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vpajlbig.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bewyvstu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3moqxpzzl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yldfzohb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3noapiqsr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvdesszp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kbwumrzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gnqqfvro.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rmssblvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pasfycza.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbovlxo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rsqoimsl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qwzstvsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sfbirqgj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qtljiuuk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qkscnjhg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbsctnos.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fxxddmvq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bzgangdo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vgeeweob.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gaqfopaq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kkptveue.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tqztmwjp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ifvsjfde.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lyxltwst.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3saxicvgv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ksshbolb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xaoooiiy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rcaxdhlj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yloonnpk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zoxbssao.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bcwmzpqi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xtkrhprp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3glgsnmjb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xkeayqso.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dayccvij.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cnvibwnh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xcvbnrwe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ecltlwic.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3grfisvgg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jdilgbxj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zrlzrqzx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xzcumgcc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iyjaflhh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hrcgzoiv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ptmrwhto.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dfnyjykh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ndixjshq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3apttahru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ugpanykh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lzjgmgbg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ouuzjdsg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciojvwrc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sombetoc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wopcujns.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3daewtmqz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3viwuiwki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oibnzrxg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xxteebnu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bcwvuwzu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvjyesus.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtjyoxwd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3upgicdfn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jmxbllis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uprahzir.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bsramxhv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xyknaltl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fcshmpkg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsofmywd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cxvmkzau.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hkhbqcay.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jkusuxnq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3udjzteln.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hnpuvulq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3baqksomd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mrubfxcy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mniaaulz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qgevossw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qyvustut.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oakhxjpo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vffwqiwj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3myxidwsb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxubpdjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjakerus.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kpcructg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgaewsec.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yhqouzwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jdubaret.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pwfdtyji.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nclpwrax.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uhrpouet.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3aklxyrbp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pbcioedx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zaltapkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uaouzmay.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nylvuziy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ppqjgbku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mvdytloa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jeblqpgm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3plrdwfsn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nrfnsoir.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gjytqbgu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ftxbzlxs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukyzjjuj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3osdlhwnl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3viljjuuj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cjbyuqan.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lxovfwtq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3odyveotb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cmviyehb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ytngkybq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3elydlffy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bogdmyxc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3oyuekozt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rzfiszoh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ofkcbzxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3umtxiqwu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3edtgyate.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lrpbjgii.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmmnehm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjxekjtd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ubyzgvvr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjmbilyh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bcrhyfof.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wzsczglz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qnbsakem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3judynyhr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qsmujmbb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cabpfvwz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qpifszjq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ktllcbfh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zvuwihss.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hiwtaxop.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jhokawwd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jllmottb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmnvtfco.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vlewfqhq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sfxzjqyi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sqqxhlwz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vkvygyyy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wzojqoze.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3eyalfsib.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyyqrbgc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qicelcze.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jornpqlv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yzctegfe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tswsmaft.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oqpdgtff.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3whewacwe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ghjqqdsq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rcxlruza.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ihvsykbe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3swughvfi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iwofzrhu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzxzvptp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vlxoxqut.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bzefuoum.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kholyhmo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3igbishis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cbofgaxv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jojgmdic.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ixxqmhkc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3afboezsv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pvwqiahd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qodmvgaq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxoyuurj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3idaneqvl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3acoqxhkb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yxbumame.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3deupzugv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rlbxbiih.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uwwpqxpq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uvbvffuq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vijyevbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3slxptpbj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3svqlqetf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qsmanfrx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xtaatrhi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdegknan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bgvwqogq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ykksolhh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ffwbexrf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3syzporpf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3glcomjqp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kkvpuxvq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nqosnlpe.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dygkvtuz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hydtmpkk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vcvpcpww.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3emsfjseo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yqemnzqs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bgrtfhzn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3idlufivb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iyaeyfcg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aeqgfgvd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wzojbswm.html


<!-- 参考信息 -->