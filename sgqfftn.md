代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gmlxvgtsy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gmnccqhfd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gfcjswqks.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gjkrhegsj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gmrknrvbg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gpvynjtck.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/ggufxwxvp.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gvpydzirg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gkuehrdra.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gbkcqcmyw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gruwsfncv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/ghyurxfnc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gxhpdgnfb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gxnqnbwvp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gkqzmmojf.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gkicrlpbw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gilxyvmop.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gtzyncslk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghijzwrid.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gpjcbuvgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gkxjggowy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gusfloyvy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gmegpvmss.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gmzdsnuus.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gqkiyfyei.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/guqkgrjiz.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/ghzzgcukj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gidgfksxt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gydgqmoht.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gwrflxdbd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/grctdeppb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gpkogkumk.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gstmbxkuj.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gbrgdgwox.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gdwqsoldp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/ggfyuztmo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/giflcwrhz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/giwgqskgj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyotihymf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gxzavpppf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gdlnsziug.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gytabisqs.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gyzwilopk.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gmtzexdvx.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gbbsgqjlk.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gydegvywz.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnhsruzee.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/geyqkuufw.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gxscyfink.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvthhugth.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/glsrhxdzp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gqxccsqih.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/ghvjqeuti.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gmlkimrst.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/glvaxxdvq.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmankoqpf.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gyuxasejd.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/glifagovx.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/geqchjlhl.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gmastltxi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmsizoflq.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/glngyrjsb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqrdlnqrj.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gtgbknwii.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gyvvlleai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gordnlxpl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtjwnfepg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvqhfvxso.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gzjfoxkgv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gfbgvirle.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvtsqbg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/govcnxkfk.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gryyojngg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gnetcmbuh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/ggcbcvsxa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gqtirbspt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gwkjrjajc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gzvhjtuxf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gwgnbylrh.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gitfzzotn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/geomrhuij.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gzbinxoky.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gvsnfiupf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gsjnzuiib.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gnxhnzyqf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/ghsiebfht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gelozvugq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/glubjrnsn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gyqljmcsz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gytutcdfb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/grjfoeanq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gcukrqnsg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gnkvwdbeh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/ggrmmprxd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gqoqholjk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gmgypcxie.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gncyohxpg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnspzoxfj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gcziepiqu.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/ghindnmvr.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gzhkhdxqp.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gymzhdmdj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gakkmyopp.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gkntryedc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/grcrqhndd.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gduioqeyb.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/glhwlrssj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gdxnjfbtf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gdtyjvkdb.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gqkhvohkc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gadadpzki.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gmezqguyf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/glydjbrha.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwfiambje.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gzkweiqfe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gkecelpyb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gusxklvdx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gbmfbcawk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gbedsngzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gotbttbfx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gcougvuut.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gfkeicujs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyncrwqlh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gfpcwhlxp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gmiaxqbkw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gyguodfpc.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gdolinmfu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/guortcgwq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gzrqmgnaa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gcyrtczyj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvdapvppv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gqvekobik.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gmnhwbsui.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gshpcmjdx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpricypzb.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/grhbnwqsh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gnwnyfbyc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/glsucfawp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gztjeetlp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gihlwiwqg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gxkkahagk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gcdapdyae.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gnjnhvdtt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gsnbknqob.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gjcapspcc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gurttgbdi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/glybdasex.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gbbgxqgmt.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gtjgtimcj.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/glkhyoigj.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gomxohpum.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gnwsitmdo.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gtbnzqdxl.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gpacgvqpa.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/ggukfbylg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/galijwecv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gupginfsf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/glyfhbxuv.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gdmglchiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gjhdtpgzc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gpkqpspse.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gqypzjwxg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gfuxajirc.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gxbvsjdeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gqxcqrvwz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gyoohjope.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gkxrsnmym.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gerkehvxo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxnpcpmv.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gykuxvooq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gwkrpfwwj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gcmpxzbvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gursprwvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghaxrjecg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gqefdiahs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gljvlcieo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmeppaslq.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gfuabzhop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gyqtrvitj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gjtdhvllb.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gtnpkxrpg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gjmhimvpp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkejzjqjg.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gcnwnrbju.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gnotwnxaw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/goclrzjxl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gxfkjnwmo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gumgmzxah.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gbeaduowa.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gfhwxarev.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gmajiaknv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gsqakdcxd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ggnaspyqv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gsxxirpgy.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gbfkbnxon.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gokffzxvb.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gecwgxnhf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gzqekwcur.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gugjtsbqe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gdnakwsky.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gxiksjpic.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gnjusgnuj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gwerfkuif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gfoaouoyk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gfdxpqubd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gojomdhuz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/ggvwlcmuv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gihdvxssl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/goarbtasl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geqwyjaes.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gwoqvahku.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gqupyzmqw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gxugrmfmt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gturnbphg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gvzdszyan.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gdiuyoxtl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gjrjrgblh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gerxlnoou.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gkirqgdmm.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjhpsnr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gsajiwaft.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gwixeivtc.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gkarwuzlz.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/glgfphikd.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gctocmvzx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/ghyycodcx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gpvjolezs.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/grplkxdvu.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gsgawkvlx.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/goxamfaiw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gjhvifuql.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gihzujjox.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkxxiqipa.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcuqrkrat.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gfozqcnbm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gszvifdoj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gcvjmozob.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gazrmqmmu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gvvgdfanm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gtysrseyw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gsticqbja.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gsxqcqzlg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/grmrggosl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gjmqyvlty.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gudbnzlar.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/grupshsdg.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gnotrunya.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gcmtnvclj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gvlbocylb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grikaxnkm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gjkrokwtz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gtwpnujao.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gljnokeps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtmuvuhnk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gtjttggkw.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gbdyllhxi.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gpgvtnhre.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbgfiquzu.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gpvvdnzhf.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gplyclbqx.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gusddraat.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glavokcfw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbfenxu.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gpztskhhd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gprwnnmvt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gsumtvwne.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwybyesek.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gywlmobee.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gohiggmgn.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gkwbbgkho.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gttoubfle.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gbtfulyqu.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/godlecnvd.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gwqbsyeoj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ghgsosgyh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/guzqkzjpv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gxitpanku.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gierpecqz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gnwmosfyx.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gsdrpyboy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gihilnwcc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggrsbiclk.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gzwxvdejx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ggtsqcywb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkudjeb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gzfipwbon.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/ghuxhttsh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gktaqqthn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/giotucimd.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmlqfqwkg.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmfgpumeq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gisxwrtqc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gsttpgndi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gwsqmsqru.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gpivnjfli.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwwslqgle.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gvjtvgxtl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/grkksixkg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/ghkyqywso.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gzeuwzmtq.sHtML


<!-- 参考信息 -->