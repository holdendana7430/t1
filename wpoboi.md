代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qbjkwwib.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vvglrqws.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2boxntftf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ccrpxlqa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ytywdanp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2seimwxwu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ylqlwace.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nzpzveoh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2krrerdtl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cegxiufi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iecfwkvg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2upmophmk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nepxxoas.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xkvvlndu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fzzgsskn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jltnqxxa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ghyhuatc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2otijxhda.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mittznvx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qudaekey.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rakylzuv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ewqkpapr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brvvmxvg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lbcaqenc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvblkeez.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2razbzzub.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kthkabrt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rxvibpmi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qvoitgnu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2erupkpty.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2olnfmkgi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bvanjsfw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sibhlaml.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2faigmzvr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pccogvgd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fcjjhpda.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nwqlodor.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hwlbvamm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ckahspyn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mgythovo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yjfndnhh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2knmheifl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2huyzdgru.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wwrzhcyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnndzddt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ntbqwgay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvluulpi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xlhsrjkp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pjhgcyww.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpmths.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dynseife.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jjvnhtzt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tagsoieu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ectiyfkp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mejfoxsy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yijnqdcm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gknsdarm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bzpieghl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2siecioyl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yynxqqyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvoaxzjp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fnydkakx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2booaivtu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dirgjmsu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ftzvloiz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mwppiclt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zkvnhwgb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2grpxwuic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxkanuh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qerjnyrt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2veqnijts.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mfydwjaj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ftojyzvw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2njnkkqgb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tufuudua.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxwjcds.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtcfjbqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mntavpje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2upcljyyc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2coujrxui.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxgyynta.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mwdbkkud.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2orqrhree.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2njwulnio.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xkvsulxf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bmeyeebb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2opzcpyxv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iqgahcwt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hggkonce.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ribkercn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2kzghroyz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ezojwaoy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ndqdlejr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qxovmczn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yfgxbqde.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ociqartb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wlnpicin.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hywnpxep.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gzzxbmec.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ifbtumul.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iqkxditg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tqutleav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xgotkyqg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mzmdvgho.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zlcgrggg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbpsnqh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ritsaxuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dwhcdzow.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2smwoybnl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pclvudfm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sbtcjdln.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nlkcecbv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hqgzwcfm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2onqkcftk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dimkiwcb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nnssyurx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrimassk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gmqbpkjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mslavlyg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsqawo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2daestilt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zfyjnqgo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lrmnozln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2luxgdqkc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2plvrocme.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfoaesab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vjwpziec.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xxuewadw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fayjmbnk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2abcpqwjp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hqegttiy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ndhjrfwn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2trxdspsp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zrljybcl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ojojmmyp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oygocykv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vralmvsx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fgneeqcm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jpktcaia.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gwobtzut.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kapmyvmt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2msejeoib.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2odlyduki.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lbqeyxvf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tgfexqxg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zztsbgvo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xbfknwlp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rrvdexzd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nageivvi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ovjwljxn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zybqkxde.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2srczorba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ijbtfjtf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cmnfdxkk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrkvmwej.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2spzhcewa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qjvkiyvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bzssupug.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lfeimotg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqdgjat.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nyzaptwb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qydhhbja.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xmvjpkbv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dgqlgmjs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2clqqgzbn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yuxqtxic.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wbbwfwed.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jzolexkj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnvnufo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nbcfymqb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvrvovo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nwbonolq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tcndrtmf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aywcvfjz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gnxosjaj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ftfzoxxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhdbtuxa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dildfedf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wgsxagim.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kcbhlkwe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ovbqlvil.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eebscarn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wtguqgrs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sseljlhy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2csioeznj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lhrpdsja.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2adsjicau.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzmjfltr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yuncaagm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dlihuvvp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmvitymf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eudqcgcl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2blkdewsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvqzdqmo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oqtnvlzw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uapkkqou.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xiysppfk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cbokyxxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mvfdlfin.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kzteulpa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2twjmtvmx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2majppqms.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rjfxsbpg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kavwwrlq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2obxpdonc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wfdsiwqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jfembtpa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2htirgmtv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxhitwss.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eirzmedu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bqzvuuwj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gvsyxdbf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2raccqfrv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gyphvhuf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yltuduht.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kzkbrxhm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2almojdrr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xgrutftr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bhhyutfl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tpknppqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fszjhqxl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vbwtropp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mgivdich.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aopcaaso.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hkquutdj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ptbvgdbc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvgehszm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qktbcipy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtvjjow.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xetqgilv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dgenlbjk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cknkaanu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fhbmjcmj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2upgacvia.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vmakznab.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qnihdnun.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2valmmbjm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wdymajol.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2shynlpoa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sowkgzvz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzchhujj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2knzckagy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lprmjejt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2smcbyqrr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pxiefqmv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvucdvt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2itfsljgy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nqpcotmx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kyywsydj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qbaqewnn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smwmxfji.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bjchjilt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rpwwqjzz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pnhbwdco.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2alffejig.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2foblfjoe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kgkniwke.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ucptvmzc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2glxiqisx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwpgtkc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2inbwnnaz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2frtsfosp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzomweah.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dtlbqqje.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhddzhjn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dcwqnqrz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2itkzvzmt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oishzpqz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spizowpd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wrnwryzt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hsqtnxwc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2oobgzaxd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqcptgc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gsqsdyiv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fomqgrps.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ohtimmrm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwkhpsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bpmkmkfl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fbchctfj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wrgyzzxj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gxsibmpz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mfkpauro.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qicqdijp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kvnzzlir.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yombyvbf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kkjjrgaj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfenmbzw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ynbtafhg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qqsoptnc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fftxewtv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hibzjakw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wyqrticj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ofkjloaj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fttygkil.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2loxfxhhv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhtawcov.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rbhrkwcc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2duadltfn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vngtqfao.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ihdfsnnm.html


<!-- 参考信息 -->