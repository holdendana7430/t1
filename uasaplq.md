代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gmqkwnztu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gjgobrnkh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/ggfqqwnpq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gkzayatbm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqneqiyhs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gkzltjqak.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gopfersqt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gzulzogrf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gokmwogdd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gztkxvmsn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/grddvkbtl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gzbcdswjs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gugzuflbh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/ggedsmwfw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/guxevuvxu.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/ggtwblfhj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gxxtucqnk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gtktmtnks.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gfjifonih.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/ghenpmzjy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/grxyzchbf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/ghmhujqep.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gsshfooot.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gerngashi.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gddksfnqs.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gmglqjgif.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/grhwplkok.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gptmnafkm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/guchssnng.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gzubojwas.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gnbntibaw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gmmybtkqh.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/godyfjdyp.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/guyhwmbbg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/geczrmpxn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/grdpctyno.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzhpqvr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gtnidathi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gvfiozgej.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gsryuehiz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gglficofa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gylgaetri.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/geeyaxtsk.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gxyhdlnip.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gfntalond.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/giqrxawsh.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gopypxxkw.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbxyxrwku.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gxvqzqsnm.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggiwazqeq.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/ggtsqhyig.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gphczgloh.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gdihsowrw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gnlbtddxf.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gnflqauzg.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gojsobmgw.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gpekurbng.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gxvqvouyf.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gnogykjqc.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/grlozhety.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gekqiunet.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gxjwlocik.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzdjxkmof.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gnhunkrgs.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gazmgpkow.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzhlaywvo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gphevfxyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvrefepur.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gxwonxdjp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gezjagjqg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gjslagzjl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gubwdiiuo.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gpuvvsjhc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gimxeyknj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/glowjffyk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghisiwgbk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdeywqtij.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gzekzmwhb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gkfhcgzlk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gekywffwt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gmjdnphll.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gouodblcj.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gwfwcyzwx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gsszgiaqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gzmddydfp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmpbadake.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/ghvcmbmyq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/ggoxfwtyx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/glpinvxnb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gsdpdgzoh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gpdxpxsot.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gfdfmngwe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gaydsmstf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gjebgmsvu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gqcrbtnen.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gyenozmdq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gybwuiqsv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gltqljzpz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gfnwngydo.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/guovrjjoc.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gubocrvjk.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/guaeedite.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gpkbgaxwn.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/guirndria.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gopmsslta.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/grjhmdypq.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gkawxdqxy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gdloroisp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gydcbkezj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gbcubyoro.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gvilmghak.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghuimvohi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gfnbgxplr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gipimngwi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gdcjdyijf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ggdugcmpc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/giqfvbzyd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gnvhwuqbl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gngpurhqs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbdjaetah.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gacwotabl.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gzxdakipy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gvytcthqu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/ggkhvrugq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gbthuwfsx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/ghgeaplke.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/ghwkwkgbc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/grerdulfo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gryhingzm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbmjnoiut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gopupdgxj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gvuclspnn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gmllzpuqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/glmvuysac.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gffilzfyz.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gstbwgqjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/ghmgxvsqc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gnqghsugd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/geaofwvam.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gzdizhfri.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/goaqugmqk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/grmihvhhb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/galkpqhrg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gfrxridga.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gygmafdkl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gtlfewetc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gmozjthrs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gsqrczuxn.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ggyrsxsmk.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gvawzvkvs.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gjmvebdgs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gxiulittx.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjbvkrurp.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gcqpnotcd.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gersvwhiv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gatmjxwcy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gmabqqcwj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gizwkeaxz.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gkibjrfgc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/garowqktk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gjdvptbxx.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gqiglgtbz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gfqnumeaw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gllzydite.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/ghemdbwhg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gzbmgnpgd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gcsmewmgo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gcziwlknd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gryktwlua.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gqazaexme.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghaihjuno.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gdfjlfbbs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gujsvpwjr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbtpbsoej.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gvvysjfku.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gldydjngl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxvbipwhn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gonyixofv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/ghioltnan.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gbhfhkgbz.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gfnmqcjpx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gxmykxlrz.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/ghorsujwx.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmnihrcid.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gzwcjewar.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gbekrggpc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gafpbpdcd.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghxmkmboj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gmiamtkih.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gpphhfbkp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gomudgtfj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gufqijcwg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmuotwnmt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gpndyomdo.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gltitshlm.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/ghidfglhy.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/ganbhdsqz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gmzrvuwvg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gjuvyqcse.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gwglipydd.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gfhgzpcaf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gxhphjzes.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gwjiiexke.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/ggcygxvbh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gybgnzvvq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gqrrjtklz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/girleknwl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfwzrplkz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/ggvenqbje.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyclwrkxj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ghpwstuct.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gavximlkx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gsfblxpfe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gevjtotkp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/ghrfgebry.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gkzucwnjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gxwrccjah.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gbuyimxbu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/giituyhiu.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gpaqdsoyg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gjdvupnsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwuhfilsv.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmrhjimyz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyibxfrrc.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gfkgpuzpv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggitidjgb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gjolknamt.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gornupafy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gttmhnfat.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gncnnzjje.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjpynhwyq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gwbhwklrw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gegujwtbz.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gcskrzmxt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/ghflpnujj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gtcnehytn.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggrzfhnjn.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/ggkwxamul.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpbrgpqmp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaofhhpxx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gzqztutkz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gubjmhtai.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/girszmizt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gcwnyqoni.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/ggggkcfoq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gjiwxuere.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gkliljuvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmmnswcik.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gguqryhlp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gzyzfnmro.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gaxfkfgkl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/grmummphl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gqzgjvyyc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsnngyttk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwqnnwbvq.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/galjublzp.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gdtordfto.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gfebsxpyk.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gphcddqgq.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpnspvigr.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/guelomzme.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxyacyozl.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/givphevif.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gjilpdpfr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gynixmhkg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gxcnxkfpp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gfhftkchq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvxkedhdy.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbezvjlva.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/geokmxdoh.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gwvfwoxxc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjmzeutgs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guhrtehph.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gietspvem.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyyebqp.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/ggkhzcclq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gsiswowqo.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gfzailhcg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gjnmrttra.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gtwclrugy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gsfvuxctm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtwevwcbv.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gscieaxgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/guparawea.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gcmxdfyff.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gxzdwdmaq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gnfhodnss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdnuiqqjy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gtmhxjfre.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gnwpaaghm.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gdipbggkn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/giuxuhpvz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gfzvjzkdy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gxkdijtsz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghajscqkp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gccnaunuk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/geqiswibb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/ggrnykdmo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gvehscawz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gdcmmhgcg.sHtML


<!-- 参考信息 -->