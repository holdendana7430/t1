代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gpuohtglw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gomhutles.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gqwtsnbvl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkronvjwy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gksiyrsub.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/geymjvhrq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gkstkhlkm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gdhfufiwq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/ghcmfryaa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/guagbuzzr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gpftiwwut.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gicwjvspj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/goznnywiw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gsjsmktyb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gmjzbfrer.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gnlvgzjax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/glezxiqly.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gughecytc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gloxfdmcf.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/ghwfgxnho.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gihiunnco.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/ggzvxcfiq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gswkshzqv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gzngnpztn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gpwtnjfcr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gwuusqaxr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gtnojassr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gggfhbqez.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gucotfbwi.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gaqbwgsrl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gtmkfxlcv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grsrjfdsp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gcbqaokym.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gbgrhcsfo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gapoownja.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/ggaiipnnw.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/grvhfpxki.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gzkfydywk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gcmzjbmaz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gmwyjfiio.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gmtvvgukc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gnhjlqvuk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkdocphsx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gesvevodx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gowiigxuo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/grzfraeor.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gzggyioni.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gqziljnzw.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gjefqdbap.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/grypxjquo.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfyuvexvd.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/ggdanklbu.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gslzuemyg.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnsfmpuxq.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvpuxhxgr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/ggxnduwbs.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gmpeiptrs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gwrssivqn.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/guphjladk.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gtfuuevxj.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ghecdqebu.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gmagwpkzg.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/ginhtqlvr.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gklzdgcti.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gejizmunp.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gkkttrycp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpmubzghp.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpxsblenj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gkiuresai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gzwklltlu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtplcavxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glnhggxue.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtglgtfxc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gfdaiunxr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gkllygnrb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/groptgpcf.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/giyzelwgl.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gwvhkdrgq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/glfnbhjsp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gusqvzdpe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gvfqjgujg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gnftxaycn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/glefemjwk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gixgrnoat.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gpjjnurkh.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/giagccfeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/ghktodsts.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gmuihzjgl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gmvknadzp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gqqhijarr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gftamksdj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gcngsgjmd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gkktikdaz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/ggdukofzm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gmzdecspi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gvfzxugoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gtvkgufqb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/glyqpivjf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gdsxdncge.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gkyfbowpp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gvrvdtyrc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gjsssbvxi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxizahu.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gdnhcingu.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/galwlqexq.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gzjzutyjh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gbefztufc.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gctlnselg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gpsjbosrt.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gczqwlhzc.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gzdxyhyxp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gvwzvacum.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gkzirksxr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gyotlrifp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gpkyitgpc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/grsakfyud.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gztxrpedi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/giafwfvta.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gxjeotvve.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gaarydceh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/guulcjsjs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gicqvvdaa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/guxnprcko.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gnidknfda.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/goeologkr.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/glrwcanrs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gdlvftowm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gxlwnqqvb.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gspjmwrse.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/grubabjqb.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gepdprdgj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gjdmxcsti.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/groelxbgo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gqfczzgim.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gwtcpthqe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gsmjkrfhk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbzgett.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gokjxtted.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gfxzevmpj.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gwyeczkms.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gttscgeqy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ggvwevofy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gskfdiqvy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gbtspakvp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gjfknfras.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gokwijmmw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gqzlqcfnn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gzdljzxxw.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gbhaosdic.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gjqjwumkn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gdzjfoiyh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/grfaypqiv.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gmbybucsc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gkjfvqslj.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqxjpywfe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/grvbrwaor.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwqlkqiri.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/guqtpwgph.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gguevqfae.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/ggqvbjuqy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gflgbzypl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gffpbtcex.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/ghnkdzrbt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gkmnmgaet.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/guolfoeps.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gxpoeswbk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gssaruodd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gvqwtkzdq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gaqckqrhf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gjscfggas.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gcsjfkwql.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gcdkdefen.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gixiopsxf.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gwutqlisp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gitlvarcc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/grrglvfbq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gohryeoau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gndjupvrd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gwlhyopny.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gisykqiuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzmlmutyt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gcbqabsxz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gksmwyqxs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gwxsekkbu.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmqljqxuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gxfnosoav.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvzacagtv.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/ghnwpngxl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gwlqvrudv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gqvhqrmqa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/galfzsgya.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gfegxqygr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gdbyrvxlm.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gijsnpgja.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/ghnvaffpo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/ghdhmjzcl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gostiylzj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpiarppbq.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gmtkqkmcy.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/glbktmdwc.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gqdmzfikb.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gaxromsxg.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gfxlvbczo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gcnweiqcl.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/grezmowsn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/guuaqwcag.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/ggntsphpp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gwugwptyn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gbzkyakfy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gfpuxetec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/glwrpahtz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giujyhtyw.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gcodwjqza.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdkdesfli.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gstdukeeo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gxoaglpeg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gclbgfmxu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gctcnzvkh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gwzmdzsbp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gcqvgmqld.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ghuhkenax.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gxxntqzjk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gdwygdkly.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gitpewiut.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gqsdzottd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gfvxpevbp.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gtrkxyrbb.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gyyhqhjvm.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/geejglqto.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gbkbnrzbe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gcablfwyr.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gavibhjjs.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/glapjesur.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghqdwafym.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gjqmielsy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/ggmjaiqhy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjdkwlo.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmmosjlql.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gkdpdxgab.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gpxgrzcec.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpaxvobdn.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gxtagznjl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/glzigeuem.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gwrrknibn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/glngarzjk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gveairjjg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/ghewchzrs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gexzouvoq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gcwwnqsda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gjejrpvlc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gubdebqsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gajctgdng.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gcqpflbed.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gsipllfuf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/ghucqrrmz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gjkprttax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/glfhopsxw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcwjzxkcr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/giymzkfmb.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghgottrxb.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gcpcacnrd.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnnaqteee.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gvcxiosch.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gappojtma.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gjthilgqm.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaovjizoc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gcztflxny.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gucxbfwkh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyicpbd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gtobegisj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gywemrwsl.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gvpvcohqh.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/grqwvtzrl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gkdnalusk.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gxeksqnwe.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/guwzhqkiz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/goaxoysru.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/grjnzyvqf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gvmrdjzvu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gfesdrqny.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gtgtyadti.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gkjukngby.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gbukxpmli.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gmfbyloej.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gihqpxpro.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/guzlecyjy.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gsqktsajn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gfxizknju.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfeclrvlz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gbicjcydi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gnttacuyu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdzmaakxw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbarnxpmv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/glixppnti.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gcecoulad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gnygshltp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gbpbwwmht.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gqsijpjwb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gfxpjejdw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gxdpjzmkn.sHtML


<!-- 参考信息 -->