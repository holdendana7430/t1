代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giewrjdwd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gpqtyttlz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gwaxjjyaf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gnrtoxfqk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gmcizjmey.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gbynheqmp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gqyzfozpc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gdeungrtp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gnkuikiqa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gwtkmwyas.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gkomynrxn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/grflhofjr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gylluryld.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gjhvzqlwd.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gozajgtfa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gamvhqume.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gvrosqcds.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gzsrlojkw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/goobgfidm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gtnfmvrrn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gbnhjlwok.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gxsqjjtxp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gmnxakrwt.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/guymqqjgq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gjjzjrkpe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gpwvaltgh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gqwoqdyrv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gshqxkbux.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gczmexgau.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/glvgtostt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gjeioskha.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/glgofjaxo.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/ghaarpgda.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gijywbene.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gkutmoatg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwpzipqal.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gtstiswyf.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gmjoqtdnv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gyucemsoj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/ghbaqjqyo.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/glnljhjfh.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/geewfjbyb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gykjtsuwc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ggxxvukrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gckxjjzuc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grpyvpacf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gziyoshuu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gkecxcdsa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gwityltyp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gelewfssg.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gerulduph.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gjmhfixzj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gvkeazlhl.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqrfwdnbf.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtvhpvosn.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gutmbaldm.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqbdotyae.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxidecmgt.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/grbvcwpkl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gnaxpvbkg.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gadizdinx.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gxziwvtdw.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcxyqqpwc.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxuycbygw.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gdzhmnvhf.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gcjancdsj.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gcutrsnpu.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gdtatxbbx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfrgzkowd.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gvvpbgrao.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujidzhdp.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghgldshio.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gjvkvdsrj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gloccdzsz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnmotarkk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggfueycyu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/geiwcsatr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gcufjibag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gojgoffuy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/govcswxoj.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gtjdpviir.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gakjoztqw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwtspyzi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gsiztxlbz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gngdgxzzq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gkjuliajh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gyxliouvv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/ggbsscylx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/goecmsebx.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/govhlnopy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gecwmhiay.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gzxaovynx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gqsddippb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gepilgnfa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gftmjcmjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/ghmsyexzx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/ghaylkzjc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gyvwbcawg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gqcsessgr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gmtnawlrp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gcucyrxzc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gwskvbtey.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gdnaezoue.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/ghfdqepqo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/goiqyjjiu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/grfrewqzi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwbplvhfz.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gsxidbydv.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gmfbcguuu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gznpflthc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ghjfefrvv.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/grumexryf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gbviyalgw.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gcbenezde.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/goxkyighu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gcivreelb.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gjwtvrlea.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gelxqadyx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/ghvhqzybj.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gclwnsuxe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gfldulzvd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gwggeflnn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gcbtngxzn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gzfbpagtj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvgmipnof.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/guoxffujy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gwzjiqidi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ghvdvnhrc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gnddxmcpp.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gqqrsztqx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gvhssvalo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gztgzfdxx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gmfotpivo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gdirihxgu.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gcnfrfffe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gtnkxagzy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gftxvkilo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gmvrdypuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gosubapws.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gjtatmmna.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gvltnvxbo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gwvuayeud.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gswtiigkh.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/grhbspccj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gfpceyrhq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gshbucgct.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gbknxsrck.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gorrqoxvd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gcwcpjvqh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gvzkutobu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gictclisb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gygnvkfum.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gjobpxjuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/goqtxzvld.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gflyrgvls.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gjaozecjw.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpgbobmyd.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjcizuvqb.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gvqgaayrn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gweyxsapl.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gbcrwvgxi.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gyjdzvjzs.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfdfigmwa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gfwmjbwvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gjxkfbaex.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gijulnhgi.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gtwbtuayv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gcmxglubu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gkbjcdrhu.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gdfbhnffs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/ghfmmkgsu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/guptmagdh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/ggesvxdhl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxtcrgnwm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gsenjehsk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gfcdwhsyw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gmgskursz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gxjyqdcbh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzxtwawsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gjlobpiss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gfblzovfa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gpxkzdbfk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gwnijpyzx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxrsmxsdd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gioytuavl.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/ghtipceis.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gznehbouw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ggtqydpwh.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gvyalfnee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gwraywezi.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gezeidccc.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gllrthcjf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gajltlbbr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gqohmqusy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gyhcjyccv.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gnlstkcoo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gbcstwbhz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/grvrujfkn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gbhhmgbre.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkoesos.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gapwiczuq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gwbmvvehc.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gaiawqwqw.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gbkaeuobr.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gqwlneizz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gxbjypmgp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gcahoofxn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/ghyuylasn.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gmdtvrfce.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/glwjkdffw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gaoyuobck.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gqzcjsowh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gacrzkira.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gqehashtd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gaklgholx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghwfojexj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/geznowjwb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmspcndxl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnkvejobb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/girdbhdjv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqelntfef.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gswifzoap.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/glhhiasoz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gsdvlivdw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/glabncrdl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gmgqxyukw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gjwockazu.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gqnbxsobf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/glepihmcz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gvwwbldop.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gguygaavj.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gpsjwslvc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/grkouiwdf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/glhgnixmk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gcrujyaoz.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/giklxvzhe.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gyaviycii.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gogoljpha.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gsxeoivlh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gfxafivrj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxdsyoish.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gbwcmolye.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gtxbfbziw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gmyucghjl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghhvnucmn.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gbzdbileh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gttokcazl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/guwdfnaik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gikmyxkmm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gcneeandz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkytddaso.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/glpubattl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/godrydiii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gqdhtktxz.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gyekwjmlz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gscgmwpyz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqvjdlwqq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gczeosgce.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/geqplcnwa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/glxcohnxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guxyyimgz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gqscswfqp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gzcewzmph.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmbmddjuw.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfquxkvsf.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gvssohexs.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ghgllwatb.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/geayfkndl.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ghqdwfizx.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gfxfyncva.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/giksnewep.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/guqhymhct.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gtxkamlam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gpkyihuxk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gizpgrmmw.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtxabnmxl.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gummealbp.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gvnxmyzcp.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gowbjoptr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/goabrzmby.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gujsoghxw.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gamksnxbu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gaxluegmz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gclygtxyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/glcgxsrsm.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/ggujqafwn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdvnbrmbr.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmynrvqfj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gkugeyewi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqgoxomrd.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/ggwrxadah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gpyfadgse.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsbnuuhzr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/guyqbkeho.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/givkhuxsb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gqubybowu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/goahmjuzw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gjzcifqdv.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gcleoscqc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gcohpbxis.sHtML


<!-- 参考信息 -->