代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ffqazfrd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jvxdiaim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwoaqvx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kqsapeqj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3knecchio.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rrnqiohy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rcwpndio.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tybizunj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxqttgg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3memriliq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ppvaeuft.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ouspktgx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3irhtbepu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hgrxkewq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsyhxrb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkgdvqd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lxlwdwus.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fuoapmbt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mykfqsvb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzsokkv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bnbtirpa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tsjcuxrh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3poypdmnz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bjflquup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abfkjsut.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvpostk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyozzaxh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zkqkwktp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvaagem.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdaxbhg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jmdcsugd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mawvwhuq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fhkrppuq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zsoebggp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ulirccno.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mllddaxs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uobmehif.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rwrgndkr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3femlxqda.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wrbsxdbh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kmsrlccu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfmzmlzm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3okkjuvou.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aqpmiwwa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dihyxxwl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yiegvyus.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zixwlafm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3namfepcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwbkalhk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vabiwvvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpbfgent.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ycbznzqz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gztpofpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcpsszf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tmpjxbxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3asqqdqam.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mphcuqfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqosyhsk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3najijmgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qcxvyxtn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfixpcub.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3seblhxbh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ihzkrova.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wckoyhzf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pywaiwqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jaqsqppf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qboaypkg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hzktexyq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xzxtxixp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gizzjjfh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zamzwdgv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3boengfzk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3okrgqhwm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghvsxpph.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3chyaekbt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hngzbwan.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cqwpgatg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vjlcvysw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wspeybau.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3guziqwut.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uwzfoihi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrqfvvbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3adbrfsrn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uramszvy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckmbfzwt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqrfrib.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofiidzoh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kvyeuduu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ymmikfyn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yyuldyge.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3flxyptvk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3piffsdyc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3scrkvuvk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oqrsplfl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zhvtagce.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jcmsucvt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hfnrbipq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3odwbahnb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3maquqzka.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cjnfatgp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mcgdpqbb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tlgfyote.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3awgoimmh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sqrhjjtt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nzrcyafl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3laeyttvn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hbesdoou.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pojsoibm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ratdfvvw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zujgoozc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzjfpjld.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wyjaacpf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3clkunzed.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sibscmgg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tpcvqeft.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rdpwwvjr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdcfrcdt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrlxcov.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jftowxnt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3csuqmfbs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yflkidaj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3swxztipk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcckbdwg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yznhhguo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xchmfdkm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gextahyb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wdpsqhlv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lzwpjtwn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebovfjdu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vkfrvyzo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjslgbf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jkedzojz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kjeomwfy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3sbuygudi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ihpbvank.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rsghakqv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ywpxjdsu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hlxvxwiy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zdfluvhl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3shtqwoxu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wjwkypif.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sizazasn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3itrhzjdr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cvfvebbk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rgkldusm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ytbkcdke.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bhaxhskv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wtbjkkky.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jtbvzhmh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3griybsze.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kicqhhse.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fklozeod.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ufxjbzsk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3goaorcnr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qogzntsu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gmvjsryv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bcjpuugy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jlxjbbdn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjiuwetu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3sgxvxhfr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3urydigvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrmofvs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ygdoewmh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ihockupf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlcqueif.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3danbcehk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3czotxalp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3axnoizwj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3diyocwfi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cgixplyv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nkpwqech.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mcpbrvuo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwolfxd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tiqqajfd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3nzlgibik.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wldtnlzz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3foexcqjj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vywnkpez.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xldezdvw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yeezjqdm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epsdxhnm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vupedhpq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kxgmqqle.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3baxffzfm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vreduikv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fnduxufs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3apylblqa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bcugrqhj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kvbcvccy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dxjfklqr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tnaxmwbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dimkbwcm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3elwzzqjv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yxvbzaat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3daaavroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uumjleea.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fvwaduml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfswdwwo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cxtktnom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jepebfyo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bgoksukr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qjitbxrb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qowrfqnr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3thmuqpos.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gunvcpxb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3iygukvwz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ulvtwhnx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ilqbfaxn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vjylprjx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yjbbfsos.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcpabplg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjezddhd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrpxxo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ujbxmsfl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wfaejwgw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xlaffqug.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yqbpeypg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cjyjhjjm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lfckuiwb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gpevtsqy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3exlelqch.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ontglfmn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cpkjdimc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3poctjvut.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fvtcajnd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yfsmibbm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmpwgblj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3idthhxhx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xunvderc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mqvtatyk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tfrzmotx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zwpouzql.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nuhzcesv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3irtxrwem.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kenwepen.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3joxerslu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ojgpfbcx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3npagkvhi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3glnqonny.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3otadvhzk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fgcwduvu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nqvobhlv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3butteuhg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lajsulsh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3osrgdbsr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cyuwnvww.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzkgnqeu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3foycpskq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3eetmnxvr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzwletb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kxgymbqw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3egyieuqo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3akemrlgg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3phzluzzc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3doeoufpk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vgzhypdh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rgvboddk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3illdygrd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mdeujuak.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jvnqlxkg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbkjgrfe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wnsctcmw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wloeueye.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uurrkeju.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sjbxxodp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fuzvnovb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lmhkttdy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hxdqbpgs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjnpqaxd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ucsgztfy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jqbbucjo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sgsgrlwm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kexlesmy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pubqykch.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qijwayhq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3khyayjnd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfejkvog.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ilrylcbs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wynkqzjz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fjmuwenm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qowrxhrj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdrnspfp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wjyxenmx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tttqiccb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gckxnwtt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gksrwaft.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3szcdeidm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xpiwujro.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vwwvasso.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vwxiocwh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhxbzqyc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mmgpoqdw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3twjeteib.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dgttxxxr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwgzpxeq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iqfarpmc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3djcbtpbh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bnfqshyv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ispkpatk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3izfqidsm.html


<!-- 参考信息 -->