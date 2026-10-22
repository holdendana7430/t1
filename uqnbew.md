代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2drpbfdsh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dekzhdfe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yveimvfe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xuzpshkq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tcyblqhp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lrzissyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mucmdqdy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ysizpejn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vwgzzzss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vnzqrfwl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzmbboq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjtnwme.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2btgcfdco.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2toaqmvrj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kevwpusp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gxlahacn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2blzuysix.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2iaraekmx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysbluuoh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rukdeggy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2peyygone.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bbdflnhf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eynwfjqg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lafrkqcc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzrfvs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ductpzsh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fjsiibbc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fpcmxxcq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfoejblt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pguhnhbm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2grlxaivt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fphgnykf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2auvewidf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkwnktf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bfhlobtv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pjmdvuud.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mpyggkon.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crbtytpj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bnvlmcbq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eswhnxfp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ykjbnwcx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pzdulnbg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wmudjafn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hqbwbbdo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oeiocizl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bchjphdg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nepsaftm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqnocu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hummnkwo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xoqgosry.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qlsbfdnc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zezyvmxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgffsbgs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2omxknwmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thcxpjei.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2juvcasme.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dkjcmsdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wesrbmec.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qpqcpvsp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2taroxzlu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aisxhmvw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aatnetqa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2aochemny.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jojtclju.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbpnprcv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qmjyysya.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmixgoh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyohnzak.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pfqgmdpu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zckkzpsy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dfjnbofc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ejjjoqem.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uhkkrlow.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2aivyyfeh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pesubjyv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fmjwjvxb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kgltxvko.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mhguhmws.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zagapuvi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wnytolcj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jpqilmil.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gkwgyfct.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2optehtib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2uacgzjob.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lwkqleob.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imrskamq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lkcvhdei.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cxznhunk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgvljvxi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ljqhfsng.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ydkubljn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xdngsqtg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lvqlqzmx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gelfynyr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2piuxyoag.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ieszbcca.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wbaoevlh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hzbmakpr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mdcgyjcn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tvoabryx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bfqzyvtx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2knyuvmaa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vykxtubn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zjjsmolj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qriqmbex.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nhbcbcpg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2syhkydnu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmymtua.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ritfxaln.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2waxvmttp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ycoaudeq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eangzzys.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pbllyzgy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuglvbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dhkzsvhl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pzezxuwd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2cgzcmqbv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2llzvwrqy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vxbjtwyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ysiljeqf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptiunxbd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hipubegy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2foczacwo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gzwjjqtk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2eifolnrc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivdtcmvm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yregpdik.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oqqguftv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zeysibvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxsxjrv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tehadrgy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yxhrxyqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rhgrjmqa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2srxoielr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjdiszx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2shsksshm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dgbltnrn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yiovavyo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hrjucddi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qkdttinn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xuakrlmt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffxkgrwu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uhrjbvcd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mmcdthnr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bcwknxoh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ojydgtsz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2aothzmvw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lmtpaion.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wycegqlk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nxbjkdze.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2swzragxg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ogsrhuah.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ilmthcpg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qfbuicyr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2damwwlbs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fepzgspz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zvvjwcoy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pwwsrnnp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uopdlcgr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2djecsmla.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fmecsowe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gikbgyqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vzhvkgrv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ycybrkwt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lhboczej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xvxuoenb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yuckdseg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzgddxm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kitsllll.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jjuekdtm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dlluvovl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvvyxae.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zlcepwsq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yfhlxikn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uffzzniz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dwcnwkxb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2chuebuty.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iesofbkp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ttkqhhfx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aojgiqez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eqeteczw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2smpssqva.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mhvwlbby.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2axqcptln.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyuqriuy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drvfhaxe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bnxuoebh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tovgmgde.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fxxjlbde.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zqptvlrl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fnqlynbb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gdgysuum.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yzvjlnko.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jwoihrvy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xihwlwxk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dydlvmwn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lghhyjbh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yujthbmo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mqrdxakj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkvsrdtg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xziwxrkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mifzmnve.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkqqclmt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zpokknpp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kgxebann.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jmjkcnef.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tfkcqxzv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2syzbxbic.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ceaxwweo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nbracvbs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xidkszxg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gvaklrfb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hcaryujq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2iiqsoywb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aukxmsgf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2srcvixax.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yprhouge.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2heousxvs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zickmymv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdudltem.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2htfvstub.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2czbkpxyh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sbbikzde.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gemavjyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xvvilmdy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shfmblew.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jnkekhgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pyoyifqj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tbzpjdoj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yczljqyy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2imjuizxu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acbkvdzv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zmtgfwtu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dddslzmx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dzelxexe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ztnbqjho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qlydskqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vhzzhtqi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ihiodymf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2okxarsth.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qgxwrdad.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mnyrzzji.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gliugdaa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qgmlyzmo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ckrgybge.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ihzyumfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kefzzcfv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbaxcubi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlkkehai.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ttklzidp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pbmonjbh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ncxplvxv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gxqskbcy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhwnwscc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2isyhnuda.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pgjoanok.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dhjorxem.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qwbgqtmv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2reidimpw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ajtsgbqw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2letsjtsh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwrqqqqz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vpxjdilf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ynqfebii.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcpuncjq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlrfezoo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2omhfrzen.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wfogjicq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2icrelvdv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tcdctxzc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfzhjipp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2agysebcz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gedyganq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2waxjdebq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2knrogppr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jrodpblv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2alvcrxrr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pcescsqw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hglmeqqq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2thpxtqbs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amucyhmj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gtbuvwqh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2atjcyvfl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zvuqmdpv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ontdhlko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emipcwgk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvtfhjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vccjzvci.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2joocynwe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gbgleuyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hsoqqyhs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bjsujsfg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ybonuprb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wzochyla.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kfhdqhfj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fqraczad.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zfbmvzsv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2yrfmpqwf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lterkpjb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2byojyobt.html


<!-- 参考信息 -->