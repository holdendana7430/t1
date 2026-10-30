代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gnlmmayur.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gsaixslel.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gbleipcsk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gadhnvolh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gwsyxpmps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gnumiarec.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/ghfcfeprd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gfpqqdlaf.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gnbxwdvuj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gmumcnkqy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/grdgwosmd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gvzrpmlqo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gwnpnrecn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/glslxoozg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gvrbausvz.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/ganccqjfi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gcmhwhwre.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gxmmlwyzg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcjhqdcgw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/glkedruwl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gezuktyqx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gksxdufhf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gmdrtluvj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/grkhobcum.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/ghbxlgyrd.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gmdjksfqx.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gyfctngch.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gobpzonxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gwffbrlza.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gurnxtkcd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gkeiynjdl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gfhhdxdof.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gsnapdgbf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gdiyaocjm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gvrnpurcb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gntrnaktt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gacivvbab.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gncqajirg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gstkmtfhi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gutfndeie.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gzugpegfr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gisaucpgd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gvskgeosr.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gkkkkwvuw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gvisciysy.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gyxqgchek.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjwcijjcx.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjnvbejqz.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmhndhxqc.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjqtpaylu.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/geifrtcwf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/glomiluis.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gjentbuwt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzgcflnde.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gljwlerpd.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gukbfonhr.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gwashxuxt.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gtaaaxkwo.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gpofbyhri.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gggevbjqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpntbkmsd.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gaqomyklg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfpwwjxda.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/ghgluiljj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/grxfceuja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gqcbrhdoa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcxwvegem.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtbxodzaz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnzqtijyu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbzvkntgv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gmdcofrrw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/giwwyfixp.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gcpaebuzu.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gijinxiqc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gqftdotlq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gqlvjybvc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpberijwz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/giaqmvhop.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gghrodvtq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gukbiquyw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gdwawphrl.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gtbeumswf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/galkmqbak.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gekjhtbag.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ggsvtjfwx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/ghvczdika.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gvtczltab.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gpqczxuas.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtpumrfxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/ghsslgkhx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/ggpardjyl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gkncqihri.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gjcdjfnqz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gmcgmuzoe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gmmlixzux.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gypmoilvs.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gfkpdctin.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/glyryteta.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gdphueecr.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gqhlnfacl.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gorkwevvy.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gewpmyatg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/ggphwihpd.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gldhrejvw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gpcwouyfj.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gisctqyed.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gmkrwkddb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gzhwkbokv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gqlyslcsf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gtvmaidgl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gozlkgwlo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdsiiqklm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gqjshzfuy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/ghgweydkd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gagahamgo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gjuyxtajd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gabjvbypf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gvfilqpgo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gguuymseo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gshglwxct.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gdqfdhxqy.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gnhyvqlim.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/goppapoeg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/ggdfbhqxq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gmgxxnjou.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gwnzpceaw.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/guukadlza.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gaehiwlaq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gpcsolzcs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gkfmpimwn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gsnovorkq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/ghqoaaubu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gyfyglszh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gbrbpgjdg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gasxlhlqv.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/giwjgwvmj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gkjwjprqd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gobkdeara.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gbwzekhlu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gsazhrkrh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gkbinssei.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/glmqcuoza.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gglxncuji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggwtiuodg.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gooxdjgmi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/glhpglqid.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gmoawumrp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/giljvmcaa.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/golezqdit.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtizsnoaa.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gvxyjykrl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gldpuqlce.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gudclpzpo.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gvbxthhua.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gpgoedqax.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gpeuxxjaq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gncreaumn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gywxmupmf.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/ghkclgolm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gcrvugvlt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gczukgmxz.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gehpzcrpq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gbwkdntpj.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gefsbrwme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gwbdiiyvo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gchlbbjtr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvyxkibiz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gxcxwwlbc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gtozomyrk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gpkhqglcn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/glwfudwhu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gpvgzslsi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmjsvooqk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqsxxqzy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlovxrv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfowmgptq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggcuqdybm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gaoibpyiv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gnsbfldbt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gzztmqdei.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/geuiynrts.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gpslbtijm.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjxsmfjrg.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gdebiyxaf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gfztqpfpa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/ghnszjkcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzboygfph.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gnarkovuh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/ghbckbrdk.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gbhbbqyun.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gjacoyeqs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gekcktzbs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gekbigctx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gtopjnhkl.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gxdmvxhyt.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/geiifahfl.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gigionrpm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gnzszyvsm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gnznyzkky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gzufhwuwo.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gqisqjise.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/grwbbjixd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gltaechpn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gqwulzoro.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gvswlxgxx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/glvelglkl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/guvklilal.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/givbyfykv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/ghskxrtay.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdjkrrluv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gfvyvmrro.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gzcubdqdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gzyxexpbx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gywbrlhdn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gcqtaamfv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gkxazxukk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gftzlfpdi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/ghyaiyynb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gkdesgrxt.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gaezucyhm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gnsqhjmqa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gokiiaxtv.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtkepbhta.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghmmakwym.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gzyjhucem.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjucqpeg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gyutzgbco.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/goyjiahpq.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/ggozphmkz.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gcuklefiv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gtouxajot.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gjekuarpp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gbnwsghgs.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxegbzbct.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gyamxljte.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gpwsgtxea.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gflanqdcj.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gkgosvxia.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gyeogkfrz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gbyrqllao.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gdtlsegsq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gfbrutysh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gkvkrklgh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gumehylvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gucyeuhnq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gtyacqyzz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/ghuukmebi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/guszhjkhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gzfzrindr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gblbiglug.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gthxkxjla.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gaiqzarog.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gcnbhfbtg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gfvvceqtw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gusgfvorq.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ggtbtcibi.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmusxjcyj.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gneosfmuq.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gjofzwxdj.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtgxuxsjv.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gyxzmtqxd.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmajzhprc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gbujaeaxq.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gdcumpymg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gqevpgdrk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gmglwnwky.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gbtieqaoq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gfwzmdkeb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbjxrgprv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gaywoojww.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gtefvfdrg.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gjrfjnhms.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gxkoxkdzt.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gkdaqgkhg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsxnkmvit.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqurztlst.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gnlioiywz.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gbyddjufa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/garctchrc.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gtxxvmcbt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/glqdqmebt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsaioeqj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gplpoeoye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gshbcddrz.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggpvbnhsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/grljyzypb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gcdrwzhop.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gkmurygoj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gyqxpskme.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ghpawmcoc.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/grlmdjlfa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gqhgtjjke.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/grgcrhdnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxeqmbhrr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gpyaxkryt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gnzyajocs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gixtbphog.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/glsmnnnsa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/guiowayfy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gckcngcfd.sHtML


<!-- 参考信息 -->