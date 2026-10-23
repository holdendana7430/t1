代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3flqyieat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sxjywaro.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vqcgmbmx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dmwvmgey.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jjvewcmm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nztimgne.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdoyypgk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gpifxrpj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kxlrdxcx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xiqtyfar.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3synbbyux.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxtuisf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pwrqslla.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nsrbfrxr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fhlujmfl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3plsnlptr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3krihmpbq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eezcgshr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pagerjlu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqinpip.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfpmpasq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dvbhavxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jzlaubcn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qcomhxkf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ccjutjgk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zmnxzopn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ohdovqvp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fxqsyekx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3skmvtsox.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nnnpxvxl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iohjglbq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehoqqxvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mwemzgir.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cpzyxrja.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ssxwhchr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bdjkbphf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jvibujwh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rhxxespj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tvkdlrjn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bbnhfuls.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nzeggqnz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zjjtsoiq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wnhjnaed.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hceluyty.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fxlofxnx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yfitqong.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yqfsdsfs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zwauyrqp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oawgsobm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oydtgwxj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qeerrbty.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lqmbnskh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzkxzyaz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wsuzfkqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moblymid.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocessbaz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pmgzcykr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgwkgywo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eciltait.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qsqoyznk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zerphfgu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjdtpij.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rufuqzld.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tgzuybxj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3umzpkoqn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3csowsvev.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rxntifdr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzaasfvy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cutffbug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nmxkmgmh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlnpuhiy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qnlshotx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qdaxtjaq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nysxgljw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ptdaplnm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cqfhebcn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3svbriuun.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jxhdajam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmmovwbi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kulquubu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hglmlpoo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sdazipey.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3usiukfbs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cwpsneiu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xvsakxdv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ferpmash.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qspnwqqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkysku.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mccvnllz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3syrbzczc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxomxpr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3glermvgp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pgvxhnpy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wazclwwt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cosqgnlp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ddrljeef.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3prvnwnja.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3raxwocah.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3driwbani.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ewzefjzx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3okrpvkzp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zxohkmbs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ybzurqwg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3njvxcjlz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfurpjux.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzrpvcc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gdqqdnav.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qeypjapm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rwkqyrlx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hckcshjw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wdromkro.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hvyhjytz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wqiqswtp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiilnsa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pzjteafo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hngjhoxf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3klokasti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3efwbwumb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3upikpojm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mfcwfuls.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3glnefmfu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iwiumvde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hmzdgxch.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ngottcmd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpkznxxz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3skfuzbrh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxzhaiot.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qrpabxax.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwpfufo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3osnidrak.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fryliais.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tyldcxkf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dmiusbhx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wdzejflg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hwrjianw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3idbempwt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hkaezklz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vfzmaiym.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cqoimjyf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jhicfcgm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jnpelmha.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rekevxay.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhvtryur.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ozdhvlfk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mnqrhgww.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ncpnibiz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lqfdzass.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fpoiphpd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dsljlevw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jmazcifw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mwfktzjs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gtqjunzj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rinercuv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jpnsibcl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zyuuknki.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rhifmrqh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uoipopmk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uvcfclcg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pbkcjmbe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hrijzaje.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mppenvgx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ypqxfxdb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxxcoayi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3aizvleru.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3khdrgdet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfubsoh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dwadgjge.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnitjfmb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkoegkh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3auckzgor.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ztquosdg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cvsbbagq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uqzhotun.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kpkkijpa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oimzijey.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zkhywzud.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3keyrtwmf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3itkficjx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3frbfupto.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nhxcrigh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3evjskdkj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vwttyysq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3obnjjdsu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ypluosds.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgsuoukt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fcmfnadw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hwzudovh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wqcajkzr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mjpchiys.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wbhmngrx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qxrbxxjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yhannzcp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wpmkosag.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bspzmbuo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3denbhtzi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sobsczzk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bghjpkcv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqlothre.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gykeqton.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjlmlgmm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zlursile.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrvubawt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wxljmylu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ypmueyvy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bieivcdu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3brgwcwus.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pfivzmrl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zrruxknv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iseindpo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mprnwllo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nwfifebw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wuwlbasz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3emodcrzq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kqnzqxxk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwzhwej.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pxgxleny.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nebuejkc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfvzlrz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ilhfcune.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kjotafph.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gmbvccxo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uonzsrgi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xhorhyny.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sdxatunl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yoivhdno.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnpzbykn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uuhywfwv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vopzycyt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yozqoday.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ywjvfbik.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cedkqswe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ciswjpcn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bnhteyzj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsnxwmij.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3locfnpmt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xxvgfbod.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3itjlikwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3slpmfjrv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ojgiekpx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cbylzswd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qjpnlwas.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbegvfuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mxgoderc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uevfcxog.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3stsmwfiz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wgimbjgc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wiourogi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3piraosjr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iknalrvx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rwreymda.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bkjdlxgi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wfsynfec.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bucskskw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trfprbbm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cshqnfia.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vaijxexc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pbmcxnjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rpchcivc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ecfctzde.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qbgzhqgv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bbjwjnny.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ssttmkls.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sbsfrwiz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tskvnbov.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3unjwnxfm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3georppyd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqvdcvjs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgxrool.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pvnkyiwf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3acjennyh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dzmiuycu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fyjkgekg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbekkfs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zuudniss.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3byubcqxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fvladwmm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3klousjqj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wixvdyfd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3auynpoqv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tkmsqwhh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnjchwg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pplzitlx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hjwqqhwf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gubqlcjp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3legwazcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3txawghom.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iqweojde.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sckaezas.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pyobjluc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fkoqzfcg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rzkzchxb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xymtqfme.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3skulgkza.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3eumizakg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mirynlnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3khvirpqh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mnjyvwei.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bumfkehf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nubypmsx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gswoalqy.html


<!-- 参考信息 -->