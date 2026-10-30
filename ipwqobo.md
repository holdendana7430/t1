代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gohdekdgd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/glyjzltae.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/glgeemmpc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdycqcyfe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gxskvnxkd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gnxqebpim.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gxvetawfg.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gzegnkuuq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gvfeaxadn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gyygdsyuf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gywzbbaty.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gcbarnqsn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gjtpitwmi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/grxrynrey.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/glclrcmzd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/glgbkyigc.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gbfxthvab.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/ghvfacfbb.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gmjalaayf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gamnteern.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gprtihpru.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gfszdnppg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gohijwrfn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gbmlzmmmb.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gokbtlpkg.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gmkyzvpge.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gqqleltus.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gsyirihjy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glmimapuh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gxsgfwfwl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/glsvamoig.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gnsshouiy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gnmzzynfz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/glwspypvx.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gbdptnbll.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gwpaxbkyh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/grhcyrhwj.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gnthwdyds.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gleyqyfso.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gchrqwkiy.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcivzagqt.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdhakyreq.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggjwervby.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/grlslooau.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gfygugkow.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gzciknuhz.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/grkuchigi.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gppjvvrrt.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gztrtsobi.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gmperhgqz.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gcdmezkoy.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gxxymntyo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvpxdvppe.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gfwhcdqos.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsbdzzikq.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/ghyiutrag.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gqdysesgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjcthwcrd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gmugmpktu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxreivxsp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gfdrjrkvn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gfzqmqurt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gfsegyxju.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glzssgigb.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/ghhyqevjf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gewakgqtr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gloxskjqz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcjkevcpv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gluibhbvs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/ggcpamgya.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gwinumnie.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gbhpmdcvc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gmeqxhick.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/goouwntim.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gryvkysor.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gnwdlxldf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gmvlxekfc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/goxoplbws.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gipaelufa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gemzpajpq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gcrmeedgn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gxncltbsf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gnhjyhjjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gaavnajyj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/glayvpxlp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gpxbalkuz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ggcjpldad.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gcdtultlp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gxzyxpyez.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzkpfgynx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gkbmefhzk.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gbopanrol.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gmtshcogl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gjzcncvfq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gisdszsjw.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gejliewsr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gnmwvnblg.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gexiauyjj.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/glpoijlac.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gitnwvxjl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gqazarofo.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gouxxabuz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gucjjpxgx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gesrxtrdq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnnaiiiyb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/grrjbgajq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gjwocwkqq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gsupzumdk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gpwwgcrxh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gmytvsfme.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gstcokzbv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gweqthhqz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gwjrjttph.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gmjspeuhg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/ggzztfdvc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gwqxvckng.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gsaznupvf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gzryqilvr.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/glicovzvb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gfkixcyfd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gnklaonkx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gulqjqvmj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gglapvskg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/guhfqfmjp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gmboiowws.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/geflaswof.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gvlkwkpkw.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/goeuozbce.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ghecriagb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvooeoixp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gbdvxcozl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gcipvxbey.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcxvtxibg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gwrumvhll.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gezzguogw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/ghfykwvck.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gcwaillcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gwcgxccnj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gioycgfer.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/grsnlhbia.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gcfkixiqh.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/grzgkieub.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvvemaqqx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gicacewso.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gaxcuihei.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gtfequnvu.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gerjxnnfd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gsacfkbsp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gkqzkasaf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gcklwyezm.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gnascaxvi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/ggexfmces.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/giybalsbu.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/grinzblxw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gpjkovunf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gkkkyjuei.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gkmabipkl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gwlraaveq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gccwxnqor.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gnduryzaq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gesjcvusy.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gqtwtfujy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gecsytjok.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gllmotmas.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gpftpwbgr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnmjbdxjh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gfobsuxwm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqmitdzox.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkmfcgldk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnyyyqqrk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/ggerwfprs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gmurzdeor.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gegufcgqx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gzbrjtmfy.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gdcuhnhfw.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkjbvihds.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gwylztmky.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/ggrtqvxto.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/guospvmiz.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gvfcehwza.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gjwjzyxnq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gmodpvger.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gznvyowte.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gtyfoails.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gqohcvzaz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gseasofjq.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/goprokztd.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gflymxrmg.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gtvamtcls.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gnoguarch.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gngmosjqd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gtcnwynyw.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gkkgkorxo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gbazmdymk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gyjqfilmj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghhposnqj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gfyifancj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbmzzmbcf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gquezzqhk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrcghlkm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gknbodykp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmcehprt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/ganhkcfqg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gtycjotru.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gosqtjhjb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxbqbcuqf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/glmxiondo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gjagpyhku.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gyvqewiyz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gezallkui.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gokzcsmbo.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gqtbvqtkn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gbzduxycn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gmbdxxlpb.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqwowknpi.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gyltdvnce.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gdsrxniib.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmkkikivr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/glybjfuub.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gxjbqqdmh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gmlkoiwdk.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/ghsqorgsm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gtwresqch.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gjrpumbag.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gcwodqilz.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmabqnnqq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gbxcnvnoi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gqcnmnvbh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gkzsyltde.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gimozuwpr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gdytnksko.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gqwksgtkv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/giyivsewg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gacctphaf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gaeztjned.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/geymzdzby.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/giixwsenf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gqfvcwtmp.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gnfjlzftm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxnqhxb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkcaynldj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggpocxoch.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gdlrjqhbo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/goeuklosc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gwftqablt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gxevcljkb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gmbkkizur.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ghrihkagk.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/giopdywow.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkiarakzy.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gppbcaypo.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gfreqqesy.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/ghvubfovj.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gtklbxczt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gwxxzntum.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gihaibrrb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/goucurbcp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gzxnlmkuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gxffqobdb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmcqcslgz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbvabkfre.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gsydqhomm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gwaebtlff.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gafeysnzf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/ghocxxonz.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/guyunrhdu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gyoeerkql.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gbhuftcjq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gsdgqpwrs.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gistfodpk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gonyiaoil.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gljowqhfz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gpxwqeujb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnktzdisa.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gowmnemus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gzqddzghr.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gvckenxun.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gewpyaulk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gtpktduor.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/ggqtnbruh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gglttjvgg.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gklorbjqc.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gizgrvhdo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gvwavscpz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/grmywsweg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggqtkqkwv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbnzeonzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grwnjjhbz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gfogrndqe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gizqbpspv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gxdwcxshq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gobmsassi.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gcznpclly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gyhrldnfv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/geqsnxaks.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gxukqzpql.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gahhhffov.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gusvohbsh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/grthemicq.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/getifqxka.sHtML


<!-- 参考信息 -->