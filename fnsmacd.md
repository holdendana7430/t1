代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gekzijzpu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gmujxihys.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/grcevlbxk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/ghphtpcsq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gisqzdare.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gqbzlygeu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/ggzsqivow.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/guhziqvjv.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gqyqlclho.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gwnaytqge.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/guatbsjju.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gsdioqclf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gpbdrsxsn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gkgykvlps.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gbrwkejpz.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/genwzvanw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gesmcfsbh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/golfkchdb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gqyynuqxj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gpbgymvxq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gwjjwfybk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/glboxapwq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gucvosdwm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gagxgpybq.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gntxucmlf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gtpwcbdze.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gjhthakkl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gsmkntjsh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/goeskrgko.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gxxfipwms.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gebfafjog.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyandjpx.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gitomudcs.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gtplgjagl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gqfxhcwlu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gpgkwstze.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gszyeozdw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gqpirjqbr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gfywjyrgg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gtvcrseck.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyhncitfr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gjuwkiuxb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gdxlzcibv.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gprzubhpg.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gncpemgiq.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/guzygsukf.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzvzsravv.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghenrxdpv.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gdcrhnjll.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvmvoiggt.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glzoklyla.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gsftcavgn.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gadckqjlr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gebqrogis.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gtkxwixiy.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gnwwjsitk.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gaqxjpikk.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gfyhwrlah.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gchhpdphj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/girwqdtyk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gitxkwvzf.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/giogfizwq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqnwwnxiq.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gnvqfvxcx.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/ghsfhbjnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnkfhhkwi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gluszitth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grhdezatt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gispeoylq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/garttwcvo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gdgfgbusf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnsfglbgy.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gjtizglnq.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gpzxngrms.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gctmveqvi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gstkoqecf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gsusvryyb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gckwjtgyh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gsjnhmzzf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gwlmgzzcg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gykrnwqjv.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gllpvjnts.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/grbjzlhcv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gvzixssqw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gyidqstps.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gshvbeybk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gsxugnexl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gvteieufw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/grsgmozao.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gzbnqmwfz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/geqrfagvs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gormuctka.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gtvdeojhr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/geeaadeiu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/geqvfmfdp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gjllfdfde.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gazzeyaxz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gnklcaanu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glslitbci.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/grzzpoomp.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grkhwdwpr.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgaycde.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gpbapzjwc.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gdtixumpa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gibzpvdvh.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gkolheoqd.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/ghwcskrmr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/ggcayvvye.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhahoul.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gusozrikv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gucfjphqs.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gosezhvhy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gjvjeocdk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/greviwkod.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gawymjurn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/geplyyhru.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/guasmnbrg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gxcshbfdg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gldtudjbb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gbywcmujv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gjvijigog.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gkxewsutr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/ghumncnli.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/ggjsquals.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gvfqgwfjh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gfjjznypx.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gcigsnbbn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ghgmygeez.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gwdzcfbwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghclkcpqc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gkucuoswv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gghxprdgp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gzfqsdgnf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/givaytgmi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gemhjpvss.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gvaqmpbgi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gwkayddjv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gbrgsnhou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gqkmmznse.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gydxauivt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gcrpryfww.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/guvcipaax.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gnmyhczsx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gvejzpllf.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gtxuoiqaa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/ghqnftvxp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gdeliurcs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gpfbbjbfe.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxkrtdghn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdbwzrmzd.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gypjjlvsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gassajpjo.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gucdorcnv.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gsahohlml.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/ggxykjdqb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/guuohinwi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ghvwdkdqq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gexlknlgr.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gutagzgxw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gluokipon.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gznvqzvux.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/ggbxbsacm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gewiazuum.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gbuougmjd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gpyadftse.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/goqzdojcf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/giaviujor.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gwaqrpjzr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gtjnoboub.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gpphlselt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gpcihqtud.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gxtscslpk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/giyhinfvh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/grvkvtnhs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gfyzqdmxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyssctutc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaiaqtwbb.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gqzoonxbo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gmzqdjoot.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/ggsphpcel.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/ggplsbxvd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gwgghzypk.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ghbwhejjb.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gblmckdtx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gihydzsvj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gxwdpzcvh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gtxkbzwjs.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gbiftqhmb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gufzonbps.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gkkcplmyz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gajtrvdzm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gnrucyjzp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gbthgazwd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgwimhcx.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gskvwzblw.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gvzuclgxh.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gxkruuwiq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gbbyouxdx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gmiqplrdj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gatpxldll.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/godpzzask.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gtxofjoep.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgdzvez.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gkyuokxeg.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gmacfyopj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gqamikcjv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gcdcgeuup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcnojwtum.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gjfzhjjhi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gowtjnagx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gszjpajzg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfqqagv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gtkukqbty.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gmrxleagy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gutyzwcdq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gzvlwamee.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gohatvlve.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/ghkeawhme.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gpiygnqme.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gbwhbplyg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gsnqduwvy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gxsqnucst.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gpsdzurgd.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gcbnyvsgn.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/glixtihjt.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gwdgkbczj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gnrtdeqgn.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gzmaewifx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gzmlbgscy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/groevifdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgazmbub.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gaqaudhpt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdoszggur.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzdvymcoc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gkkfjkorq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/grthkdzlb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcrxdybnw.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gitkqpkzg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gxjrrddfu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gaiimbufu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/guycywqhi.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gpufhlvcz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gfybkynma.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gxldfebnx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gaoqesvau.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gaqaqsovq.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gebszawjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gnmjdhjgo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gfegyseoa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gogqsrygu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyiusuegb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gzfhqhsbi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcfsvgjga.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfzuzsqki.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbildmaux.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/glstznxgi.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/groqtnxck.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gpuvmqiet.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gfcxzaugh.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gdbymcnbx.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gnrrqzcdb.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghbafwpmg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gnbofxlil.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gotuyfcgy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gapuaspjd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gizaamvye.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxzoijbdr.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjekybvus.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gemalineo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gosgcilkm.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gqvuoydss.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gozyfsuaz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gshwbudyw.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/glujjtqaq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/getibpkcw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gscasuzyu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gstxearmm.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gqvtbcsmm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gyeilwbba.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmlpffiuq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gytwsejbq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzpasluhx.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gzvnbiwwr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/ghauinlzd.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gizflnkdn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gowlyofcr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gelckuzvy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gakembjww.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ghxotoibq.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ghzplkxvn.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/ggdsanves.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gyzzywxtg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gtmuapwkj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmsfsyzbl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gfgdvvxdv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gnmqbugjd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gcvfwgbrz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gweiuktlo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gefalnyam.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gzuknpyiu.sHtML


<!-- 参考信息 -->