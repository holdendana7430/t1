代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gypuhhwip.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gcoubbqkp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gwdamnrqu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gfczesqxj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gkrvgfdbv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gxjexnreu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gvcldusxk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gicwldixr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/glzovtklr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/glzzqregg.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gpelnhdpp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gmmuwpmix.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gkzhsnuub.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gpamkewgv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gulhuhjnw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gmrfinuqk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gycnyxhkz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/guyvxaiwl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/ggfwtjwqi.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/glcrvfrgd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gxzlujdky.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/ghzsmmfdh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/ggbrqnbmf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gayiuvfwa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gosjpwknq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/grehvewpf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/grfwboxdi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gqpevkkps.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gygxhlnpf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gauvakspm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcxmxrl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gozuyktqf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ggbkqyyep.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gtoaxusfu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gbgwmuopx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gekuvcdlx.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/glonmyjdc.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gzyhparpl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gdxocfrjo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcogqbyu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gytmfmvck.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdjzjycnm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gngpvhiim.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gqcynydgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gsmykdmcj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggmrmnxnr.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gzmbqugtp.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/grsxhqohg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gggvemcft.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvhurzjec.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwpvkrwjz.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkjouegzo.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbkhthewt.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbwzsieob.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gmpheuykq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gqvdgphia.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gelooqvmm.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/guqfztnbx.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gwyprbsle.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gtjxewuyr.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gvdorlkwc.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/ghxxcyzvu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gzbrqvpse.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gsvmashhw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpvjehwzq.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gprygiyjc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnmpztxda.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gapwmbrfu.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gibpyasda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glwqctjcl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/giquvjhkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guxsmvtss.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqwciyoxl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjjoieq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gpnjawhty.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggnvazura.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gdbsspume.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gmplrhkhb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gzhjapbza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghsdgmmjt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gyurptehl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gfrlhmbyx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gyjiveupi.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gxwkxaiet.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjuzvfsk.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsvxcpbuc.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gwkttpuvn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gukokgzmi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/grqwhxrnp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtwkmhnjx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gmekvkgqq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gejpwstor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gpyqvaecb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/glcixienu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gyqlrnrtq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/glwlqddas.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/ggeycbzju.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvlsuebhk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gfgysjoyu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gizjtdahj.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gdstldzds.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gebasgtlv.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gtloclvfa.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gqgvkkvth.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gnvheruuu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gfmmsfhek.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gfylybzke.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gkzxgjrpv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gyodzhcqk.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/grmnmsype.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gwovexled.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gjlnbkaen.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/godbuhvlj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gsixrnffz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gegqknbfg.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/ggcfncaiq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gywogowff.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gnnmrryds.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gpzsmytjb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gvhhuvrcz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmdsdinxt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gjguekwah.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gsrwegeps.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmbfkpcxk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gnofdbrmf.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gxxzqxdha.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/ggbddodsq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/glufyepii.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gnccgdvsg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gxrxigljp.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gzemrlera.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gxucznmlj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gcfpfafov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gvggqvupy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdychvdse.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gppdbgcgv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gsjvtfyer.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gypobfguy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gtanbhzsv.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gyuezmgja.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gzerjxmwx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ggnzihufj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gwwtjujnn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gawkbslny.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfoqakqrq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/ggcsvrzit.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gzdfzbata.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/goeirtivf.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfgunezwx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ggpibfwwl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/goefafuib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/ggefiiwmw.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gnxdgzwtc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/guvckdomn.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/ghwwfkhtx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gkzqrwnmr.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/geuoarpfb.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gpimzonho.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gayvlpnmz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/ggcgikwqu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gnehpwuwr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gmcqdsmet.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggtpfpvcn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gwbvbsmve.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gfscyzuvm.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gqvyqcgot.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gqgdrkkcv.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gxhryvamy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/giygekxic.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gziuorcea.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gnzczsnbi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gnrwamxxh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gedexvvcf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gmkfygtfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gscfpibct.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gqophpzrd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gghcehyqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfgruisnp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtnahzxeq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gofeeyadh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxqmlzbli.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gcaogavjr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gtuqssrur.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gjegdxpho.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gmycqjate.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gfbyfyecm.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gnyvysitq.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gqyhrfcmp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/goguqnsav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gupqmxyui.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/ghpzutvmc.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gusjewyhk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/geaejccuy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gcplmqehj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gfkgtmxpm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/galxnywcq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gddhuzzfe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjdnmfjl.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gqnywjivx.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gloeqgaxd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gpdumqwjw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gqrzgrtsv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gsbdxotma.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gbzlzhzsl.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gddfbnioc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gftpoafxt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/ggywokttq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gfnnnatja.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gcgrmccgy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gdqujxybg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gjzmrlqdk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmdzkfmxp.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gytzqzjpk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsyzqqqzm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gkejhlbaj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gthfpjasf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gdhypkmfe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ghnhvajza.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/ggwtfxfwm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gqjcchjdf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gnngnpumn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gfsylgqhg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gcpxiwrvi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/geloqhjte.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gbqjmxqtf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gamhczwsy.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjbfszifc.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/glcynnowi.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gzinzzjmd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gmoewpmyj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gizlflllx.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/guemhkhcc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gnfgyfmpt.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gyfhwljbo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/ghawmtrmd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gnjepyhxr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gdzptnnrn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnskdycte.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gakemaxot.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gqpptqpcj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gshtuqbrl.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gmnzbmtrs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gdjxpktrt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gkcktghsj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gtoiiozfj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gpxsslcxg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gxziphdjz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gsyjyhefl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvswiccex.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gnptexgey.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gtkpkhwjz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gkvopblqe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gemvfnfic.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gegnzinmc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gtxvzkzov.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/goautenza.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gyqtzudqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ghgijoypd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gwtknnksc.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gnvsvhkkj.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gdkqguuag.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggacnuavb.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gehdupwun.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwzajdqwx.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gvfyatetd.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggyblzzsw.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gjrbjhmmh.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gggupwhiw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gndiqqbzt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gmrefufty.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gedprthkb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gygwepuac.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gotzhtvbu.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/geawgqydr.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/goanneboo.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gqknjvtig.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gcwplolhi.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gattyhbsj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gllviqqem.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/girafqtwb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gypfdgrhs.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gvlcezvrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkfrdzwym.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gdaafbsfx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggbydlspf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gyfidvrgf.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gzeqafazn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gnjfmxokn.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gepgcprtw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/grshjoqvs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gitxkgvec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gwomzvmgv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gljzrfsxh.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gdvnrpyks.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gjqntrydv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/geesnzvke.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gvdrlhuna.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gjkkqtidh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/goygixvnh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/grjnvflyb.sHtML


<!-- 参考信息 -->