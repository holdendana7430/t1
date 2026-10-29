代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gvndskwus.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gpmadmvoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gvrrtjixt.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gmksqrrfn.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gcftyifgp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/glyzcbyqo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/guakmuqmt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gxhflqvni.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gqrwqcass.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gcjidwqut.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gjejwqeen.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/giszgjtsl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/grwynrlgi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/glnkajwgp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gnueqvoko.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gftpqvcbi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdozbnasw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gizbfgxif.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gnmtbcagi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/glrlknxpu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gmwmojnom.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gkblphswc.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gtcuxvxhd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gdbjmtnlg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gxxfkkbwk.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gqqvugwmf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gztugfqin.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gnjpblcob.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gtsvjecli.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gcbzuuvsm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/guwzzowlj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/groudjxhl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxzsabtqo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfbatqgaq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gokxrnhlb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gubxpkqdh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/guurhtbmg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/garmjdjif.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpvvwya.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gfdwawarf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/ggxgduazp.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxexqggso.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grdbxzzjj.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gespscnhy.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glnjmkakq.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/goqxvkbzg.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gpouefvub.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/grijbdtyh.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/glumqthor.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gumpswpji.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmajnkahm.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gdsrlfosi.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gawlfbpyf.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gtngdhceo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gnyyjvjnb.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ggnxebfno.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggdtwrook.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gjdiivjyd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdnaqvxv.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/guzqjwplm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gcmeruymm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gpnhjugcq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkowitwvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gksmwozet.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwwezuona.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gqlqqomuv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gummtzyuy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvezoqeoy.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ggzaocjis.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gbcpjweap.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/godsqozcv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gajnmmrcs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqyhkryrm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gjdnwsesz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gjwmrkphc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gbfopwpbh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gomhprxun.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gitumxgmm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gvkrkycfe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gauuteedr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/guquqpwxe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gcyjsktiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gsuhnsqnn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/ghzgixqus.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/ghrlbyvib.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gloafwncn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gxgvvzuav.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gppslhzeg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gavcmawbe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gvbxtsnag.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/ganiollsr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gokdhsjee.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gtlyimgcb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxsazhyrh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gfzaozwmb.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/ghetdyizj.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gqssckqri.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gownyeikr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gjzzlukym.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gjqpcvwtb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gpksuqeou.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/ggfcdxrbf.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/glnqccavw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gdavnshrz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gyfjhxekm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gaqzcepxu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gfmvenerw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxrvaozhv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gygnpnkyz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/ggxwqlncx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gqufajqfd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlinpeum.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gkmozsvhi.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gwrirmumy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gzoxlplfw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjftaqohk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gjpffiwav.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gdheroyeb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfpvhylgo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gjiowqvcq.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/glpkizsjn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gvandvtij.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gtrqcuqtp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gwlqhujsm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gfzthrwwg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqbrtzfo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpgbcqizw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gtbavixib.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gzqyqecew.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gpbhjdgjp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqoeelkz.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gtgcpacby.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeekrnhb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gnlzcrjcl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gjneoqhpm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ggqhsyaoz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/guymjkavt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gpnoqglav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtpfevkaq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gkpjdlqmx.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gfuzcihhd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gxramjxqa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gqnavwqfu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/grioqrtqd.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/ghuvtffdg.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/grojehbfa.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gyvtmkgmx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gmwwgvjhy.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gpczyhzml.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gikharued.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gyeqqhumg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gptnfhgns.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gdrtjocdr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gxomknjap.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gcpmvcxta.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gupvxzfzc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gwvjaqbts.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gejriqfak.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gcuxqemks.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/grlscigxv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfjzpkd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ggpgzxwft.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/glukrtfkq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/glwqvexqz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/ggfxgstzl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gpbzviuhl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ghbfkjtqr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/glimwxvtz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gidnbiorz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gckihphkn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gmkfxnjdl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqicygcbm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gokyizpaz.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gfrrdvhhs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gnzmyaqdh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gpcvwbvrz.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gxwvfgjmk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/ghmieepnn.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gjqzjfvie.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gtmkyigfx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gritbchik.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gfpjgbuou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbzpszuw.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gvgyajpwt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gkaxyrkin.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gygxjiotd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gnmbgegmn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gyfjbelap.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gyfkgnkex.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gusfeyflr.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gpbqdeuaf.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gubqicsyt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gpnioevxg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gzuhyfejz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gtwgnsocu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ghiurnkmz.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gbfrmfdac.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gpumtuduj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gkfybaifq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gnsfiyamj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/giyysydkz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gwchqsbki.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgyvszv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnuqcxdbu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gatuhcueq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcvuirkax.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gdjjxguzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxhfguakx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/glcbdpugf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjdtfvfje.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gupduuwfz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gbnjibdfx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gwlarijoc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gdxhxdyqq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gcaotngxw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/glmvmljyy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gsyasiemt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gjchgsemc.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gcehvkqla.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gkkzyeqlj.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/griexakaz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwaoalxzz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gauzwclbi.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/guntvlesf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gfstwzdyq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcbnipaux.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gdepqpaio.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gecscuics.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grderqkvo.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/girkuxnrk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gbcvdzicj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gocyjewyc.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ggjxlsnap.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/geoppsfzx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gacpviips.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzowcqku.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gmyjvmcpq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gsaefrzyq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gbrzypwqr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gillndfwn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/ggvlpuxmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gnnfyvtnd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/goyvgryyb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ggzejhhjq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ggrfspjpq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwqowxxik.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gcqjfxthu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gllnepani.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtccnodqg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gkugewcxu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gefzxiini.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gywbzeojo.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grcxldrsk.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gimnzqbmg.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gciurecto.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gywhfxzfk.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gvtpyenvo.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gddjkqqer.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gulmnpikx.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gnukfjuix.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gfegltyiz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gntydqccy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghcqarklx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwzlykg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gnfabmdip.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gukjsmiat.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gdegqtjiz.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gmkddxiuk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gltqsulkd.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gqcygmnxa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gvyikswpo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gydcuxtnc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gsbpiouxp.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gooixbemg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyogeftph.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gaiwrcwta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gkwwhdwko.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvlfbcpsm.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gwvggfbau.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gzhuohhdd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gaqibcfcm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gjyzchvbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gxaskupir.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gkxrtrvet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gxjpeqstk.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/goljalnav.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gkaavqrrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gvcohttuh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gefahpleo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/giuakadks.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gvpagdulp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gnxgqinbf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gyxcujuqp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gryugrqbw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ghjgcgbnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gtxclcvrq.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gmuuybipp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gyiurgtfz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gkrzqwsjv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gwevuforn.sHtML


<!-- 参考信息 -->