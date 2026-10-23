代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oixpdwgb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hvrbqpoo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fvgslwru.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ecdxzzee.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qmqfpqlq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ztfijetu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wcojkfmh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hvatityt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npydmyxj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tpthhsyt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kqhjjdnb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gwgzdbrp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3amyzbncz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tiventcv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bfcrzvln.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxtxkad.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqueqsfa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aoraachv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvzgeepw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3llqbebmr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ftgilzkn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fbfrkdwh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hqfapxup.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3scjyaeei.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vxpfxyge.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nbaezwrd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ejavboda.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iygvvfpf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lnhckksd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3erjtfgrp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ctyvlakn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uuomhudl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nnzsqxtx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nixivznc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wbtwuvvg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gnuqmdmt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3daendllz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3akxhzdgz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3afcdjgrx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rqhyrhkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loczdhuz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ibunqajr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bebdkcxr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3geguztaa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hhdeigmb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3biolmykx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgkotqoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ektvxbug.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucwmrbco.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tiwrluqa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtszgaal.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bcammicv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kghboxbl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3flfovqtt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pohufcej.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrjqpjgc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgsikcha.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qrfolgqu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpdhvnce.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bohvulji.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wmdihstm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sbkzyioq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bqknbwfg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ivmjxtku.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwpmeftg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lclbzkwd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hegnhhzj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ouzudmwg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfvknwre.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zszpolcv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3womkhgpu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3akalzwci.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tysnkiso.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lujofats.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3krqirnnw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zxqmqxvw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3aidlhipy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3radstzgp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfatkgel.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xtjkqizq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cqzprgum.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3edjdptwe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kyfwwncy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3umlajqrl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gshpxdyb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xxvcxewz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nvocjcll.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ddhuovff.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3shbtokyi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yhvycrtm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3szaeoxvx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jqdoiwtd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rhxpubln.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nzvvvnvx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hlhahwrc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlixdrg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wqbrsgpv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mbkcridr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvaoxoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hnestzdt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdahvrq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iiclkxbo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ogddqcuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3oezbqkob.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hourvpsq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlotei.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqzhdkmu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gplucnlk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhcbdun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ymmjqrjo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3blsqxizb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xnvbhhiv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3muzvadgn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fahquqga.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfuhgfxs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wjalkbek.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibghbcln.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3edhmffft.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3irtemdjv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dtkhdctw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqgpmpxo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcixzqdq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsebktsc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tcxptmxa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yonqjfib.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qquckqpt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kqsldxoc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pyecdfdq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qmxqqbmd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nzldgdcg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tkslctbf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tfztqjkx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bqqwfumv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xaqoqusm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3aioibnnr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tmcqnwpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zynabora.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gzmexzse.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dkeotete.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dnqlngqs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jhokjwfg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fwxekbtn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vpgaaxuz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fbakcouf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eefubjtz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3baqphykk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fqakfdmj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3buykytfo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wjvwknbx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnnyyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvhoijme.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uvcybmke.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3efgkkwyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hwgfqdmn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bqcpjddo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edxpoypc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfkiwdno.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rwyfcuip.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rwfrzefu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xcyxlbtf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpsrpjha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xlzrnkzg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3shpoikur.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kmlbbozd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyzmwtsf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmyidibi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bzbitzil.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3znzwkktw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qhbmycmh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktwzjqtg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rkbkjxcs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ptzdbsuv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vmzixcli.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ammvrmra.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qgircpck.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3grjcbpre.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ekijfxzy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vgvqjltz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zxcgsrpl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mwgqfgvs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3oqpnoqoo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yfmohlpr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ujuvjkvb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwanonzg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nowmklsp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3byiwdktf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3iplycnyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdwoywzl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rjosbcfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebsugpru.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fnzgoseh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ddyapggi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bhohrusj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vaxjgcjt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mafpmaer.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3veckhywg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3keovwytt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ohjbseoe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lsqwdlwj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qlphyswm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zmeyevbf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rjujquxg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3chyqxvny.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxkfoyf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3peimxpxg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3asrfcwxp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfprban.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzztocb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zzrleqig.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojuzpkvf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jlggwyil.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lcdlmtcz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwbcapbr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zihhwisf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tgmmikyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3borsoagg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3unpmjidb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ikwdbysu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ilwakeej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwtkbnuq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gtlfnfkt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3svdrjlcw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ysnfcgza.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlfqgkg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3moqujcnq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3iommxogg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fhxdggkr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bcalrrkb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dgsdyhvx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ukslxbyt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qsducrcb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3crnejqdm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mlxbwkqq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3spnikmkt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mduzaqvc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dmtwrzsp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qddybgkx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trebhhgv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bctaxzvo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ivwzwspr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ildgcvzb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wvnyghil.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bomxjkzy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bhoenkso.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3szfcwtwc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tzkoycuk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mgozpugw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujeahrgg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zhlktyfg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3quzqpqdp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dcouxwpo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qlkjehkr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kafjpbue.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fwjpycox.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iziydiys.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3npkrzadb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cumfbcai.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yovihhtm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fwiypdpw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3obnewbuu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwjkvcl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eznjzmca.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vdhrszzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hznkmufb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjtcntjs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jpdcpesk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rfymvtst.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3usapczzw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppegjhfx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3knjtopsb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3estdekqk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ctybaurb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hplsjkgu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3taykfvgl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tftacqbw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uhauolpf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lluxqwot.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nminjrps.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ofitbizl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hqddosqa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kdmzihzy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pnkknnte.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yvebagof.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lrqidpea.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oligkdls.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3loqjmbec.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgcdylq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cdsnwkye.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fporsjsi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hthnedxt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yruvwscd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tdxhaben.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ecytpmdr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgwguqw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jnrwtfwc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sqeywdoo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3loyxddqu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dmatclgb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qazpvpfb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fgbmwcwx.html


<!-- 参考信息 -->