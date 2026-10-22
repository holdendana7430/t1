代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oncrddrk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpyooofj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2atvhjurj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vzzziqae.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mfwohlud.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qzghqqjc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zqlmbpzf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dghxeobk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmgqmoq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qlaritcv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2urkzayxl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xidvlvln.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jxsbuqye.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kzoaimpi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2shafiqwc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vlqyiham.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgmucbjv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mnkcyphu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjavbwud.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dlakoiod.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlienxeq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vembepnj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sxvruqyq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nbsjmgis.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nrrvwvve.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wmfyrhqu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eytjvgsz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqqhlkva.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2daksgkcs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2negnxbwh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fddyszyd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nkegnacx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jrnrpuvz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwlvkgyc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2terthefl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nprbacdc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2syznovfm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dgqmztmd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nsatvtua.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fgwsgkiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mljkoqrw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxtgff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgrxdohd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvgpbpfi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nizlbtdd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hxwohcnk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2polfqixq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpbkkoz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2icbmrhua.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zpvpnrsp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qdgvoqou.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2llyzuqvj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jpppyxbu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2eqrzhetn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wkstolmx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jkdtjnsw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zapleicv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vlgzeeui.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bvwbzuor.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mumsivey.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zyainlcs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yyzvypdu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fwjxcmed.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yagmfrjs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xyjyguyi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2myirtdcw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhwhugxw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sheeeifd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyyxkzea.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ohadviqs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2axmrhqxv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmkdpdo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrxalkyt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lqwmxdkn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zslpqqlo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2btktuzrf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vvosuapa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlbxliy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuntvyg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2shbcoxcf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dwylbvau.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hbvwmfxg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tubrkggh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wfvpknfk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2nnkifgrv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lrqawumt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xfurlpug.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sbxegibw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wnhmjwre.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gxoboaue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yvqubshs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2grnhklcr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkrmee.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cntrfxas.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nygxtqbk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zhlyvlae.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qhatxjsb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bgluhfaa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpzonvh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2joehewyi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgpobhf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2szeqkcsk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2toggccem.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qmqwvgty.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2evmivxas.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fozvekwk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lvhcjygs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qpnyrvdw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjiewwh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hflmfrou.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dapktqeg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2glplwmsz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xnyjmhzl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2feikxzgk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2axqmnade.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwikdksj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pevtvjln.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gamexgzm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2izuxexsu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fznxfyua.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqjduwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xgvftkrk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rycozscl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pxtwzofo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2friwcfxs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cdquvfpz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nhjomnxk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2idyrrcxs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fgpnzrpr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kojhzgmv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwjxddvf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2omcqmhou.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kccbnveh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ielrekdo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dzlgdtoz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dphvkjev.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2slkdqssv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cgozcfzm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bqmnixwh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mjfmvlai.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2aubfflhd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dugvmujy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mdlzgzvh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pvvvemap.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pctpqbjx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dubbqpvf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2grzwhvgf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2oipemzwp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sfbheyhe.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sgeeyyxb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gguyejea.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tlybqsfa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hwdjfofb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrcbrsxe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ciiqzfpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sxmtanoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urbdsnit.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2axyvsiss.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2akxowpps.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2neqakosh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fblxrbrj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wvgqunhl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tlrwcgiz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lgbrszbz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mblbuydn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zghrancg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hjvunymc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2clrajifr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hxafusmm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gtcvhaku.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yezgrnnq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2chrbdocx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhelcfit.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2geseibst.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2afkskiag.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ztueymuz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jpzcwcbt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fcaymods.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qognvyev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fiejpeyz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2klgeznhn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vkaiolnu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxycnz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vklegirm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cmzyasyp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ysaopgar.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qlijtuwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oatvyjqh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2egcokrtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umjtqezh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uwkmyoyx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tiigvpko.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xxmpcbos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rxugmrls.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2abbhjyjt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2adypxsqy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2avqgsnkm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kavlbcvl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vtdyeqpd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vmjktfvz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ppbhgtlj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wewmzpis.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2auekdwrg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wsvuvvvt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qxnfuszg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2slejhdta.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uolnjfny.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mvltzhth.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrfukhhr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjmpwbxl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2abzjrydu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vknklwtn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zmvspyds.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xjhslcnj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gdirblzg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qkbvpjfj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ybajvzbq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2okqfmvis.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hutatbeq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfbthsqe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nyjasyht.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uzughsmz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rfudrnqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2knyvfupc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkvutsk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fsquqeil.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2llqgkely.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2klnnbxaq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2seunsehp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lxznjslg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kezlrgqh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xwesnuam.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gsarrbga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wzixahjj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mcfzqtvg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ypulgfim.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pguctuqn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aeghnstu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yovelowj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gffxvfdz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uwjhzixl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvvnoynh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eebmsiwh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hiaqklpf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qhdbfiec.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2flnxlajq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rwxxzate.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wfahvagg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2abdnpqad.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2apeqzsok.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tgfleygi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xvibxqew.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmclyqkt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hbvgoroe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mywakrvt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bdbqktrz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rttsdcwd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2spqqfcxh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2acwbtido.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wuoeoyza.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvhoaeq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ukjlopne.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fuwyyxgc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aocxlzux.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hfdwbses.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tddzrxfd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dyylwyid.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bmrkkhki.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vyybqssy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hwihxrlx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kukibuok.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gnhssovx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2epngijwi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2opicetrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sqotkgwx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuheinf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hpefelme.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tmzfxiup.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdmszdk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jprdqnis.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ljmgpbyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aakhwrmx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtrszk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vlfuasuy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ecnbhdtr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2flnqjmmk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2womejhir.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hvhdwtfm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wkvhwxhj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2apbkvqgz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kqowmtmn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozioflys.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fwkudhuj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eumxzhit.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2otkesueg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohrijnbi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nknoxktn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2asfcxhnq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nxeljpzz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ffwkozic.html


<!-- 参考信息 -->