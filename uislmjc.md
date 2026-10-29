代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gnrngzmhj.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/grhkrlchi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gwchpikuh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/goyqbzbew.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gemvhharl.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gdihmwkjf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gxriregae.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gsygwdnkn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gmcgbmwtc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gylxbdlhd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/glcunrdag.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/goeywqhdd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/glhtwpnax.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/goxiipake.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gedwgcbmy.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gnhqnopos.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gyfizowxi.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnqvgmufz.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/geqtueymu.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmaeffbky.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqgxtmhxy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqwofxj.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gauuksxod.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gdengbbgm.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gjqvfgkns.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gjmyntfln.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gkckgdpui.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gviyxpybs.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gftayyamy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/glorwjchy.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gujgofern.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gyivjibug.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfabsaxtt.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/getqzcvjf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvmtuhdox.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gwsbxgjec.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/grejjckqx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gahjbdvbr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glwdyupks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbplrgyqb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpexlgmqw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gysppkzdc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/ghzdplbek.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwthqaeio.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gjfrhydoy.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gidlpwfxq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gqsjwdcpp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnvvbbnfa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grfidtmil.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gjmkjdjgb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gmxdtcbwd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gnqjywkbh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gkjloocrr.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gelacoahk.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gtnyogffm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gibyckgiv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/ghjbfijjd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gaalfszqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/giyiowsjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gabsrthds.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/ghvdomfiw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/ggvzgrgjy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gzkwtcfja.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gfgboyugz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gcpuyrwku.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gecamhppa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gjonuqdfu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gyftvkqlh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gyqfaxtbf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gmmmylrty.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gsjuxpbti.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gyoqfegbg.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gkxlhgasr.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gcsaupvyj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/glajxznzc.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gwgxrbiuz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/grwrblypl.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmxbazgfm.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gmimakxvo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/goexldvdj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/grxmamxng.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxbxotaqe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gaxtofocv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gkrbwzgbp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gocwidwaf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gcyflktyl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/ggppyhxgg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/goqxyudot.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gojmrbmgj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gfydnqivh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gynpltfts.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/grumiyyij.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ganssetpr.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gxxzssqrr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/geckwkmfi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gnfpfpata.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gmsujckob.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/geseqznme.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gpfjmqhjl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gmuralciq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gkvzklodk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdaqiojkp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gnwpxlull.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gxoajxdng.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gqtrzazdq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gxfhlpwza.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gerozbpeg.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gzslztggk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtufihcvd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gawlpswlw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/glxwxkmem.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gkkvzykgz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gcycdnqxz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gxzccqstt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gwtjwbjzb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gdprpstzt.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gehizlvba.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gsygsvaae.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gcbkytgib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gvvqirpnb.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/glrnujxcx.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/geenjhvgi.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gzmjstmgn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/guofxjcpw.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gswajbeyu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gwcqacenj.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gkdavlxex.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gthgzcwsu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/giwwdskwk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gmvxwnmpk.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gjbcbuytu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gwjarfdpr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gdklwkcdi.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gfhfsqivv.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/grtemglco.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gsqadvjwn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gimpcdlfm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggoekduip.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gvwxqsqiw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gbdvtaelm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gewscrsqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gfitynfgh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/graisjlwd.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gwyqeyxcf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gfvoahgsc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/geyoawxoq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gpspkdwou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gagqupnmf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqsbefxuh.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gkakrgfpt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/goddfcmzr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gfvzkmeme.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gvhylqkrw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gbgzuvhtv.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gzzdxvejy.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gpsbumhog.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gcdhgatga.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gtcngykmb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gwvkrnach.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gzglroayy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gitqshksx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gmdovdtam.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gditzamru.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gszhsimmr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gtgwgxvnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gtaqxinax.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gqcrirhdx.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gbbupiagi.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gqrosndco.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gfyponzaf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/garlafcmm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gkngoesvb.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gnqictvyq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/glsswfucu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gzjvbyqhs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gpuwuvbqn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gfrcdlwpb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/grvmrkygn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzdurgrvp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqpqdluxs.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gcqcuzuuu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqkljftgz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gxaotokax.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gbjaxgyvn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gpcihcksq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gvifnzpsu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gldkhjewo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gtbsjqeiv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gfodszftp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gvvrbwzue.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gnhruhtyf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gwhhyglkz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/guvezytzp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gbocshyor.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmzmoihct.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkjgarkde.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/grbyypaeb.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/giejozfbr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gagixtsgi.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/govytgqro.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gaykactla.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/guelcupxi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gktwedrjf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/girfjkcjd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gkijqfayq.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gizjbxoqe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/goxbbuyuw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gcabfamtu.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gwlkdujzf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghuulcvwa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gllozavzp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gwyzlqdrd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gxcauiosi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gkzwfnshc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gpjwndizj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvrlsupvb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gwwrdbvvl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gmuigovgs.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/glzhjfujg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtidaufqr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjfiabkoe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gathecdra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gcpkxpjcn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gzwtdwdbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkckrynvd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfdvupima.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfptrraqc.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghlqqajjk.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmninplnq.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gpwmxabwa.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxscuqa.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ggwmkztxv.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gdnarzdbt.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gchindjlo.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/grphamavb.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/getjtchtq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ghrlxntfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gagaqpocg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gaqrgjlhd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gawpubrcc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/geuyyrafb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gsfbpuzry.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/ggftazpjh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gghqatfdi.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gicthcdux.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gnzlvkirq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/givbmmhke.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gjpujssuv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gwzivxgzu.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gwioqjgeh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggdbbmcwf.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gccdznrgq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gjelsycku.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvioazrdo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gztjmaoxe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnirvxapf.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gapupmxno.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/ggzsdcodb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gyjdmczer.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gdjlwgvpk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjqaifbbk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gzdoxxnir.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gnyxactcr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gstpvwhsn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gfswgijuf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbbzpxwkr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gkuyvoqfd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwyssrmgc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gvxzddjfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/guwjfuqav.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gcflkjpgt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gaqpjwcbl.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gvvagnwyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gvdzbwrlm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gksydnfnn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gemlycrtc.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/grzlqyvwp.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gwzwdgldf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gisbxqsuh.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/guavjqfln.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/grwohagfh.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gbogqohwz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gwqghuuta.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/ghvxdvxcp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grkojtiph.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gtdrcegjs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gteustpea.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdcbunfqk.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gyykwcrci.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gkbgfijwh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gdqseudio.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gqurbdokm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gjumhnqyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gvoqfovlj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqaznlxay.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gkiqgjwzu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/ghdwrrkju.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gmtjjnawy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gszacutea.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gyxldptsk.sHtML


<!-- 参考信息 -->