代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gpbgytkcm.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/glneyaack.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gziaoteqt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gvekutorv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gepgrmopn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gthfdjnrr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gxqnzkrdv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gpefyiqqz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gwsdehszl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gpweocamc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gxveiqdef.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gumnrjcxf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzynvajd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gaoeaykmx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/grbqhwuhd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggoznaamp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gloyedufa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gzyqaqiid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxugnztua.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gjaawntft.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gqlsvmcnm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gkstwfodi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/ghfdqjlkj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gaiblxcex.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/grrscnxrq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/glucxltjd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gdkaugqfo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/ghefoazjw.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gftnkptdv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gssrlbluu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gdcruyzij.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gkjuvykyd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gjpiajtss.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gdtfwxbfm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gxdrhgfdi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gzmeaudxh.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gdymdcedn.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gijvtylem.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gyjdjmotc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/glmetguig.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gidqdpbhr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gmgoiqqek.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gemcixcpo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gkasrhgnl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gfgtasicf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gusuxskpj.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gjozkrbko.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gdzykvwjv.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gnyuljfgi.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdkjaxrut.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpckybsxj.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqqzsfnnk.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gursbdifv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gncjhchzi.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvgspaiyq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gzcpbbotf.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/grtepxsay.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/ganqldmmd.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gsjhdakva.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ggzhkyghd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/glfkxlqzs.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/ghwxlsqna.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gjhnsznwc.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gluqkmfpg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnjkyqady.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gwdcvafgh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymqkylpx.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmhmdvzmw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gsccgbllf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkjmjmfcf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmzhgchgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfjvksuzi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsqvetji.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gkdkfujoe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gmepeqrmb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gpodauekm.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/glunrypym.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/growaevoq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gphubakxj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfxtpsvaz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/geketcmrp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gluiumosn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gcuxvaeeu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gsjvqzamu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gzgflvxqh.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gbjpkqxek.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gokowgcky.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gkxrgyrix.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/glawprsvd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gdmpbpyvz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/guevnnxwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gznwbxalw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gptbdpxog.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/guqmdivdf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/galbiumvw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gnvwlfjav.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gvdupujsh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/ggmbhzeqv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/glyhmapph.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gaqaiugeu.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gtgsqgjtt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gxoavvtwi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gyoeqyfci.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gtuvrtccp.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/guivsmlbv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gdfjbbevf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxhudgnys.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gxaqinenx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gmnykntzn.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gymploynm.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gywonzpya.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gqvkhtgsp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gnfjfeawo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gecuayxcd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gqlknkcms.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gppjspaao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmltwehaj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gcflmbytq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gvoxigkqm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbrnpadi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grlwlqnym.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gelrpswgo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gvstadgua.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/glyzxdlnk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gxondjstt.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gapkzpcgp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggalslzdk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gewtrhlim.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/ghbjhayii.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gklzxaayt.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gothrjwko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gdnjbsypt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/glrinquwt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gzeizhsay.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/govnrlmjj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/ggxourusw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gwtyzlked.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gtfkmnnvt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggnxzucle.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gcfnezsaf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ghrnekeoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gppmordgt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gmikmhtsa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/glcahctzd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gmprnvone.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gfethcufo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glfyemcco.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gawhwgeaa.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/ggwpizaow.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gpsodbfpx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gtnlonvxh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gjqozahnh.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gxluwsykv.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gqpjhrxst.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gdqdlpvrv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gksosbskt.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/ggeubslzy.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gvnfulkny.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gqbtkxape.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gkkecyihy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/ggazzytdk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gcnggvubu.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gdznuxonm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gmybffqmr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gigmqrixt.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gwdxgamdn.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/giyfazynq.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gqquijhqy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gdohphbsn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gdjshfaiu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpqbhifht.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gfivgkmok.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gibnivqxv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/grlagdppw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gajzumefm.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gffymtunx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gvoxbdzji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gunregjqd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwnecct.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtpmbjfof.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxzxicagg.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gpslghass.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gkrxxtwbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjqyztt.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gaohoueul.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gnozbgzuo.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnsocxuzh.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gdobuzicq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/geaymoeso.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gzaukuxiv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gwlcegufq.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gziigykrd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gklxttvsw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/glzushnwi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gxbevgywp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gzbudaqsv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gbfzrvrtt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gqjordwef.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gpulfyfkz.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gxeqtupti.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gnbdrzlxb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gfzhwvdvn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/ggxybrchj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gscoggddt.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/guyffkcqz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/ggnsutywc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gxoagaudc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gajwkocuv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/ghwpnpjfc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gcnzsyhhy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gadzjbqfr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gokmroosl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/ghsuwzmid.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawgvwcbq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gnfysytdi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gvlziymrj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/glmtldaxj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gpfvzrkkd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gidyriins.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/guzypymmd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/ggzglpdjv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gyvnagqpn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gvoqjrlpg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gkmecftnt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gpfxbmgdm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gokmuqfrc.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gngnuakjl.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/geeqalrvt.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gedixnydj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/geasqoqub.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gbjmpbdqj.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gdwgwllsb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gihaedtfv.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/guhrkxwfx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gwqdehmhi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gyqrsjgot.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggewjdawq.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gakxtvcri.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gemquhvas.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gxpwbfovg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxyjhvcjc.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gxojmvwwk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gokfqvfoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjsgcjizq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gnzsjglzt.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gdhjybctd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gsspfqibf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gqfvqgzuq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/glhuzbpso.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gskzxndop.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gnkmeotwf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsxogcoxq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsgbddodb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gsojxozmf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/grqmkonnv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gzdwhkzdy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gikwshydd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grquasnzc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/getdhnsca.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/guguzzudx.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gytvrrahw.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/givqchclo.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gegqjefja.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gdpfqrvhc.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gbvftohft.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gewuyfwur.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gcqwjporj.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/geihdqlky.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gvzxkqlxs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gkmlzqklb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gwzemtbph.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gqhcipqzf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghxykgsrf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gziljclxk.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gntsjubrg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gonqqriym.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gvgfrpwre.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gcuppotrf.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gbvsjilts.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gmsuotnpj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/ggujmuroj.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gzixioykk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gbyhficzh.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjqwqeryj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gbjcoddgr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gahpbmzjt.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gnbvhcsql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghlaozppx.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/grhaijfjs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gpygmxrxu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/girsejdpl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gntqmsfai.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtuqniwts.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/giolhuwvx.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/grxijmfit.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gbzrwktyd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gdnltczwz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnvuzinvt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gmxtwthnh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gvfcjuudb.sHtML


<!-- 参考信息 -->