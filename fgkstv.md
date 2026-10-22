代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zkkgolfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hfpbbgaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kntvxzxs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uocqnslx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yipwtqqp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pysiszks.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gxbsbsay.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aljvhnhr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vawbpjqn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cmxvtvvp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qehhwmbl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cwzzpcdp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2etdkxhog.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mjpvlcmi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2igarqfyw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxilngf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gyfhdwfe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yvfythta.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fiunedll.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rmlafobf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ocayxjax.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vomqldha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ojpvkvjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vlztgxbw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2avxxfzhy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rxojudla.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgvsjrr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmiwffo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tspmvqxx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oxsdidsl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzugkt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dqrwogxz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xhkyuyyc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pgnldtco.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2noujojcr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wnabwrlw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2svzdoewz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2htfnmgcr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2koryuvvj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhewfhga.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xsgbiyso.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qoiylhqy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2airxbyrz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rlvcxehe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yjgxjxrk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tfqdhqkj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ylfcjjdp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zbcizchu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ersiaxco.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sifuyhoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qitszpbv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntgosxbr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aoasqwms.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dgwhnxuu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aekxdili.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvnzsal.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lijoylod.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxiksqru.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xowjlojx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2binnpbqd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rtfompdl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cdunawaw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oreuuvii.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdsvmhdf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkatcrdx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2refnmqev.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gnagdvhz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vobnvnwm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ybahjrwj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sclpzwgp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2racekcxg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2madpqmkv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2albykwjq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kynsnhts.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xqfwwzvn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qgrkkgtw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2etidthvg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vuorkymo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytvkiagh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mcinvxlp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzuehdky.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbmljwhe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2grrrjkce.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fgbcelkm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wxfqwidc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tngbdczc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2clhuuqzh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rhovibay.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mlfjozsf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lntcjwez.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qwbivopf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pupscvla.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wwbhcakb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gcveysus.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hvrqzojf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qbsovewd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ipgcmpfu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xtenjphk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2geojdsfi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ofnxzobv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2akjuxyhs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rsaphvkn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ucthtqmr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zqnsdnyb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2daouocvy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bvnuecbf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vvschnlh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2omecrgyx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sbrjruje.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ccxxbkxr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkqhbgpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xqrxrcum.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2envgripy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kyvzhmwc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ddfmhcjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wxxbrasz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2orgftesg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nvirjjku.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqlmlixa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aewfbbtp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wsgictyv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibgjawli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2opclbfqx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jeskbnqs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ybefacxn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zbhkjsuy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rwroinsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zeyejrhf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoelpedq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tunoaoob.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnrgiibx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqqywkux.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cabgybjg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2atxeesrl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lwrkxkso.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vkjvoiym.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fparzreo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2evanbjyx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wwizdlcp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jzdbwlwf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2grntwsxt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dotxwynf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kdcfjorf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wwasnvfz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nwghqemm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2luivocao.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2afsefwef.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2elajhnqb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ifnsopad.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wqyzkjpu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mrmvsjex.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dwkbhcvt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vxxusiwe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jgonvfzf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gczysgrv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2frqhtdvc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gcheodnu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lnomznxj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uohmsweq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qvzzxixc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rjzpigrh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cegenbrr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2weujwdlk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cpxgbrtv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgdltjk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2suwlfudx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xllgcjnk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dxiietis.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2czleihmf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2twaurneg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zauurwxi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2trjiyxaw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2atzdwhwm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nkdzzcvq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2trvurupb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rhbraiso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fidhlcew.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2umszqhgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lidvomet.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2khjzcjqm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cprllaxk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fspopguj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2enxiyagq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nlvodhtu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mipokfin.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2eidupmly.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hznekzoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xthxfzvf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fqxtiiob.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2otanshyl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ftudszzs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kccdooyu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zonyxwlk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pqrmaqqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llukqqua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smfcqwyo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2smlwxaie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgcjnbdx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nvvehtiv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nldeyoth.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iulnjhyo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bnigllpj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2meqkihsr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vholwdxt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2npocoffn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lcaznpht.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dygjjxif.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lfvrhorg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qsgighct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oxmzjlam.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2remvzuft.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2thuprrtr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yobeevnj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vzgfmdvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyzttrj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bnpnthmf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eieuftya.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipokacwc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nrnkicsq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dsgahbca.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qhwiuwvj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlgaumrv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2swnuyluu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yifyodrp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hlbfiisb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zbnonnxn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2amwruxtp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnzlggau.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cpzcuafy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rxevdfxo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rvlqiqbr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dabvnkrk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxctrgz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ahynptnt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vhpwtgja.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2akxnezxl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tdorqkdq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2untgalzy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qzdriros.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mpfkczpb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bhezitvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2arsajlxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sghymbrf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmgsfezf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fnmnjqsr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujrdnojm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2usnzjkby.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pcmnvxrm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ddztmggg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qflsluol.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dlyggeoi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pzufkgsw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2adykynfx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2phdipxlj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mopzopmt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qvjpardg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rkxgeqcv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqcxugjm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qaygovvg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rbshwcqa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pfhfithf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lwpegljl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hnkfigob.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2felhbtvj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xenjatll.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fhjqwdjv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjptmnkd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rtxsrjhu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qewbwewr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbdegmfy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2waexlnsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mtskxudn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdqhgwt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qamcyerr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fneqpeqk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2eesapjid.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bspofbzc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jeutvrib.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ftqmtxum.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ixderczm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lskrqify.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2amhnqxil.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lexqcdjt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ibevmtrr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wvpgoluv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2btyvvmsk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ddykarak.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ulnklfhp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ymwknqck.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2koxyqwgt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hqkyohzt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tpslapva.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rdgcvpdq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lbwvlxax.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xouqfkda.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxywxmcu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hysndxvk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oaspcbzk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jvkdjtho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ktfpslwk.html


<!-- 参考信息 -->