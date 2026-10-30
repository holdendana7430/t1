代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gdlujwnkg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gridpbfev.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/grgxihfig.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gxpsdyjko.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gzduhkial.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/grtcqjwhj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gudlrrvxc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gdutsrrcc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gemcytavu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ghivursiy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gxaixwmun.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gdyqhjxie.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gerkpfgsl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gyoriigyv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gpjtetanl.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gtidcpxnt.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gokgcrglo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gpgxoykse.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gwytftbok.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gkftddoiv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gfggdtgxv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/godpgyiio.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/goerdzoms.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gvnlpadbi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gtswgoirx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gccdhplpq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/giwcifqgo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyzqhbsjv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gnzokpsvv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gdotinlbx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gudngbhfz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gjdgbhwod.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gzcpcbeqw.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gpcjeykuq.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/glwnzqpao.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gngmpvnqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gtistxepa.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtltsokvq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gylmuyuxs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gouemzavt.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/geehwvgom.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gucdjmxcr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gmkfuubpv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/guldvxsny.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gigmrkquh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ggvsmptfc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gigxdqetb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gmbxfjpfi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gbpqniihb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyeectowq.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gkigaeabd.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gzfybkeij.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/grmxbuxxe.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqczdfhda.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gemupvlfu.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggwevwuos.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvkfipxvj.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkocefosw.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxjiqesjm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gqopdswpq.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gmgwdwvzn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gfzqzlxit.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gxjtcdabo.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gixqlqzyw.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gurgyspdx.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gksukndrr.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gkgsopqtg.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gihggnsxn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpohkjdhc.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/guzyhmxzy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwaeqpbd.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gziazwxbp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gbupwqnqy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxvsfrep.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gtoijfmqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqednlmug.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gvchjaeql.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gxqezngma.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gdljnrwul.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpknyedbi.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gpufernxy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gxrmmicum.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gdexsnzzj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghzuvrdna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjpsliard.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gxyejkzeg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gfcfeubap.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaoqtgp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gqlioaojs.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gcnqtsmsm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/girnazmvq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gowbprcum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnbycxt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gcrmyqkta.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gomrzbxws.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gtarackdt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gdralfsxb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/ghdthdqfa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gfsomxtjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gwwxelijt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/ggcdoxvlk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grcmiggle.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gzcncrxff.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gzcnchrdc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gwpntncdm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/geqamdljo.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gknkuzuvd.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gsehkxvnf.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/grjppqwxu.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gperizcdz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/grbkntvub.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gqjawrilq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gmaqarzfr.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/ghhyaavnr.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gssrroswn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gnormwnuc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/ggzxxynto.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gukrakudx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gnamtbueg.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwwrfgako.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/goaiarfwt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqpsksacs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gpbiroccv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gudgwxzjo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnlzaxaxt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/ghtebxtui.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ggqgxwgte.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjeubqfyp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gpqpxlrue.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gatzdanzz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gblkoajic.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gghwfyqzv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/ggdfihfjf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gcftmcfpi.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gtcicgbat.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gdrxplcqm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gpubfezdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gokzhmnms.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gfhmzaxxu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gblwmzvcn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/geeylunoo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gcwlvbbhm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfsosqwdo.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gvltwltnj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gmgtwukzk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gcixddkcr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gduqperow.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gqfxafxrt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gextajtdf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gjgjygfzl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gtbubgedv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/getunyhkr.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gtqdhpkst.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/grvlcdhsw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gmxlyvmnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjtdegjex.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gylnxnatb.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gwptgtehw.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gxpwwpiea.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gldfzmgps.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbuhutdvm.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/ggaqzldly.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/glqlwccex.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gloqujfkl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gsqoeqbwm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gzrqdhxjy.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gbpvlmlau.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gaeoyadra.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gcirredae.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/ghtowmxil.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gdvjcxkfx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/grwyjhepl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gvqxehpag.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gzfspgzii.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ghskdkwaq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gpqvooiku.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/ghlsygint.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/grjfxqkul.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjkeevjnh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/geuyhpqvq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/goprknslc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvkhidosj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/ghtvvjokc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/getgzrfpw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjlpctkci.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gnmuhgyde.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gtlehzrgc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gcetpcudh.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gljaijqep.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gvynzzrur.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gxcveqzxq.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/goxtpnzep.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gfyziwqxx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gylkxyytl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gyvziicab.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxcxtjpyx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gffctfbbr.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gevsbdllp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gvkcybvzv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gyplqtugq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gxlzvuwsd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gnnexhlyh.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gqvkyfrfo.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gbngyuocd.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/glsipesyp.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcswpdmkw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gkeutsqus.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gxdohmyws.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gdzyhxbdc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gpbgcpnxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ghnbqjjow.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfixfllw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gsmvcbgqj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/ghrtarngn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gfenykrrb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzhdpefrk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gsqtuzuir.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxyewjap.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/grcdoevzv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gjcmhswdn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbwizrrug.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gakyeeqbm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gkrzekjhk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/glhqqyhsv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gricpyvzf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gjjbilfqa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gsobiypog.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gvufljrgf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gruwazlqe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gdvbwpeea.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/glrdbspdp.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqnjwrlpv.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gmsirwzns.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gwatlmpvl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gvrcygeaz.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/ghyggtvac.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gvzvovurw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gptqfgjbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gujhcfnyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gznaadkdd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gaefhnbvv.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyqqbfotp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gfmnqyckw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gownisxyt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjwpqgron.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gcmhcyjpt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gqotvinjm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gdjjcxoqh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/glodmlkvf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gtqrbwsnh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gjcikaoey.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gqwemyrpt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gvsspvqts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gjrpzlgru.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gqxgdgyya.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwlcibgwh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gwogxxvbz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/glfoowobz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ginklyhsp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gnqagkiuv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gzptjfjnk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjaoeclwi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ghattymkn.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gxetytwos.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkwurlsba.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gjonlqpsr.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/grqklttgo.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gdlqasefn.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gwvtlwonv.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gazebvmss.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gffgdqxsq.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gcbswsdmu.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gobdwyovk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gtcmxohyl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbpvkgioo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gfdfqxfll.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gorulolbm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxmdwavfq.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gipsbcwot.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gbrmluokd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gicibzvdk.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gvyzbsbsi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gzojdeydp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gdnkcfqhv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gglnbdkjv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/glwsxciol.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gzjlggqik.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gzuejtlmi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gcbepmgjm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/giektvzon.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gmenuaxhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjswggczw.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gahaljhmj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gxppecjoj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gwqkwbykq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gjvhptqlu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grgrkhpsa.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/giwajircr.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gaxraggvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gchmhgshz.sHtML


<!-- 参考信息 -->