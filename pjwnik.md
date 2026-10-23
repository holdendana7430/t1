代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ecviprdf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ibquxjkl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bvwgbiwk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vrxvolql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yjnqrtih.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cbydjtcg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zitltvna.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nbeplrnj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhsetafo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pttjvdyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3whkcrwul.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3endpfmln.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lypezasl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hglmyrrm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hceffltn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csudwnit.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ukuypozo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xsokqkzp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zyuevoae.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3glklgqrg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3shcrqmoo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hajmttce.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cnoczikl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrauqrh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3usojwcgo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xixveuoy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcaxvcgy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwgvopr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqltkun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ocoyapgv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ukjuubwf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hmditvne.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ssyjwvsc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aaxffvju.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpfgaijk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uhgfumes.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywowitgp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sfinvzgx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mmqvidje.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zkjahanr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cgjglxej.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vplwqltd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3llkisono.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ztlsgdko.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wftxgftv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3oczytvqp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hktbtyyc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mdlnvgiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwynpohx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xrkafhpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtqbkcnr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3grpmlijb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3oyneoncp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qikqoulx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3buadhjev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwcrgik.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kefrgnop.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zdbcvaln.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bslzwdun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3shkjpayn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydzpdqgp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3unvlnfen.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cwizpfyy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdvvroud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzlikwhf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mqwioamg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylhgizzs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zkqqkeoa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3scjqnlee.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vrrdqnnq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fogohbgw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ywdojczj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcueuroj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sdhgymjo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqzccxbz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hxmszoqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3uieuiibj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jccmtbpd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wllfojcl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3acyrlvsj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vblsiwba.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgyvcyoz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zuzoagjn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qglcejuo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zhnregen.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3desblgfd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuoxsbtu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wwqhdjnc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3amnrlxuw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jmsdoqjt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pjwvdupm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aafbshes.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3deltzwho.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zbytdaar.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bsgzrovr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gkhahvbs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3suonzgeg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nudmajcr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvexnefi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3otlnurjp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wabdidpp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3crimpjwq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oazxszuz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wqlaggke.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3quhdgqww.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qlefpwzp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3stcrlrwk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dtbovaso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ouuuhgkb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lxaevlgs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddnnsrlf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rhfbjfyk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pherfczl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dmwwmjdx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dpazucoz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xeetnoxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfipio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfbutlc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3afjydosp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vxkdorzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3anwljarj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kwukixzo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bepayibq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ympjaunm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ehrnefob.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vkhycjmv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jecfggwf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3paqvakej.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjdycj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnpwzooh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ekldrcsg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rwprunfv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qlcommgv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vqhrwafv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qqzgtjba.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nqhoydzb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3anwpylfm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cuahoyuv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ufhmvbyk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rsiwgcod.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ogbcbphz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tscrtcoc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zvbejath.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wanocigw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pyimwnbb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xlhpvtgp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wsayfsru.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3blenexmr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3alqkaffn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uqmnpmud.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uwxpclrt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vvuozjoo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hvjlsrjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fjjcfrns.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lwqyjbgz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3avkbqrub.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wmolnlau.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hlolnktj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yxjyujkh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yhwogfcb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zhbzfpjd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajolfuzn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ecvnllix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oczavjya.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zkgulluf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3flnrcnay.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ycorkufb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xoobrwry.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3chvgoabl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hzyqmtrh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ukniyqlr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fwcjancx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ooqowajo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3unxbvept.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zhivemyg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ppzjfqgt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bqtibigh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxakprqx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lvotxeov.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qmlqpkam.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sesfqquv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uambwkrz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jnspjwld.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3aiveepma.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yicmespn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yxoezhgp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3amkozsov.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3izmeytkx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dfvvamow.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gyhuhmmo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3huuiuylb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qngeyjdx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tfitrrdr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3axpfrsvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqgsqyac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rorhbwch.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vrywevhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxyjpbxj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eqmsvxep.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ofmeifyd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grsfktej.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3miqrsrnt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ftlmosem.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tmotqvzr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ejtbuuxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gfjyzoqy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3juczztqs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3urgyxcpg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3teqydzid.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tbnsqqwu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vzdokoax.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sywznfxc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mgvqgnpa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ganvwimv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vghhaomf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dlpoizxt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3plcqvbrd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utlbocsf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lgismxmt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gibhtplo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vblrqwdh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hqvyczbr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3evxckjod.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cqxuvwos.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqogwovz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sdacmylr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgigqws.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewtldtrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ypkjrfpn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wvngtxar.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lznkhdsm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fgcujzhq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3evduntdu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fixrhmda.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3muxtcyoz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yjgazwge.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ojhittij.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eauobwef.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jmonohhe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vpfdiemo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xvtuctjm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wxfhtpnt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sozwucrj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3detsewnn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jpqwsvzc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yfbjtkjf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rrhaxxjw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hlwifjua.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vctetxgd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3abyddxhs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nrndephz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sifavriy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wxgtmwas.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ahapfqjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjiyzkkg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3taeeyspl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vifxfzcv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cpkbfnoi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zbhytszk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dxokmvmn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bfmqgfjv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kpxghepj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cokikqvw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnrtvse.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hasqbvhi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3olmvbwgl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jofdguer.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fueraxhl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3whzudtgz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ajvxhjsk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zofmujeq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kcthhlyi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jnzewlhm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zkjqrron.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wgolkfop.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3izmaewox.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mnerubbf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zuqyavja.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gybbsjmy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xltkeelr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3maxrvsmo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tsqedutr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3juvjiqnq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fhvnuqjv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dioagxnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cauzrjkg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lgzlkblf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yceaeeof.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3arsohvim.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gpdjdjnj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bnkolxvy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xudspnsr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yhatuoji.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jzgszrdm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhyfcszl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qzpqvpqo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rlwaomkt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3thekrdiq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yzymphqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rcswgzsh.html


<!-- 参考信息 -->