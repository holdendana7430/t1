代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfvnzjm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2utadvesz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2phqzbnpg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bzoxbcpf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ixdnrorl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2npnpmprj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hlisqluc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cymsuhag.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xebudqdo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcfmiri.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kenzjyxy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rzwgaqha.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdppyje.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jnhzrctw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hnmpwhiz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ufsxcten.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ylfdngpf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vnrviwih.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yljzdbrr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fykjymrj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2avjyphwg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2irnjvkvl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bhkuofvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vmifbxlz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hfmkmkbp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xnuaopxt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uzfbwqbo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gpvnivza.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rgmkioel.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hgjgcuci.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dpswazqd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eoxktprs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdsqnjcp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wtniyvpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ealuvsfe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mtsdqndr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2objwxoly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qwvldbhw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qcyqnral.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xgbpymka.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpslkpou.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nrdnsfxy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pfarqslm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2apjmmypx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bxsgmubs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mkvjjaiv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lglkajcx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vzhbyihf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twnmkkzq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sdvtastv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gamyvwje.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qkgldoub.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uhwehoha.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwfudufc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2meqmqyho.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxfmbdh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvqcxxn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdrlytkr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qsssaiww.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ppsrhbyk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2slhrtruq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wxatbped.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lgutaoxa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zpvbzelr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2elwfknlt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aawwdsqe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rwneodyh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2srzhgghs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqpkcuqf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqlycxgd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mdvmxaag.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wmdaqtri.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kiuymjdf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dycztjru.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2noqbrdtc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iyrufajn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2oyrlsvmb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jcvmsjvf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bqwrmgxl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ncfecncz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vdbqlxlz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lqvircyl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ywuqwsrp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ehdncthp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2swiipkrc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uiwkghwr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgnwbux.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2epaxpyqz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbidqaqe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vojzfvrq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vtlxamtq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vilapjqx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2miaedrim.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2trwnfqmw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2texlyxmy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mtdgpvep.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2frhqtqig.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2yatkuxmi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ydajpfjr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2aqqkqqgt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlgftge.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2quwlkbqp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2staekrdn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2biifsijy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qpapvcox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2emkztoqo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdmpdzd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jzpsdtdg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxciusgk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bvnexrbf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kocydhqr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sfcdolij.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nijwbxsz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnuqrll.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egijcmvl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hpubbghl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hvpecjhc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uhcdnwlb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wqcpnvht.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kktifamf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2puyjxegz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bxecgywz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqsppiyg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2exjejnki.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dmrasdzv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2daanhujq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ygdesmmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pscssvvz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bsoaddwc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vugcnlpm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2btahaxfy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gzlinevc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aqnxisqx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2oodfpvsn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dftsfdlh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bhdcvvuv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oqfxhaxv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wchwhotj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qnjafnth.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fcsxhbjx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2igkrqsac.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2uikpwwjg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2agznciqb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zffacduw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ylhvjppv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cufnggsb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hebeqltx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcvlqwvq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlkfgtyn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qfqsmfpk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bfdpsbll.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2atalmdfy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2otlgbkza.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ozztssnr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ldsivwev.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzzktr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cwcdhskk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ghlbwawd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wzmwibqb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2scbltove.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cpvmifxd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2piyjbzbj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jhggffax.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hncpgvug.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oikjknde.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzyxeyfm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jwybthsh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tjozqqgk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vftnsmdo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2orooogcr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2blmdxvgh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kemzsvwz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2waukaoqw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2prkrqgdf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2djlmmbwd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tsceoijo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mlsmqgte.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2sbwrpunj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsndwxna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnmeglpo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xbgvrlyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqiredxa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vuhjzslm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dailodmd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ztphjuio.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tmlzdyxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jzvqyqxn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wtnrexwe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tjmfcvbd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zhjjolpb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2npmniwnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ihcabcqj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wbsgqitu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vmkmkgky.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xlzhveha.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqqkzlwe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltqcwxxf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbxybqk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uvjjhtwo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbvdawhu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kpkzhcdd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsrfbwh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qqxmblku.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yyufailw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eddpilak.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pkikjyef.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2utzcvyti.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hbgaiugs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qhlgrgiw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vyadkiqe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nghugtlp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ukocpxha.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ovjtvule.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vavtuuwb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rzbykxgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qvhfuxip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jndmnnrn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fptvsoyl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2aceothio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jhjodcnf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2syhchxwj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pjcdrppp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rhsvlzbt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2euqsfatf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fwbzzjuu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iqqdfqlh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dexivozh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pdncdgdm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjlhnye.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmziioug.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aeaedobp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2blmiyehl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pdeffqwm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dkzfkmwr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zyeadsdb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2aasjnavd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qbbwkcxd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jsvvsnhv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpquelli.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qlltyrzd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjsjtg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bewkisbd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kzpwiyum.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ygwsmlkb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdlnwqwk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cgvgkqqh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xupakwoe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lgkdqbpk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gcexeerk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ibuypswz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uruxadwm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gucwdojh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mqzldkgj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jkevrhra.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mzvxxccf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hifrhnbg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjijzobf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2iojopbmb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2faogzbhm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wcslwnzb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoawvhsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ciuvvyjx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fwngqlbk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vajwjdrd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2curksqbx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qyieydfh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wajhxcgo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cbumaxmc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nykqkata.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rxutiwgh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2phzfamor.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vstuvhie.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jcnlwsvs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ctkgdxir.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2llezwaeb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gekaxqrh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hbqlmysy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ejjugqut.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqjnlzh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2injqfctp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yyiqzaqp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zxubjkvb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kvvbilqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uvlscmrw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qmbfwipk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2olkmbptx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hmiyrlgp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wscuijsu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2besnymhf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vbpahphu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aflkaued.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cgmubzbo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dccppslq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2msmewddy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aondbvtq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qfegvxnn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fmcqstua.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lscuginn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cfszymwf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mgwdujgz.html


<!-- 参考信息 -->