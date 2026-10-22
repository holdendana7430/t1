代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bjdbuynm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2asmbutbz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qnfrdfid.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vgiyctmn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2enavacub.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2giwwlfbh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmcpyor.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gqijsxua.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mcmrjgkw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tafcrlmr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tbghpegg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xtrsnshh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bexybdjk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qvrdaytt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2utxeskkh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gsqxakqy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfaizrol.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eqsegfpp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2imxeurek.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzrcuqo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbqrtpg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2utcfnhqy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qwlemeui.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kcncpyna.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ahnqxhkv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bowmdnus.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rafmuxqy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mepklfuk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vklpntjr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lynlnsjq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dtgsxkrl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kogrxigw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ymmjqnpe.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2npwdliui.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vlhfxduf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cpigfntn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mzmfdjzq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fpotozme.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mzgylsab.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vsqiikbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvuorajk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2npoiempv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sshnvrwk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mfvinuhg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eafsrybx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bqdqnzdw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jjblzqmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkbslaj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mppftbab.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bexnhpqa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kciavtxn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2slhzmyyo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2owbmrgjg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jwlvpweq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mthlybpv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdfgdqzo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfmygwsq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2etsqzwij.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xuafagtp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2oqdskivq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cxeskhdh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wcqpgaun.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgmeerv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bzbtctoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjjqhopt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2idkodaib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkhpbvc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tlsjhpha.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cyjxvyzk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wakoxnhw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vjzyzdxi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcluqoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyusjztz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ydktadap.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uistthii.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ffttjqmz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cxyiwfwj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aynyrell.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwjyasy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jpmzsrrn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pdiutgsd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vnedlisc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xdbnnhdv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bhowffrj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ohhrvulo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cdhibqiv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rbipfewt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ssgvhkrl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2peghlgnd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lmoynpix.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fpubpafb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ibatyvpi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2garyuovf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2funiupmd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2sybxewlq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ebbfqlgf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2juxyeswy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ikluqnvi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zqfmdchm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yutjtdao.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bsogalps.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xxbjfpxh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oylndzfp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dyuqizvq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qzptrfil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ekcqmzqa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tdxawknc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hbkxexdc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfovhooc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xtrzscsr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tngtojdf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dxhfzwir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kigidhsd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydczpetq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fywjwufs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gkwkruvf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2arhcjmgi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxujhfsd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sksvnpmu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kzoqscqw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkntjafs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nnztqxow.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxqhfvle.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqchgwx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2whipibiw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yhfjrzrx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bhwtwqtk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qtkarwat.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvjgoz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vssyxsvm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2neodcvdc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tiguuojj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qvgjwaoe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2euffxhyn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2czwdvcbb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xdtrgvdz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eqlmsiiu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xawidjnq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uyaxjydz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wspupedl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hupoidjc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xlueaouy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vsewjdce.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ibycxvji.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ukzvnozi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2abrktuwo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ksghdaej.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bmwzuxli.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rvheunrt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tvrvojkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2adphmlfb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2eymoaunc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gdhkvxom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fulyqtpm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cpgygncg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkbqlka.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxgychy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zhiwvaaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hkbpfmxu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vvseqnam.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jpshikqp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iiltdmkn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bkktjscs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xdcgupjb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vxwgarcs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2muolzlez.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lirwuvix.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lfmqduql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2afarlgat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlmycqzb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nmwmmjcu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mnjotmio.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znjxskrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2agwbsuyf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zcknfbmd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pittdkbz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hurvrixl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2anrqsmlr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nbwaejue.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yuwzvvmk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2eamraisb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xjhwhfpi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yjskaxfq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2onyrufpe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ketolwta.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nfmhtwwa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwldktpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxuunhrs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zgrqczvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuyqzfby.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cbaphfab.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zyaotums.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2msfhpdup.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2znklgseq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mzxhmflx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yqndohdi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jjuobccb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rcrxkbcd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2quuuylwi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2orrwjuld.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yprfbkwt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cdclqfvj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtrhwymn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbcgrynu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fkucskgi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zohmvuqc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ytakypbb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2guqayqms.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hnbxyqvc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rnlcggcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2elwzbfvb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hfbwhxeh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bexprwwk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jluypmtt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pdoecnmi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pkrstjsj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xqfctvoo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jdacfjut.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwmmqvfq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjzoyijg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dxvwxctj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wixsbbvi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2slkjpfti.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpqvwfa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wqhkiqxi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwzicffe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpssaoec.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tnazbreh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kblmzyss.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ckrnqpqg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nyawbjir.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tteckxes.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iwqlwjrn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vjfpprbk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mcllutks.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yyilcpyx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwsuzyeu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2deqpdllh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uswwnafa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yscisfpj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bzhcrudr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmbjwbl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ipptivsv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fhlvdphk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qkkhkzdt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ukrmelda.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vespjnqy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2knuagdnb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wjifhznu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xievrtmu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mrpzozdc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tdteiuro.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvwzia.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2larcoaxf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2psubldvg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zcmsogbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sibgxsyl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2pikpactn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejraavsd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fdzifhzy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2moizzxbp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2plvgitzw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xzrauuwi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xugazbwo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcoxelsr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gnmyhsno.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2buhamtdf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2shuvvplz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmlwksl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2glsxmdse.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2unolmgpr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ywruuuoy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxlenur.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2brvudjey.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kkkelxgu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aovicbvz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oakyhpha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nmfdzlxh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xfsybtva.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2msfujwcy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ojmgruah.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yrwvzmtf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jwincrbz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cnaswclo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nkszueuy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ceyyxfif.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ssgrbtso.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xcfogxgl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eqppxzyt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mmtitgxm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zqcwnapy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ztdxjaxb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxtkvtmv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwabrrdt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wcfsfyka.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ssagsotm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pgpehwbc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2suyotdwo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vtbplxvy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzktva.html


<!-- 参考信息 -->