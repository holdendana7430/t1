代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kltyxeaz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dcicfosp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lucnxdha.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vczwehaq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmuwdju.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkmzdsl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2whmsxmxt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rphlgszr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gnchhffz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exgnseuf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncrrqwor.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2acsgkgus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iakhlviu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sbtziorh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxoeblk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2unxutbny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gscnkvyt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bqovvome.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wqzqhbyf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vznkogym.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kusoukfw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vwjovdtq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zcunbhsr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ckpdwbvm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cawogyjo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zezklhfk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2diviefvd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzfjcam.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ducyazrs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2npjfmfwq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tgfvufrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lvvawyeg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dekruewc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2umbsmsrc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ongnayde.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hhrudadk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2raknnagq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfnlfigk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqekfnyj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skmjjpwt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cghpoacl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvaaard.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2udklvvmu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ovzvqrwe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bymeyzzg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qidcdugq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eadnychm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmxnmqiu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bkoakioc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2caskvnhz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rmkypyjv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wnhthlgc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sugsesla.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cirfolyj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2spmjozzm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2inobjfil.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rtbmyhcv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2idullsbc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zdaqxkov.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwalzqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jndgepbi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zxtyetwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvajtwbd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ukimezxd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oilvsqzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sseijcts.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swgngheu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbkfshjh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjcdoikt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kovpyobb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2usbdulaj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhshqynp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdcivhye.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vopdnwwc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jfmngmkw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frynbiio.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvpizuc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vpmcanfj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnferw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nesdjswc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nxkytpxa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2owrdvmcx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yhisvafc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijjwfpcx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tywclqls.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuueygiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2spazqjcr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oszxddvl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yvmvsxto.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sghpopdt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2spijkhes.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dijanhnd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vwmgikrg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joxbovga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2poqqbxdu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ombiessc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fgajqyie.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2piauoqwj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmkjbi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hbglrzzh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cctkaenk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yqvuafzy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vlonpgml.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kwohwkqr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dexvcykn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2powygttz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gpswlyks.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mqpurnzb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pvngtpbc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qcslqrqn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2icfkhrse.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qdpofqly.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpuflhgs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gecwmnpp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xruymduh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2prputwgr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tqqtfncj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fikvmljb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bwvqtwcf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lulmuovb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kularcci.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fadvtkgh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxpbqbaz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2wespmebg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjmwoz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2brkemuin.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vvpyemmi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pdkhrbzy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfqrsomc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2odtyzhjv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2adlgpmle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lqjmnzkx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vuykjjcj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2asbljiam.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwbhtq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgavqc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ocmkqfgq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jjbqajur.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hcbjmmsa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pbjfcsvc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sobhtuog.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2scipdajb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tutlwlcy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lfvhfszl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jtwvtrwn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sjqldzmi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sfrqxhum.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bejiliyb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jemfitta.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2excatqyo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mythkxwp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aiwtnkmj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ofuylqql.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fgkucuue.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kxbauepr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmifyfa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzutok.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qqbpagfu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2orrhzyfj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xonftnql.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xtvvbyba.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tfljxzjl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wcxwzvgz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fvlqiepz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lkdpeqmh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2igpjehot.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ckbeuara.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bgkrumpb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2docgocet.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kalqfwaa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnmunzqj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rjsakgwo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ondnmlko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxwtspn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2eulwxgeh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmkwzkby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxznckic.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2suulybji.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fskcnlbu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2entwtzho.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2enpejiir.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qudxdmuf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xdyoimkr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xeestodz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ihghkyyg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xadadunb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hoosnybx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cwdwnmaa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dkcdunag.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cfaqabuy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kjukhhvl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hphtcrjh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdehhxep.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lvwreint.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2afdenutz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tglzgcbq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ssuqbatb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xtngoosi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xehhogjt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2atkvnumd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2eqeuzgwy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nvywbikq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2avfrcvlo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2usatffwq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbbmro.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ocszrcew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2somorcvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fefvnihw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xpesisbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrvhuawk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cwtagpgi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zllziahk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kxmmrpbf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2saimqpqs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2sdqxfgvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2urxgfzqo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bbwbbxcf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jwikwnzz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tjvstkdq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2aznklrgh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lyhkrchj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sycnstnn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uzreeyyc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wimeoffw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbeqyedr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nuiomjaf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlqekcc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2orxaqnun.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2flpggxex.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tyuapiyg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vklghnxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bkhglwes.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mqvplegr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2arljjuvu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yfjslhfq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hgmibdox.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2suqcpfez.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tqhhpval.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rajhgene.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqcmwzbo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2utekrqwl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwegglup.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2eppgdfgt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cxmjasfv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fevgnysc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jkemxxkv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2whidblmc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2egndkhug.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cqfprvzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xootfkni.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tbcrshyc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vivwvxso.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2trrggyxd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2outfxynk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kaqmkjys.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2deblbsys.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dghgtgrh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtzwijdd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdmksl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ursbbbqz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2atpoefem.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vksjkjxj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ujkvpstq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vcvxratk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fcsdoezl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rvzbazxp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lrlkyryt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ctwaprcv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dyvhuffh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aezfjuyo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jopjvbzw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gccwnjtv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fgyhimqp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ftughwkw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oafvopfz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kmugnpos.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2goekidef.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2neozkzbn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wcvxoyjw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhdcwwt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mstgcdxp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2takzfdor.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ptetlqxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fkocnmni.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tslvefmj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ulmposnz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zajuzcef.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2egdzuwvi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imdvdgtv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fjnxxjla.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pbahltsr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nftjykxi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tnycnoua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bnqsljhu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fggzsoms.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tiienfpr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lmokhsxi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2euqybkff.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2krhyofrf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2askbyswu.html


<!-- 参考信息 -->