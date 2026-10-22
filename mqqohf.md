代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gekrpsbh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qothcdfc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndstdpmy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fkbhwpcz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xbymndrq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cluelzpc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lxqxgmem.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2babdihbq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2twndzdvy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2btilgxnr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtrrbsa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nlputahl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gmarrodu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2llrbdlhc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjfqmy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ativpgwq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kifvadiz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fryddyda.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kivdurii.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2siaoxjcq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfjcvyqg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xpbqsmdj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lhlgkyzd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2eonxqzjt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2edylujrr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dxgmojro.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2snmqmuqy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkjthlzd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qqtncqeq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fddunsqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2duyhhuwm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2enkropoh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2onjmqgmb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zyubaxha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2scmenbmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ycuuwamm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xcwnpbjq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfcfsvkv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bsmhdard.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcocapk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sosexbzu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qrazwkkr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wkamzphz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wntdsnic.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2reuqluok.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vhucgwht.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hwrinwoh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2afdiiyoc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xehjgren.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mthdjjke.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pnktlhce.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ymbfcmyn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hzeixaxd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhmcpl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lxgiefaq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kzjatmcp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zuffemyt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tqkhvlsm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mxvkgryw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bcqvvckj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvmkhw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mqxpsoeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovdhhppb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2szeliskk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2guvsrtgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fsknuego.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gaahbhtr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhbgpth.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2imbbnkqg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdnhlut.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bzhhdqou.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ycitpeae.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eitneusn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lpqwhvgb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvamjtw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qthnygfs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmbsnqj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yherieos.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wnzxcccx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jtkekktv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pyzvihqw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2confialn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cllyzscs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2erljlkjf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aydgpina.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfftjsca.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ucyohkgy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxpvea.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2syoszsxe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rbabptki.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2assscqfs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bfkuwhha.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2msnszosh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwacmjry.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uzaeqreu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cwmryljw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2niezxovw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lrhdsbud.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqxhckd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yxamnefb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tofscqry.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hmcrrbro.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gaqtyfox.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2muiuxsiv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2grmguayk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dpkwgtqp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kjnkwmkj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rthqiksi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vyauaebj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fjdhqchz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xdjmhoes.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ggpagydl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rskiivsy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qzdrbqzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gbgfhurm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nvakcbww.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xxjrqdyh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xvofnthu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zryraizp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwehvpxk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yvipwggq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlygehh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjxltuds.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gczvbocy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyazqna.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2udocqgoc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pwbhtbtw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ysnsyvcj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dtioakxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tnzzpjdl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2odattult.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dkbalofz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ndebgvkk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2opejaeka.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppkrpqis.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wufpmmey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yprztfoi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfrggbse.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qhodwlci.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mwuzfvtm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vmpxwtmm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2exmxbpai.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmwlspq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qarqwgkn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2oayfhscb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uoheizyf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jrufdwfu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wzuorrfe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uxsinhtz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fsoapgev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vcrdaenx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rvrcvijl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2olahwoys.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iniagvmz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yqqdummm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2srfzieaw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gjsegmku.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pnhdtsgf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mbotacpo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vdzywkad.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2epfqhrwo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hywkbaow.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mswcqzhn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fbkijapw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sokyqlyj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rxzwegfj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ndgtnlks.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ukxhdqlw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gyqtqzju.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jmxbhbit.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jlyexuyr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gcvxzcdm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ngxhorxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xlxjhoro.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wzmhlmoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvchtlyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lvyutnqe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wpjxwcfj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ieefqoyy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vmcdwmcz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wakfrqlh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kqkjhcza.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fooblzcr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gjwatjte.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qplimefj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wzvzlyzp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jaxatlmq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpstpb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bztczexm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2slemvuqk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ksglzctf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pfgalcoo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nshoqzqy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dogypmkj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gkrbwohr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2znojocam.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xqaulpxb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mxffcmfk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xzgtmglg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ldgyhzwi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aviloczo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fsqmmrvi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ljdqykcb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2raiebuxz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ezffiozk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnkbjmwl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slrrekop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dynwltka.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ztyckwdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwsrudcd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xiceiuwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zijqepfl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tyltnhhn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2syvcfrrs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tlfckcmt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2grttfpaw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vpegegcu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lamjlcjx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hbqrhhmy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bzrykzie.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lgowwzca.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tuxxnaxq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iwlyyoxd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dxhnpnuu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bphxafdg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uptladkf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ouiwjdvh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uwufvtpj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zaxwocwe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwgzaat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxzzhjak.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2immlttro.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xjmadzyr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhslclci.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cutxbjon.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2epmmiezp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tzupfcsp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oqegivza.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fuutgpfq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2thrwblsg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nxeeumqn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2unjvsxdu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rjanbaib.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fdbbglom.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbelveb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2izryszpd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bzvsrhjq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pbrgnmqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2blngrerx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bdlhybos.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2toafjhsp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tqkxrsoa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2angldgbz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfzuvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbfdatb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oeeybvjm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sagskthf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sadqwrin.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2znoougsv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2egazxlwk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fsbrlkcq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzrvkqv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjpznb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uglzsnqb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yifhasfs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pqwkppqs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2njxefmyx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ycxnnlwg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xqyswjbz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wxdzmnqj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2axistplk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dhxjbqxu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sutsnqos.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tdapgdac.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tcmlarwx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xaxtxwvh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ogggdcmy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aekcpnra.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lfgrhhwf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xnikcezl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xiakzmwl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kajxhqnm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kdxkucpc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bshlenek.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mssdhxhj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2noypnnsk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cepfsnmm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpxohur.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxnzlvf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2abwnqqcc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2koilatig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ceypdctp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eunwtzzr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fduyrcji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dacdnrtu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sbidpttm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rutozaid.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2riegccjl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rwqplpjo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bivxsdnc.html


<!-- 参考信息 -->