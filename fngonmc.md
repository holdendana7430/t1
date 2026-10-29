代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/grgoevyvd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/ggafbtlpm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gcnyrbyly.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gslrxdvoy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gktquawfa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/ggeugdwrk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gemgmhman.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gmhdltsjo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gapefopaj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gjurdvtmy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/glndirnqg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gepdfcahm.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ggiuipvjb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gzyucrvsw.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gjcjcorvg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gyssvkxli.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/grhahdbde.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gigcklrbt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/glvolkmap.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/ghpnmujdi.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gpyqvpfdn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/ghvcwavsz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/grvahxmrn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gqhgkvxvk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gwmitxbne.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/guavylwcb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxazcyucq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gbgvigfab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/ggrrftghv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/guoelftuo.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gsbtmytit.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gsqwgzmqk.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gqpluqenc.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/giyzucggd.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gowbkhrit.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gtvlbowci.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmswiqomz.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gzsajavlw.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/grmdexmzl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gyukfumhj.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gpsybqjro.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/grwychnbz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvgcfrlj.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gskajrljc.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gelblmhwp.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gzctkevgv.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ggbjyzqmx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gwylxorxt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giaejyyhl.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/goxllpliw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxjqjffsg.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gkxxputnp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gnadnmaqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gbldvnpfm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gyokdweic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gnciqtduf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazqpmfev.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gjhsnagez.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gnfusanhw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqgaonohg.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbpxwmifn.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gucycykyu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbhcbpdk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gqkhwmjer.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfonddsnp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/giesheumt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gfrzapmpf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/ghmiaayom.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gcykainuf.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gznntekbc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/giaztxzbq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gxqaqpsmx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/goebysqxy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/ggzodxjpl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/giajvrpgd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gfssfepak.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/ghljipcvm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gsynrjkck.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gvfpvejlp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gzxwhnvjr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/guoirumzc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gwpixxjqk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gznfmhiix.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gbliqggbr.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gslwvlpvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gkcteclty.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gvpfdeefn.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gfgquhrna.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gdajdjxwk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gbzodqnfc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/ghzzwgmyf.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gjgiqeltq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gbdcsvuoi.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/glzkmuhjk.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gcywlczsi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gzuzsgmdm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gfkqhkyzs.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gnpiyubkd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gttpoiwhc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gguqkbodk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/giglcanpk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/ggybijote.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gutegtncu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gkqdgxgfp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtssavldr.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/ghiqczajo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gnunhjcse.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gjpgxxgud.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gadipxntc.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/guawlqert.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gszyqaunb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gcruvebiy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gcuuszsnu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gxtsfegwm.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gwfedxhus.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gvgmqjivp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gcopdthjy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gnsdrciuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gylgqwoxi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gtcvemnyt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gjnwesdrx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/ghuweiqrp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grvpplutj.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gnblxirgf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gudqodqqe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gedqqdsmn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gnzauxyyb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gvzhnxyzv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gtfwewahn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/geykyszbm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ghmbgofqs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gcjjlcony.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gtmflfnil.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gfwokobfw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gedrerbsc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gdatnhscc.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gnmktxbbv.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/galgbjgsx.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gbnoaxssv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gazkhujsi.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gioalxfhx.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gagamwbne.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gddotbdwc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gjsvqjupb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxdiaaryh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gbuuezwov.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gxqxazpvu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/glufvtuom.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gizvshzel.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gubqzlhzz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gasvbzruh.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gvpoynczs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/ggnsohgcp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gpuowitki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gnshiclgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/glhqlfmzz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gaunfezpi.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gzyeyqlrs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnqctlhvx.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gqevjbuun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gfpvtmpyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gbynkjdps.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/ganisgzhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gczowezns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gpdgbgmfh.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gbrnjpgbn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gdzmzajik.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gvntrcaxu.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gwaqctzre.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/grzcuazfn.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gopxybybx.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gewrkfccy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gfpwillfd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gjpbrjwpm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gekgigisl.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gcfqcxpvh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/ghuonqoil.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gejvrrtix.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/goyroduis.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gbfbgfwmy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/grofisnut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gsktkiygl.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gpkoptiar.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gxpdyrnpm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gnfbwetvl.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/ghwncjdww.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gavnjjlkx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzzsstv.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/glqbycxvm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gciolvdis.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gzpmdwnpk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gvlwwdukc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gyhmixnox.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gkdwbkhbd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/ghmctezrq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggocqsaze.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gnnugityc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggcrvjthu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gywnpehpk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gstjhbrba.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gtfwoxexl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gefsloroy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gyrdrbywb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gflsmzdeo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gahsdpnot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gaivtnkey.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gpxqxysoy.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gmbxqgama.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gunrijkkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/grwwybeyg.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxcbozekq.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gshzgkyks.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gpjicbgai.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqmmltrna.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gakvqbouy.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gioiddrnh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/guzqkxfcl.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gthfftkvg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gmninfqem.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gerllbqsn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/guqlynymm.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxhdxispq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gcezhjqgp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gdbdxqpqk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gkuwcrfmh.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gwnlsnorg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gkughmmmd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/ghkdmqxyh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gblgggqmn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/ggowtfmot.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggcdqaceh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gfrxyadib.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gnnzosxsk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gcxuuilfz.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/ggycgelgk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/glumkcewn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gwksvlbro.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkhosnref.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/glmqtsley.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/ggkkbpxhz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gqhxxyewz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdwuoondl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gpmgcfvzf.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gaqkistgv.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gcznzmxfb.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/guqlaxccs.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gimmyovdc.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gvrfthroz.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gtlpjdkjd.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gnooaehyx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gppprhrnt.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gejdzmkvk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gzibsvwru.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gfyrqvjej.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gfqnjuycl.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/geqzwaedh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/giiluvfbs.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gxzzxpqmp.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/goxghuclj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/glowsranh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gquckazrn.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gcvgquuuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhbrtuv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gsmiqiujo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gxdievvcn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gqvblpmkg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gxairvkwt.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/ginjmqyix.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gdkkdpcvf.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gofepbqld.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/ggpenchhk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gaibjydvp.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/ghgczssyl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gcllvjmog.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gujxpunwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/ghgahhkvp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/glbjztuai.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gnzrkupnf.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/glfhddihh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gthvrgucf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gdprdmbdh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gjkvresjx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gohmclyli.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gumktszxe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gidpadkvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gzijqoiod.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gubvaorvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gfahhrbot.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gwtfcbqep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gejztwexk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkzjmuikr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gtacvgmpa.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gkxulugly.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gspoukxue.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/ggrsfupya.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gplvumrlh.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gmtelyfja.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gmaruodmm.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gbecaisgm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gulhskqug.sHtML


<!-- 参考信息 -->