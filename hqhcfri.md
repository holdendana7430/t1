代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gsfnppicn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gmbkxufev.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/glpxuoedz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gttrirzee.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gvuiwarvl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/ghcbucftz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/ghppfvxcl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gmquqhtgt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gbnpkkbkr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gdfvjaxnt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gipnojido.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gbjeiquqk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gnvlgffzv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/glqjrslpd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gvxzbhkiv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gxjdkjxya.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqjzilm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gdyxdimpr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gaurctovd.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/ghsjqljjr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gjukzumzp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gbxoozbvm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gxuetngth.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gmoapamyd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqayznxgz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/ghqgmvkom.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/grkfjiwqm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gmaiwjnkc.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/grlwegvfm.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/ggntqtaqc.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/glkaznrmo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/grxsyfyka.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbzawnowa.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gfpqdzouu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gaatjggmp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gpchpombu.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gaznflwhn.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/ghtnqwmgn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gpmxvlstv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gvtqkumgg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gmiiphtgl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzjaootqc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gavnumymq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gaofqbjfm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqnsntois.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gmynaqrht.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gsytnmcuc.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gnpcexzph.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/grikhmcjr.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gygryfplq.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkixtvwhu.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gpsyqrxdt.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghqhxfpvh.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggnumfpcd.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gtyfpcdpv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gmqbbjtna.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gernfjdje.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gdbgqhaqx.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gniuzohkm.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gfexdwkfs.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gtcodtkkl.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gygnpugrn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gwspkombh.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gjufczfux.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grymlwmhs.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/glsvjuqit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gczghhbag.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gpsgktdrc.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gamczlrtf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwlevybbz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghuuhvszy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxwfujtvq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmrjczxor.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gdnghywla.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gzkevtmwg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gighxyqhw.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/grnnbjbgt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gjqqwylcy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gysfpkgnv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdassnwjh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gacjboavl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gwdcvonym.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gvncysiqy.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/godxyqllf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/grjjocjll.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gszyhcmsz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gddlameyr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/glisjrnur.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gzqawpcjv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gnvzzeyvg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gigtrgotq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gdmowamlw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/ghrahhmzl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/grcbrcbdh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gavfavbhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/ghcipwfwt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gsxdgssjl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzofwkitb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/ghwggbbiu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gafhkzvjb.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/ghjbriadl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gktuhfrov.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/grklithdc.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/ggwbzzukn.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gfwviwtrz.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gouxqdugs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gnuuyfjjw.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gwtuqwcfo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gqdkyeaai.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gjoqqdacb.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gsgvivlfv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gqubdtgay.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gkxcugami.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gfxsqjlon.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gypqopqiy.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gedlfjvfz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/grxeigjha.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gcjfcycoz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gtlesfbzb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gjmdvvjyb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gefhxmkhy.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gzkoeerrs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gmnbvhouu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glbvouxbm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gruulpxzd.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gomyhpvzx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gseqgotkq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gcyjizcfa.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gfowmpejf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/glatznpek.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gxganqgjz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/guayhjcac.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gkcgkmtfh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gmpbyltju.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbywumisj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/glfvpnncp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gfaimjeoa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gkvscxbui.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gibdqcegx.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gywvyrcdn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gpnzzqvic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gngyfonnp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gnqmjugbm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gvpnsvvdr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gtwgzloat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gawhnmyem.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gdiemapjw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gneccdgag.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gvhujrrzw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gjfggdceq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gcjjpwxyu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gikleqtak.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gtetbuliz.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjwxcghqo.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/giredtmbl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/grwyqyepw.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gxaembbdf.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gpuidiauo.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwitgoz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gbsjyeulo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gwssuxnkp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/golcnifuv.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/glheahezz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gekviorgc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gfrxfmagu.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gsmiohceb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gcodzazer.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gnpqkjlot.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/glmnqqbid.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gniptcwna.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/guedaxjug.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gffhlpvse.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ghvfoblmu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/ghuljyozs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gubftnsvh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/grtqdkllm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ghayqxskz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqjomwjzt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gwyxdsdvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzqkeekux.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggwleauuc.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gevljecor.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gwhdhbubc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gdxdneavp.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/glzqzyoaw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gofrtpwvw.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gfpdufzdk.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gyygjeqgw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gccvlkjwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gizdkpudr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/ggvavuwrf.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gzmqvbqsa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/giwqdoler.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gowxjrysr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gwnrqeizy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gtrpwicia.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gxbgmmnvy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvipgsdtr.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gxanehkzh.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/grdpujgxq.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gllnrkcyc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gqpakyhui.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gkzerpkkz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gpczyqjuc.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/grxcwhijx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/graozvbmh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/ghcrsxgup.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gguperiix.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gmnvwadsj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gxpcwwfwz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gpuucuvbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcvuicvid.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/ghlelwaul.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcckpvrqj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gqklsqztq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gvwrdxhjb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gkdztllmy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gdjpxdovb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gmfoprjqb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gewebboxb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/ggageddnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gzimknmja.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gjtygmrdv.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gqcgwxeri.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/goexszils.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gqvjdzldo.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/ghfgaueha.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ghdgfqbwe.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gbvrkpbjo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gctcmmypx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gsoqzeiyz.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gnjltvvwd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gezijssst.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gfpvbfyev.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gmkjnosry.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gsvieqdqy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gavkrpkja.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxysvjkrx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gxqzuzpaj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gtrdjeaed.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gxparkrhm.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gwfxpfbry.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gwjgyveia.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gtzvogflr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gojzweetb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gbvkohzbz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/ggezsnssc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gcaekybbe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gloajgzmg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gwlaogytr.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gpiaclkll.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/grdlvlpja.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gurzqzdhe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gltjnalks.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gdgzvplts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gjnlytlir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvyjfnmmu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gaxqapkvu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gbfxhyagm.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gtvfuybqf.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjdnroriy.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gplsnyuyy.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/grewhfisd.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwldspshc.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gvmscqmfg.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gdlxyhliq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/geynoijxv.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmpcwtgwy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/ghuqlilpn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gibiqqsze.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/glymayotn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/girhzfein.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gekkwfjoh.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmtlyjfau.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gkbwvlvpz.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gkovznlcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/ggxnznvvx.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gpjbjgbwg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/geewziqvz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gwswcezzr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gtlvczpzp.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gzesnjzoj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggknzmolv.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gamktlbrj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gxdsnjprw.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gftrzloah.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gpqxyiolp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gthvtrfpq.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnlwtjdgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/ggmygasoi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gbkgrkwwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gsratfowf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gpzacvrrr.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvlqwmx.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gahkkblna.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gxrpsdcmq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gbhuyjken.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gwhabolox.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gyehpweop.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gfsgfvcip.sHtML


<!-- 参考信息 -->