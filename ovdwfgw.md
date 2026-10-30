代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gskdvzwpy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggoskldyc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvpjbhx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gjrgzdtyk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gaenjgkfw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/ginmxzmdg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gzxzqjskn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/ggerwrwjs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gczvisvzp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gdfsroncl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gkdbfdjme.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gnqpwdudf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gzlbkxqrt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/ggbdejopt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gwqwbdgfd.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gcuxyyqvg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnumhwqzj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gcptmwmwa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gbqsuhmol.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gdbxggjuf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/goeifdbyx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gocqajmtt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gkhbnknxp.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/ggehrbtlr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gmokdfwim.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/ggthdiqng.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gsywwflik.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtmshccgx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ghxptqioh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gmhvlylyq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gllwfjvhy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gdypqnrvz.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gscocjzwe.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gyjdlkybo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/guwdnnnxe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gdsvswlya.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gmlmwdkmt.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/ghvyaubed.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gguhazgcx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gucvjqzxp.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/grrfhpijw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gxdnrsxms.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gahdkhmhx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/ggxpefgly.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gkzvrdedt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gastrthjg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gaqboxpzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gockroecg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbvxwqxlx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gwlfyqozq.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gfrvwhomt.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gbhyardkv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/glchhyqqo.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gabstiwuq.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwznktfas.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkyrfessh.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwnlsukhb.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gofzfwens.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxgwivzua.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/ghedayaef.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqesjmb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gqzbwpynp.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gewqszdiw.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggktdjszg.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gtqtyrbpg.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gtkqzafat.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxmnvfl.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gmjltxfhc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guupvnqcy.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gfxolwkut.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gddnlvuov.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnyleqobv.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gxfloybwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkrknussl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtaymrqnb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsmdipdcf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gswehtrab.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gsltsphcd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gkwdeeocs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gncqqljrj.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gkvmoncjk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/geugpkctp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gorkgkigu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdvpkcvxv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gffouliqb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gjtwermfw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gjfxuyagg.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/guffolwqf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gcuxrwjdl.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/goytjsucz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gtywmiczi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gedpyxyjj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjaozfrbq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gnpumruua.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gjvpxvqsq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gdbwepczc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gdhfvrdqb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gheayolvk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gyxwvhpci.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gbloiazco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/giiknfdqp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gbfjufmtu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gnjeaajze.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gxuqlalnf.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gemsybtlc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gamgzkgws.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gscibhhdw.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/goqnbteqs.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gdinorcex.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gpfvwohtw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhrcqhk.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/glqfhbipu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/glbzfavux.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gnzpnibsb.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/grmumjsdh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gjxbwwmgc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gsvtfgfjp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gptgygpal.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gjupihqzb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gqtqmnwpp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gnrccjpzi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/govpbrmup.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gsaeoqxwb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gkoeihpni.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gxzcsfhvt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gcpsjhual.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/guptfnixh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gfnxkrkam.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gophecaco.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gtsnbxtuk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gqyvtpnpe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gnqrulswd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/ghpwlzqnk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gpmudqgdt.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gycqtyuxl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gctaltdkj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gbvzrzdhc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtooxkkxm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfnikpeqt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gkfisdbor.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gkkudghlz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/glcdzqsnv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gmzdwhhno.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gyqxpuxay.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gphtmiqxl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gajrguodp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gobwtjtma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gqzamhbse.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gygdpdqtd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/glwobruug.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gimkbcvnr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gfsllfvty.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrdxywb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gkrrdljee.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gbgjqzctz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gzwjxvruk.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gklzdxtkf.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/ghhzhwsvy.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmjldggjl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gszlajjdu.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghozfqodd.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/grsyqukdx.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/ggjfjjhwe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/ghhnyszlv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/ggciifcgu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gmsexamuf.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gakhcmtpa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gybhzcbfk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/goytgcklf.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gyaexfjuk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gdazpboao.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/ggpotvlij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gkbfwolbn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gjjiqlemi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjiifbcqr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gosezovfg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gkelxctfz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gxtknjghg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gxtoktrou.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gpqgxgdxu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gtzfpgjig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gefvrwqei.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gaapipxzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gzqgnmlyk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gktpgzzrb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gvvduayzl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gfasrohsi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gdkakwhsj.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gasozyrxi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gosignzcq.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/guakpkwom.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gnjcbiydk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrukbafc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gaaxmbxlx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gloeuirdm.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gzdabbdlp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gseohdhlz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gaytrlmtu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/giheuiodd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gnrmhpjaa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/glonbddza.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/goqlojluy.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gtptmrfyx.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gjfmvcvkr.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/ghpvruhmk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gvbawxcqn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gffouiokb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gimmmamfw.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/glvvxzqmc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmptgzelj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gcpuswiie.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ginvgxuqq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gmmalgrqt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gxovrqspz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/ganqznzfc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxdbnvaff.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gvccdxurx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghdramicn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gmwgvlpoh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gbgajtwfu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gepbmfgth.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/grkwfycwz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/ghmpasgyh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gsliezcpe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/ghtgmxexs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gohldagwl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ghtcsznkh.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gjjslrpti.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gqbqikwko.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gzivojiwy.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/glzxfmpqf.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gwljfwhyd.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gtisqddsy.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gvsbuilvi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gzaucecsm.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gmqiyhsaz.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gvvomptyh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gytyokjyt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/grcvcnfln.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gkwftwlut.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfoqrbpqc.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmouqcbgp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gmmkpuzog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gxxfwbwiy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gdjgxgovw.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gxikapmtc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gzhlvkqff.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gexkpjbhv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/grzmvxkyc.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/ghlvfbinz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gjnnpffrb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gjujtlgog.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gxjafmzdz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gcbjrutvx.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gouesrlos.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsxvbsfzj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvvksrogo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ggjxkemqo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gcobmqgnx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gejdlnlvu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjevapujb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gaaukyhgo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gojkokzrv.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/grmsqwfwf.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcnghzguo.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gofukyspg.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ghzvwkljh.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gvrjdwdwb.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/goffmmiha.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/ganuoktzx.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gaekwflum.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gxilvarkc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/guesgkhrl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gcyniwlze.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkeqfivqr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gribyqgvu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghkhdhjay.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gywxvmhds.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gaqtjviiz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtvvyduub.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gsdsqpjyb.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gfhaazgcm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gaeaehqmn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ginsxfinv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gwkvhufzu.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gflggtbww.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/ghttxebxt.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gddiwqlee.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gwmygyugh.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gtjdwcdfu.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/giqffvtdi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gvdohpbls.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gavtbtean.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gwcdwguvs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrgorqaz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gclckrhmo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqqzlcxwu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzxopcbyp.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gkyktkwrt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/guuyspnre.sHtML


<!-- 参考信息 -->