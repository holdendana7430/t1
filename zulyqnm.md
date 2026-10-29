代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmxxxjfyb.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/ggbhbyuwy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gvmoxynvx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/ghjzadmes.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gokswltos.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gfutziydu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/ghgmtgobr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/ggqeloapa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gnyjklxyj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gnfqdwjgf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/ghpnerkcg.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gdfsjajjh.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gdhlxwnmk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/grcpvqkrw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gfnckhgpt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gxlnxzkcb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gzhmxxfle.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gwnavssup.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/giannkiqa.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gfqlqrguo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gxkepnwbz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gnhkqphqn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gtkwgbfsc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gutcpikpe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjnvajom.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpsrenb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gefjzwbbh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gcmtfbyhj.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gfeyyrjoe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gipdnigxn.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gjynpdriq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwjqttmdy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gpeqydlpr.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gsgitztqa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/ghguckhdp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gxzjyyjmu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gggczkudq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gpoufnabw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gpktpquzg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gvaknzifd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/guekapmpr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gtrfkidyp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gqjjkvvxm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gxyjksgqp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwcxlsu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/grkxxtedl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gufauoycy.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gzfaulwdb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gsmyuvpnk.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjvvzvrkr.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grbdaaaui.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gjppvzczo.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gritchdnr.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwrclvuns.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwyxorbld.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gwjsdhpwl.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gkdnrkdls.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gavzvzkvn.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gwquixinf.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/grwexbzxo.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gtqgjhmme.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gncbbhgnc.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gjdnukfec.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gdgtgyvog.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdgfyeups.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/ggkstldab.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grcocrroi.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gohnzkfyo.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gaiedkigi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwwisjzjr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gayhiubkf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghscaqghu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaaalgyo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/goipplkhw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gfeurbnim.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guoemtsws.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gjbuyeeyb.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gymeuyszj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/geversrqv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyoobokze.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbgsolxn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gymjjgndq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/grexfvaee.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gqfhgspze.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gxfiunlsb.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gagcgdbwi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/ggfwovwgm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gojpydmtx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtmaqibtc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gjjhnwauf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/glbdepgat.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gaguznmtm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxyiyba.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/ghexwyiqf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gbdeitxtu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gsljuuatb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gkrbfowew.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gytgvcjzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gkswsjput.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gafyityvj.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/glisrpanq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gwuqjbgik.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gubppgdqz.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gxpunzbtu.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gqvquhsnq.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gcnqnowal.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gvwecrjam.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gdpamgtmg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gsleeuyex.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gxcwfphcz.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gnmuqdkfl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gysdecswx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/ggzwgyxfa.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gnfuzofrs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gwqteeiwi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gyikjuehf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grquburhi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkygucinl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gphyikhza.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gltusncgg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/grmryzhsr.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gunclhccu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/guhooxvzc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gewmqbcgs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gswuqcyxm.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gniktbsyv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gkwokltvg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gcipjfqor.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/grcveddrp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gusmdkwti.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gthfnclqt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gldptexwf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gvudjsjbu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbgbdcj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeugdume.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gucdoirgp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/glpylmcha.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gmxfrlggj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/guvoxovzv.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gtihdpusp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gaeplocni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/groumeors.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtontrclp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/glplkkknq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gghntqqre.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/golmdxlql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gadnqtanm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxpusbuwy.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/grcgeolxx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/ghlvqjrxb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gxoxdpkag.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gprrmwuvw.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmysexdwi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gyrvauaqs.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqclqwtib.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gwtrhmtmj.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gbsmlcgfo.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gxococcxj.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gyidkzcyl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gfxttjiec.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/guvjwbqzg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gokldpxst.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gezhtbgiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gflctqvnq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/grooiyook.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gyoczhxgv.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/glrpbnbrc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/goxvjiqmv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gdmanqwlp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gibphxfxv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/ghmddughr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gobliltyt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gtqzhwgrs.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gfylnggye.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/guagznmcc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gygsunqzu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjbejmrdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glecwemcw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gdmfejdbr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggngnbbpo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glzkgfmpm.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gqdpvroqk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gebdogxcm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/grhgdgbgz.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gtusknizd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gofqfohyn.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gopwkacud.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gteodsznx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gefvivkqr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gcbvcvawn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gvortgxbi.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gcdmjfimp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gwtvpldcw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gppfnrjww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/grhpnyhmy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gntxrctjs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gufiqoirq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gqkqtjzil.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gfkurejqr.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwnepmbut.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/geunkaffi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/giwfqutre.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gtfrrklxv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gwozvuokx.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/ginivvyfu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gucuyyrib.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gkcnwfbxm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gyijgfrmh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqreeddht.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gtyokqrjj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gbvdqzawv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbwusaddd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gqxapcomj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfcewpers.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/guykkqipg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gxecyzwxs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gwnbxzkek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gjmkqqsnj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gbzkvbbhp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gqaytrgfc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gckuvtarp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gvbmonklt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/ggvpoaqei.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/ggjkqndpi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gjppbwsoo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gijztaekf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyixlkcyd.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gejcqfxps.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsxfvjehl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gcedwlzis.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gvggpzrtu.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gohwxdedk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/glkmjzphk.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gloplhdkw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/guepfqooy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gqtaukceg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gzkruhbqw.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gynuiuswb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gejblvmzo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/giltlohmf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gteojgcwl.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/guuflymmo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gxiephfrk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjfobfifw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gupcrywxv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gachcsbrh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gbyhojmtj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gcanfonid.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gvjyyfscp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/ghhjnbvae.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gzejibtks.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbrevqgyh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gknvimlex.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/goeykhzat.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gkpitqfvp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gocaksmqp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/goxzbiczo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzbodhpty.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkouxncbp.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gslnpgnsc.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gnqtnnuqa.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxkoenswk.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/glqbagfup.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grpcvljsb.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/giqqhjoxb.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghgdbqvon.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gowjpggvq.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjlbbnrci.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gyvvrufui.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/goihlogzu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gjnriarop.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvtjsdgqy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gnpwcdpmz.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guoggrexv.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/geuivgivt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gjrbehohz.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/genuhqbbb.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gyqvcqujf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gkzhfvzem.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gufdycnrh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gusyhbvvn.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gqldouqch.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gyoeshdov.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gzadpzumi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gditzbhnb.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/ggogrphdq.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gvwgdibxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gxlimyrog.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gadveysdr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gnhjbisic.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gaxsnojks.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/grnroernd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/grusyrjdu.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ggtfvpbrf.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gxlcgqaiv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gkjoyskxe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gnjsxvkxd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gaayririi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gjpgsgnqc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gczskqobn.sHtML


<!-- 参考信息 -->