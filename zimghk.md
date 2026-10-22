代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yupkvzvj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qdjrcnzp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2prkcbzze.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2krdfheki.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zqvorizd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hzqfgvma.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zydevnpm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uowyplwq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ipngtkkk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2oaccfmzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2blgyxnfr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kxgjpkmg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jhhaztmc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yzlnaayu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2txxklfcw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umrngjzs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryamxsub.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lpvcipmg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2waknlyzt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kesnxltm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2frpmagxv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2djzsxgnc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2akmrzlsa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2txybgffo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtwocric.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znzlisny.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vxbibhgg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xvqwtwjg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lvrqncli.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpntejfg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mtshfrfz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hhtddtff.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zwsbhbwt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2njvwsdej.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uhuhakbb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bamgowbr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pchpafjv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kkithhfs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckkbtzbg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bqshseym.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ctplegva.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dthfbszj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2udtzaxfh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eecmgmtl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jlhjcgvc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vsvhumra.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cjhnmhpf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dpotkdmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnerqzqh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zktiskol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajrwgbeb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mgvsqdsm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nnekbmjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuunodpg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xlloohud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvovkxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2poaljvam.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zbfmeayk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlrdvsqx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcyussqb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqzpfyql.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zbvptozw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2erzjempq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvtevvc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2edotrfxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pgaailrp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qopysfzy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wwvgqgwi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rrbqgfes.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2poblnojx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yjykexce.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2henpidcf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wklzlwvm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ecjatdla.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeyjvhwo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xfnfbnmd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lvlmnfoh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kjskvjla.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xfchoszz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ktyoeoec.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cunjzpth.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2alyqpagk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fqhiukvm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zrouzyfy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkhzmzva.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msuqbgdi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ozmozhdl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yioelhvg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sqoavjrv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vtclfsmr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fniockbi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gkrqixcw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2czaojohq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ubmpxcwi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2sapqecku.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nzbynezs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jlvuhnoh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fmdleqzi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jqptzsmw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jgpxbkaf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yspgnbtp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdgfnimk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cawrrgav.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yxffpjrc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbpttyu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hzzqddvd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jyfphlzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dmkzgaum.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rdprwfxr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2pppsksem.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzhpmllk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2luxxywzq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mhkyqhuz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bhyokkna.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xvwwpbyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2llkrllhq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjpjigk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kyuioyzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eytmoeni.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2tvlvkjfz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qbwtqxlg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsvuxjna.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vuylomrx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddlvunfs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2katdpyym.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dngllwbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2glynnpuk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2inawjujq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zsaalxjy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjelwzh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bepaavmn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mjiommad.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xptvnylg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ymeyxpsl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lcchyjli.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qbsjlnfz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nbafxajc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xlxlrsee.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wwtcdquc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tqblvbts.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wxdqgczg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2antwdinb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2alblvkcq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2terorrsy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2teknkthy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2amyvhtgo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vddqycav.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2onmdfopl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iloguxkv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2inuzyvfk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qmsiwqhv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2evbgsxmg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ohszxjoy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aakeazty.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hkouxunu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2glyjrccz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2weejuzvk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kuycisvk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvidgpsk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nwvwgpsn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lpeozckj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qaarsmzq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2npwdattv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2khgpwhmp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmyjmg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xemtodhl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ghrfurqz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cydablyp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqgkgwwc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2szoswoyq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lqjvenfq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aodemlqw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2verlkacv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvzdqanw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2foynural.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zftvnpez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2abwnlkne.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjymspje.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xnlmicfu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2heohmhhg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mgaxtgac.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rxfobuso.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uumdtgpx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mmxchcqp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xhsaqpxk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vyuxgwdz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ubnaklza.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ltxsncct.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ahiklzhz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bzykojgi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2enifqxgr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jvfgpgtq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cprafpvy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gynojhuf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2skktkexx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zskrohfl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bcribvyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmbwfvos.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2joqhuqcl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hribntyl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nbhcrdmy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ropsquie.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mvcbspix.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ntrpznrb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kknynqbf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2eqvlcgkh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fhxpyfwz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wbkbkjfq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ztxojwkk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2uwdnxddu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rxedgvba.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nfhbiylg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oypdjrue.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gqxwqkzx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fkduyggl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yhgszxtp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wusksmxm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yadnerqk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qjnzalro.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oiybnsww.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tbpsnqbf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xmqjthbb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2artbpjfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bozqrgqr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iceirumw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2srucaium.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkpwqhzn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlbcjacp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mjcrfdds.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wymodatt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cnkzjohc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2anhxpveg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrhokwt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjmggdus.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rhbcqcwk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ypxcabrm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oynqlrgb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zgzgqawx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxxuckg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yigcguga.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2traspwoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hkemjbvd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvbvmbu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eutipxpk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2clhwryxx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyquica.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gwpsrsli.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ddntjkfr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xjreooci.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cnzvhely.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mxhbegcu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cwmkmsao.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mfupjysx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2acsasvdi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zvvhmbza.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sesptyqo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtkyooyh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpicavej.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ggfnzbvw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kcnlnxvd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2drwxpuma.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wryzkxie.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nmpolmeq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2arkvqehl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mzaclugt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zbvergwm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2citvoddp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqdkbegi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2oiktwifc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yybqwetk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2encjduyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uaktddhm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipmzoolb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tqyuyvne.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ncxrcylt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2htdfluyh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2watgxebq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jpigzqrn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rzpaacdo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2moskscfp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2iavwnprq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cttwossq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hjumlmxt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hahwgamm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qvsnzlwt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mzmppads.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rdfnpqts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rsjvejwe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2olhnjocb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqgpne.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zgyovrtd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2srrcqxaz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uxlonyhb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xutfcmdw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsvzcuo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vaqlreyj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gruagscn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sllfshui.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zkcheijx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qtojxyic.html


<!-- 参考信息 -->