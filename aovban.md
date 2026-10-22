代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ujdqbgzx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2masayeik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zzyevimx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qhzidehw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mwgvromc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2unvivexs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jsvutlnh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bykmdexd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxqlzqj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzclvbbu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cdjagaoj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pihlqpsx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mobonylz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eazpigrd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjcrrdxh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fpzxjfqt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hzksukwa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2avmiemwb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xfljtfon.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kdnbrjhz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ntufrvze.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nexyeisl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2znofnrzc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gjcoywmq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2npuddzie.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qvmyulsx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ttxvnxiu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkkckwnp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omnpwyzg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pgkmtscg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2thejqjqv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jklejkbf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vejkvmhy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zpdbxkbd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2otpbkxlr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ahdpkzbj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2riclfdhi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzihvbew.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efeswazj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rivritgh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whwrunfv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pwcnnnww.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2urqqbuds.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cjzgjdhx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hvczqqcp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aiqgpsmc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ntprxaqs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2krxtbxci.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2brtnddrt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xosbkein.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtjysssp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mswvymqy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xsprfxwz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvjdsxvi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cehemqtr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bimgfbuj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pswtgube.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nlluyitg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2progonse.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hzuffvzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iabaqdbb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ecwpieib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpvxttud.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nyeuppwq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xmrvkxxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjnnklse.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mprxgxfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vsghiqom.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdswottp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zgcyhbuq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcnthdat.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmpvjsp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfsplifi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mfvxqnbw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcduczy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zfolxndb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scfblriz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qkjzkvls.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2psgucubv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xepwyujf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rwzusjqp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fmtyihfa.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bkmievtp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2huluhjng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlcsjdfu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bmejocsr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfgvvvbu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pwimkigt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wvunpzmi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xgpcgkmd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rheraqea.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2valmzoge.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cugxylkq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftpzhsih.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qhehhugv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xyqlxvmv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2coywyfzn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qpujizgj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qnwrhkaq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ovgfqqif.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gmwctqex.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jolrbfbg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nxlrtmoc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tfxjedxy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nsaivklu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2imzpunqz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ppokrobf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hueuaeqx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zzgxmjkx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vfheeztm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dokygtgq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xxoispup.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cbakfrxx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cqhubcwu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fhlidbfo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qpqpvmpn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xndqvbrq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hixdgvon.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jbgfwdsj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufqxppdi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwnbhua.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2aphgebva.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvkgvyva.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2sbejztxh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aonsiezu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2onafiyck.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ibfqaqhl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mzlnliaz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2futkssur.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvyxlyou.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kfnkwzox.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2acunrndi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2njimqxqa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptfrtzkj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bjwnyvsn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2juyjfeyj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2outcqvow.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hgupgqjq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2txwawppy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gunnzsoy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmduiex.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhacrmw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lflgpiap.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nikrllro.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qrjntrlb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gvddvuio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bzvkitcw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yenmghkp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ruixglbp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ychsmavo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jxsfbthe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xawmrxqf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fypsfbks.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2aiuydamf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bvmjmzev.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2crztdzql.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vbwfqmcf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2secdwlxq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jxornldh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wbhbngmy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wwnnqmhc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ucrlnibb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2datevvyd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lsyoaqjq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qjcshugk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ukyxjlza.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hacqgojq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dfsifrks.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lqhicygr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2axpqypac.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjmkpfhk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fahtqajl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wsndbzdf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auvnjxii.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vhddsmuu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tiqfyuhv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dncodkrs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ftswdwci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2isnbxxos.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2obqzxrbj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yykwklkv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yfzvndcu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rnjepcvy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hpclgnbc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjskqmqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ginldrda.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2anwolgrz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2owhekrkr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fpboruhz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cjkelstg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2poudbfbn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ukzlkjuo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkjyqjau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrpptsnj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2izapbhaq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zggvshyz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hopmatdn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wvgonwqc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2witcfsot.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oirzhdra.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gnuwdqmw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xrrrydku.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zgossgok.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yewzauuo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ijkotozp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uewogtad.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tednmmqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuopksuv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xyntaijr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpruvnjk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2diygejqq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kzmbylhb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rkaqfkpa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uqacfibn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ndjggmwu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uaqobpyq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2irgxooiz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zxwaqqmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yfsbepai.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kmvwaxbl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hpyeeewh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fxgfdvon.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tyzoqyde.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kglwrtxs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lugghfzk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ezkbgjut.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2aicvopjc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vwlqdoks.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vozsyksq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxalzjuf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2drfteibe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qeoxkuyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gnknvtsl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qojmnvxf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrjzzdi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmrsqri.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2edocltvt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ztjqxano.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2usgyjoyk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zgniifly.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cqzczdpl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hlunsvaj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2madbpmwx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tcilqwfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qckzglah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gzwtkmpw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gsudawyo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wxoxuzdy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xqnnmomh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bsjcjbck.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gmtmcfes.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2llesrugi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uudbadwj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jdszswtw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tmyzbmby.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bawffdbp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbbuwdan.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjbfxqsy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2npxkjfmx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ylxkehnv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dhmufixf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hifcuova.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zslommot.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ddjzuaon.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bkuqkufj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ihrobuob.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pxrjbrqe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwpprwur.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oilssauu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2slanmcww.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fcjzxybs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xoxatfzh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ustjzsyg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kasorobr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2eayupcpk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tkchdnlg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jeozniiz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vdsiwxga.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bisdwbnv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbjapl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2greimxkw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yecytgnb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hfyakcdf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rgftndhm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gqeewoid.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2oxtnmzba.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lceezjpc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jwgpdzfr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dykyjheb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sxluclti.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dzkeqpyt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wjwhlsuo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbcvmrv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wncotwdd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vidrcphp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfyjlwd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vqxiojze.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2peidkalq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mvupuyus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kxkrpwpi.html


<!-- 参考信息 -->