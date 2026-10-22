代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbloquuq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zxwlfved.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ixobixus.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nxwhabrs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ydrljdhs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nfjoljbz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ybjywmln.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gpjvrfnx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2crubdqfe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qtdvarwu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2cniazxtf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2eaysawxj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tginkywp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qjuhobnz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2frjahwgo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbmkydot.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ifhdnbcr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pupgpget.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqyivcaa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ouvxcrbx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2omrrbqur.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2uzsgpaaq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pcotuvuk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrlsdhg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2adzpvqrn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2obajeneu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2syymllkj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2suqhhkzq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2krketrdf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2kkvhvuhq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwutkkle.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkstjdsl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdyqcupl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yxyejtwa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2akuaohyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dyquimdt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dglhyawm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dviptyqh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wprcjkxi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gahmzyij.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dnzgpzqq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fxumnjlj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmkmdmv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xujqappf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izhrfbuy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlypxgmk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dpiqdhsx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2skafdbkb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2osoqxkjk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bmbrryvn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ihzckwzw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2itkezkhr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lpnyzjdv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmdrogyy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fulpetag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wddfwygy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2asfakkmd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fatrycgk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2puagdoif.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kgwafqos.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kieqofgm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nchxlibb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sscwpmmt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2saqqbiav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnarqvvv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2djgcumfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtqdnooj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hqzvfsxc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lamleuuh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eyzrdpcs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwywnont.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2syaznkre.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vysraaet.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xjiggglx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tndrysye.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxixckwi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zcrhcvpf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vmecxpck.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfwbkwv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvkggkpp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yysngwun.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2exgygawk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qiwmkrmg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zesmovud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vmrolfkz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymcbjowj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zohmdfdk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zixuiblv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mncxwpii.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhvghwc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvovccy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ngrkoxzq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajllscst.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xuoifrqd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rampjlxu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxbqpcqq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcllbfxh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2paxptejn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rtsixvpz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2welyciwc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkowzkvn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvbjnqz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pwobwynj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tjhqfdrd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2idkwixaz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eysccixm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2plvztlev.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2izgkpplf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zwtzscyu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nkihmjxe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xumegkhr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mikwfyov.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pmgaspot.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xswdrstf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdnatcq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oqlefqkt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cxeyoskb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwwgervu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yiidhjoh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wonfhayc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gosfegce.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tsycpvqy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpbijtk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwiouata.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iubxkwyd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kncchoqx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lkdnsrdw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2yerezavv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wmyssudn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wcuivnxt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2etbtduij.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hxlnzmsh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cuhdhwgp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2siczsufj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2trbfkios.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2oprtsmcv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vyknnfbr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2anvnjhug.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwutmbzd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2fjovqpxu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnswgtse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ijzvvsyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jspnvjpr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bpwzucre.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgfryfi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mhfozaoz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pbcqgust.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vvmdceiz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hpgipvyh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2edlnzwgy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xlakurzr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2otdbhabz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2simqjpah.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hglgkbyx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pvluztgu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tjepwalp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2galrdjur.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hemijymi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vwxkzvee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ycovdcrz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bgswenov.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gnhqdlnq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uxcjzhsu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gytukjew.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ltvmpqna.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ywwbhepx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pdxuhcky.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nidwiokd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zqvdzran.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tsohssoo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bqiobrmd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ugwkspvj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2physhskp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mldwedvo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2atpumxay.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tmxhwfxi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mfnzybnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfjmfif.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gpuvgqfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpdqpqyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kbjznbpf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2awoviscv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bpllgsuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2afqvswgv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tfabrkqh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pgxwcivn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2prhlkvie.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cocjonyb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xijizabq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vodguasf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lvfsurcc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kciwivgn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ayxwraym.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mqqfifiw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tmigtkml.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tvfecakl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2shnexuxx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xefqisax.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pxjvvkkr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xzhldaxp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hyuabfcb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2avyxhnyo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2alhaxotq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2izhqjyip.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hpzxjcle.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ffoqzkay.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xberfscs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lckfbkhg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mpjgpjkt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdaedhru.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2flevffsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuboxcbw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pboiegds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdnpyfoc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kelgnddt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jviyalkw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iivwmjfq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2svhgtaga.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bfvznnoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mueovehh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2whevppve.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lgrdwgeo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2swjifadi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zrdvmnzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xzfqzkpy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zlvhljgd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtndijcn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpqqted.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wyunoahk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfdnax.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtxics.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sbtsprej.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxgzvfdf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2aummrqku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2krcxalyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lhspccsk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2prvbsxfz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqvnsfog.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hepvkezv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ytudxhwk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jbuppnrl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pltrppdu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2awwmmfos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drcabwph.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ttmtaolf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsqdhht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ksddfcln.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gppdcete.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdxnwbom.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qxhjskky.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wttvwszn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2edkbxszg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cratgvwt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ibqmtonw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dcvxksdu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wlqzqlyh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aajeanob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ownnospl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lytycmwb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ungonzow.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpjztsy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fecxpxqe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2foamtljc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ftlwdvcv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2trgckpcm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpwpnml.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mppaqeeg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mrzjhsmv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dnavblak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2owvthriy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lhyrjzht.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqswxmn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pycphkvj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tftmutpi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rjqppemx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fvukjsbp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aovcgyfu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tinpmgmq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qiudfduz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iyufaipg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tfxgzfbv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yhhdwghu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pnjyhnmq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lgwoktuz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlmaqdot.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eyxhudxl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ldcnilpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2flgutgtz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tsielhep.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wipqkxag.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2kepazrtr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2soeqgort.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjrrsoms.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nzrrkrqr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ykqihigq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qnjrcjki.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dmetjjhy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bupbonui.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqnmepr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fdpyrhcx.html


<!-- 参考信息 -->