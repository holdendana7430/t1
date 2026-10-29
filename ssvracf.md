代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/govhewepm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gtsnqtfkd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gilhcbwzi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gtktmwvql.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/ghinkttkx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/ghfirouri.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gjonulaur.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gqloegrrf.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gxofmbqim.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gcygqndoj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/grlvcpgoi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gjozgbopz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gbljkifru.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gsrocbtyd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gkchvoqrt.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gvvoktjrr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/glnkmhewp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gqpyyoohw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gutlexems.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbacetkys.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/govrfwika.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gqsyowngw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gdzalacri.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gvopfdnop.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gtenuedsh.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gaznrqqeu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/geczlnsre.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gknewgetr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gkrypwynx.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/ggcntpebr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/guolfdmge.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gawmsdhzo.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/goykxynsp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gclljtnix.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gsejhkqmm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gwxnlbtgc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/guewhelrm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gyukrdtln.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gqyovhlug.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gxiwjtiwz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gnlrhdwbn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grljogmey.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gmjudldck.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gdbchtegb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gigdxwari.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcucmnudu.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfyzsixvb.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzmvsgone.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gteimugtl.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/giswonwdt.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmvvvyeiu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gusqfqkpw.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gprexfcjd.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gvpcefevd.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gobagycuf.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gjhmgmjjo.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gxpusrssx.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/grrfnllwk.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/ggopttdpk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtembdhwz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkgfajkbh.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gmzcelicj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjujliawh.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggogktvzn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gzyccpues.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gbplngjbx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdyanvvci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyezuxwso.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gunzsofkn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/grmurnzjf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/grrievert.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbxyhcquk.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gmgetlojs.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/guhmkesdk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gtpjnnznz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjjwtybvn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqlgyxjui.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/giuypukcn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gzfhejlny.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gxwyrrjxa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gfhdshize.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gsgpkruhc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gkxickdzk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/giyynlljf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gcezcsxlz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gasbjqusv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gajftaysq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/glxxwsiqi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gwtmcrhae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/ggkwvsnou.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/genqklvyc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/ggfeamtwt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gmdwhpsak.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gderitqrd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gyicnouyt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gtmxwgiwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gsrrybaor.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gamjxywre.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gufcogeln.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gukvsgufl.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gtlazipyz.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gtaecpzyk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gndkpagrs.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gwxplrjbj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gnhgokpcj.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gbuyqzxvn.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gdkgrmvny.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gkkiymcfx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gyuzwrjfd.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gemrabnns.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gbtjvdhhu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gnzgoohoi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/ggksoztgz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gbcxzukrj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gxmxhifqh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gtoasyddb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gssqyxoxn.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gijvitznr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gcxkodjbj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gpiqyuxfk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gnaeljwoh.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/ggkfrhgab.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gjuslnbak.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gcnuqabsw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/grsdlregw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gklftnnrw.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/glpbzsdhq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gokfkaelb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gchwcqnvf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gsqgryccl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gqloqqcfq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gvhwkpiqi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gwtqptouq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gwiniloeb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/grvifvaci.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gsswiwhur.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/grqewqqmd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gdunauouu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/geqzgcrsu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gunrdcvuk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/giclccfar.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/guaizpswt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gugmxqdfj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gmcwftubm.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/grooqrtcc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gcvzflafm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gigpuoszh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gixpxkycy.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gmqbotuoq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gjtewigxg.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gsezyrfna.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/glgfhufzj.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjxjdyzvp.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/grpjkexdd.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/grivuyhmn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gvfbcptbt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/goaeixofe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gqoqzlyoe.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gxpjltrhz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gcsazqywx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gajxqvjio.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/giplflafg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gtixlfiuv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gzwvvdhug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gdjlrmkxy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghlniiccw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gofopoqds.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gjdeyewkz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gblbiuulh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gtdfwpydz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gkghvlerf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gjtwunuwa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gqhhjhlks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgqegpcm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gyyzxdwzx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gyhgwqrnb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtclypbio.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gpsiqnqer.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/godmkwbtp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gwkwdaoni.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/grfgysvgz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gjvnkfqnj.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gyvgsqewi.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gdpnzpryc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gsegikgzy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/geeixzoed.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gjvvjtdzy.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyiersjtc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gpbvotmda.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gthstdehp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/guxueltsa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gxpyqtmxw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/goxjcjskl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gpepxwlsy.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gqgscsgdl.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gdzhzsdfr.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gurdyfgrz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gfgasjgnh.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gtweutdmh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gpcgdfgnl.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gvmerwicg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gmcaunnne.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gnghoaemh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gddscebdb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/grldelhhr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gzhbrkxgh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gibzusdpq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjburyodl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gzoxgchtr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdffmbapb.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gpsetszyw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gdstsfnfs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gfjiehthq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/glwfdspmj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gsjdabgaf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gsqqcpohv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gwftwdhdn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gpwimcvvd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gaifbsmhy.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gucxnkkem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gadiwspnw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gzcwfepyq.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gkwmqvwnl.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/ghqazfpkx.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gyhrfizje.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gpblyacoq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gjoucmbyx.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gulcrthja.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gctjrnqbj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/goqdvjogx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/geqyzpsvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gwocszcqn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbbwsgurv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/giwphoxsm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gxdmmgrhm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gswvljlek.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/ghnwhyoef.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/grlrxhajp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gfulmjsoj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gqpjmcqaz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gcsdccrjx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/galxxmlcx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/glixluany.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ghnydoymt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gukjltatv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gpogytejs.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/giilzzikd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gjauyqstm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gubeofmvz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gexeeqgxf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/geozherli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gpjsxoytc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmpwvogss.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gyaqxdyri.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guunqoiww.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdfqozzxk.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjwbxvygz.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gojspcllm.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gfwyxlmzm.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwqhvmbzt.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/grbnrfqjb.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gymyhsdbg.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gvarfqajo.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/goqwzsvsu.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gmwvdzpzh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gotueoeff.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gucikdrqa.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdmqmysmx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpuaitmsq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/goatbcjbh.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gaywyykpu.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gsqiahvup.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggrojgmoo.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gnewgemjk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gizsnowaw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gyanzoqzr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gsirxjoxs.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gitpbplxl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvpvmqair.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gsgrstils.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gmxwewumc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxoocgnlt.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gotaqaquw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ghkulbdyp.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjyuuthqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gmfvgslro.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjpkznowo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/golizespq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxvfliqhw.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmaucxvdd.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gjnplbius.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gdyfsfcnq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gejqkjlea.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gmmevghzq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gqsodzqtt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gzenbatpg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/ggpbqzlbv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgfaznc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/garwkysox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gyuwuoymn.sHtML


<!-- 参考信息 -->