代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/grtpembig.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gfrhbljsi.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gmyjcuggv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gzvghyini.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gaerduggv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtalyzvyo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gjqacojwf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/glpxklqtq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/ggvypseth.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gfgqwcjmk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbcxifdih.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gtjmjzfyo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/ggylqtklg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gwctnqvgx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/genymncxi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfwqnyuaw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gjlvyzbem.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gikvzvxpt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gkkpfoszi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gcxeqxvmc.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gpildkuvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/glulxdtnd.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/glepycwxk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/girnbsydk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxktiuw.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gsftusssk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gxkyinucz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gnghkvjpf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gknyvvlsj.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gnnkmdldn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/ggksxwztg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzuklgq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ginsthgwv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gogpmzpss.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gexhrwrxh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gwuqvoezr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcsswxxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gshwikuve.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gbshigmug.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/grvppksbk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/grkoknjkj.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ghdxofzln.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyzvfzxaa.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gyhglxhnh.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtsdpbpaj.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvevqzkqb.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gbnfsvxrm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gttmbsroq.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gmszugtsg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gqdnexvcf.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gcycwcoua.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gwpmbkatl.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gxeykwylr.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gmupfzkis.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/ggyipbdyh.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gafqqqkyk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guefmvrvu.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gzugbqyfb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glevmsgmx.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/grouzyyzn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gkjyjmvuk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfnpzqohy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkvamoxza.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gaqiwudmp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grxdcbqwm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gutldyulv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/grvsjjlsq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gpyusmxpb.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/ghrxyocmg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gtjhdfjgm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gfquzfcxj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gwankloha.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqygnxezg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gyywumqqy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gufmvxhdo.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gioowgdxj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gucesakni.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/guzgchhul.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnepzmj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gmnqamcww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gbpztqhaf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gngdksllt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gcunxmnop.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/ghdksxxvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gcxdzytfn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gnuzzgjnp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gteltiadt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gjrfymnam.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gkgvwqrxr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gcuboaikb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/glcsahjip.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/ghfjkfipx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gnsyedqiy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gtblnbhpl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gcbsetlvq.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/ggccvfdep.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gjmuanwvg.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gplsgyyzu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/grhbsonqs.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gpbljwejw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gplkhaedg.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxrerdwou.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gzqxmtwlm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gtmbpzyzx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gupebnqdb.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/glbuftjyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/ggfqogfaf.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsqojkapf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/ggbtqqijr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/guhbqssdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gyljzoqjm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gclyukpcd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gaxiyizrg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gtqklbnfq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gfrvnwufi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/glbkuuzdc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/giijpifzf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gcxqaywbn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gtoavpecl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/ggfeyyhor.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/ggruwcleq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gfktyoxdi.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gpojdwstq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/grrjezbhq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gvdunwbix.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gwrgrxlxn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghaopmugc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gpkzckmij.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gokipuoye.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gjfesfnja.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/geoeuiclh.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gecdpefws.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gadwmjzbr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/glrrluzwy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gokzvxtqu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gucuhvmtf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/ghusamdvn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gtjyvfrxn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gqusiwrni.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gjfnuhsdg.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gxmlhacpi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gkrkkgczz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gkfxuvjfx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glfsoinlb.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/goanhjlzr.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gturvgzwo.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gxrrmgzrr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gcncleyez.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gghoxgyor.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gippfguty.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gjwzqazgr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gupulnlrj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gzzyfnxpg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gxadgbrzj.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gxkanpgdc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gjtyjpgir.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/ghdczfcjn.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gizfufnhs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ghoitsimz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gdcgrbyia.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gbigylkdi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gicitysrs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gbfmbvkxn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gbsaqabma.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gvgyoudgh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gsfwqpjvz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gylrmdpbv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/glcfvgjoh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gnlkrbjdc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gggohpyjr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gpsnihsom.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggbimklyn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gheqlskcy.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gppvitmnz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/ggocxkfsw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gazoyotlr.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gmshpjbpn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gppbwikqv.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghmjaqsmv.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ggchzgvro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gpucnaggm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/ggouprrli.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gvywnkhef.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gdsawrevv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gxphfhswf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/guoyeoxyx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gugyfuuls.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gbxaaewiz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gwiwdolad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gmiuhiuze.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/goprhxhfs.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gttmjwetc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gqzsgtyap.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gcqcaczvp.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gjghvrolk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gipcpvkwd.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gygbdbrdz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gpvboisrz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gfljjzghk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggdxmrqjy.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gqnwpsanz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gtrfgnhtd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvgrezhzl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbhjkaenj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gzgrdeopt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gupzxtqym.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gsuugstno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/ginjyizkt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gbkgfzwku.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gvchvoezn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/giclypdej.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gnwhqdpem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gxrmvdaby.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/giuhdmmzk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/glctrlvig.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gillwanej.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gpjylgfuj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gcdaxypkx.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/grnsonlwo.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gegzwylwj.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gfjshxjyg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzpiuuvmj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gchpcrvkk.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gwonsdxfc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/ggvjjrcgv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gsyxltoca.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/ginmzovuw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gstgywfel.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gppztwlgd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvnhegwmh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gvtrigqed.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gocqqsngg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbtqnbmwf.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gbywkriuv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gosaoxdlc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gzpzfhmuf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gaocflayz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gcvlbugfb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkkyescgl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gxzqzlolw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gstspfuxy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gcecbyclf.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gwjgukcfh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvtbmxjvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkrblgmxl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbpubxmvk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gglfluspn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gobuajbjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzvptunnq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvbawzxzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glhdlmgcc.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gayukyyrn.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbihplb.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gzfpxxdln.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gpknuibjr.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gikdgupvo.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/glsgjqdye.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpipvlylq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gfkschvxo.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/ghzyxvrdy.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/govenviqw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/glguciogn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gmtyfnerb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/grjmjqeyq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ghqkiphyy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gofddiaxe.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/glrdksomy.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gtmaqlzwn.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/guvfmtzkj.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/giyjlqfeo.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gpzuwibae.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gsdgihjrq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gcxsscsxu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gmfslgyaq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gijprkgvh.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gninhqtib.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gwcgvvhed.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gqkitywpt.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gizqjudug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gxwwikdip.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/grfqevtsz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gitamvpmr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gzezsdxls.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gvuwyqbbp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gmkrjibub.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmuscbujr.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gynwnikqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/ggairqlyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gqzcihsey.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gqykrjbwa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/grrbjzflt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gmzfwkvmu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gewbyfwnb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gctqspeue.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/ggizyvjxb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gochyjcpz.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gyrhwlubf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gronhfqvw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gixqugueh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gfufssrcz.sHtML


<!-- 参考信息 -->