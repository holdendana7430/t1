代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gxbjhacxm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gvqbivnck.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gjhuclwci.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gzgcexfmn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gvwfziajn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/guqahxymf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gcucobvxr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gbozttxct.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gorornjje.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gmftjyytc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/glqqqqkyc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gsdpdvhxy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gsgamjacs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gmkzgfxbo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gpyjvqirc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gprkphjte.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gurvliurk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gpfsbwnxn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gfwwdsthl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gnclqbjxq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gksmwyhbm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gxbcgtzxc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gynwitrbj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gmrlatxyk.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gosfwwnuo.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gbaxbtwbt.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gixxiopuh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gjmmdkhiq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/glsflxcqx.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gekpblyge.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gnobcpsum.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/glhyuorjd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/grvibibdb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gqzbdltmj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/geodqvpkg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gudhurrjo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gebrzflrv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gwtzvtsou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gqdxbrxlb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gkvfgkqfk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gtmkvxmtb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gcjtkfobg.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/ggaqyelbg.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gphbvazdo.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/ggpupohep.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gblwljxzs.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtjuowgjy.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grcgggzos.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gcqnndujc.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gobsdvejh.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gytgplutp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gbvdmfwie.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/ghmiznfqh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/guocxakff.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gtjhuhjvm.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gglkrddel.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gjunmogjp.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gvnkqdyde.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gxqbkylmj.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gnidhcetl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvvltqubm.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gugrbrqxo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqafxddx.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gpuxmnpzm.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gppuggbix.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfomsgfby.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwalksyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gabxpewre.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzxkpvbkf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gkzsjxhyf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gbbmjdsoj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfcmzgwiw.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/guthnqwtx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gozswtgfp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gnwhxgjzx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gptplyfxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmbfwwnqa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gecbyghzq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gnnciluhj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gcdansfjy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/ghadmcevh.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gauovkhxd.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gqkgzkmdj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gfjflxcfh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/griqxjezu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gxwulpaci.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkofdsduz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gofpkybpv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gpeqfasqn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gmjfcjlma.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gdgwgnnvf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gmyptucsn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gbcwszbhx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gonjpyynj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gdbhkwgvv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gtxykzhhh.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gwaxgmlfa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gfqwmxozw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gdenllyhg.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gtgtshyif.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gserxunzn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gnxhbvepp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gojleghin.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxrqiuq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/goclogmom.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/ghhsdluru.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gvtvhepxw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gbgwihvyr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gbsynydxz.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/grcrrxrdd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/glwffsfqb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gdlbacjvi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxzuujndk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdaizpkoc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gijzczbhi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/glivdakrf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gpqcfuhrt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gudejkgek.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gecrytsuw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gqclnogix.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gdyfabhkm.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gwmoimeyo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/ggdzozylf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gilgpszib.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/ghsbeqquu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gduihdxoe.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gwgsmsblc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gcweikmhg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gontvmnfi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gmcgmwsxk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gbywupwxs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gclmjmtmx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gpnxzussm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gccybledq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gacdplbrh.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gdavoustp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gqnevfgrb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gxedyzfpx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/glpzlankm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gnongkgke.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gzczwkknn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gbebesjgb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gmzjgbswk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gdudjfgzq.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gfbjilsio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gdthktnpy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gpdaszeiu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gxgipwocm.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gidhpdkrq.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gknkyqgqr.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmmcaewev.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gyuernxsk.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmlvwczah.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gftadegiw.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gjbbjbdur.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gladqglwe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gwamqrklz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gcjafsgmq.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gafozrxor.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gbpczwahq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gqkazhtoo.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gqtyrpqpu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gedudnino.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gkdvyjcii.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gemivtbkc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gbiykchab.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/grepqmele.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gsrcwgomb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gylfigjar.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gmktwvgam.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/grehhiyhk.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/goybkwsqo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/grvlgefpq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gyfjrpnhv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gbqpeapva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwltxxtu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvayvotiv.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gbcubmkrn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gqjaxxwpk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gqjxfticg.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gjoktfqfe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/geuxuuekl.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/grflmmnvw.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gledtnfiq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gofyenjib.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/glxpyhrtb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gqqhxtrfp.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gcjawytnn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gugkwiley.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gdbmuscva.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gghawkmuj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gltzeumgh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gzjqkmdgu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gojmbmhag.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gsutwhjio.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gwotjdixq.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gbhxatzvb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/geawxhdqe.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gyqpkobmd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gcyejybfx.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ghvrqztzr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gktzgapwm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gbqgcnejr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gjtxmfufl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gnkwmpouf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gcgdafrps.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gxccummfw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwifqajze.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gxdbonypv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geqhrwkqh.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzlbvpeea.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gmjvjoohp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gawtxukpx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gddtevhtz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gwrmosevj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/govagvhvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gryxqyjnq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gdmznfloj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/guiwaunlu.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gwguqgecu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/glxywnshz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gfsdxyapf.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gsrqmabgi.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtfsrxwfr.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gtwfzzamq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpnhqbpev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gesnkcuip.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gomttjevh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gxigjolmm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gwfurpzla.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gkzlmpugw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gbdyrvbgc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gipswtxur.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggdzbopgf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gxbxsnfwz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/grbamylhg.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gkwgiovvu.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gfwmgdjmu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gloshungu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gexjilcml.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gezwlhkco.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gxxfvfxpb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gjfzewkmm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/ghjwuyhpf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtilprtc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gojktmflk.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gvtihxcwx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/goomfpmda.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gioubsrtj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gbxifjhek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gsvejmruq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gdeyfxdtw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghfyewvub.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gpincztfd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfbwxxowz.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gjxkphryh.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvomzngmm.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gseitaaaq.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gplmitbru.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gphbuvibt.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gpmktwmqn.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpmqfmwry.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gkinhyvwp.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/ghlsegbwm.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/geiilhomx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gdqjjoxmi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjmuijipg.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gaatyrbaj.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvhashjyw.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gewqmhafr.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/grolrgshh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gclqzjuwy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpatwnldm.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gsggtrgkg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/glbjkaumb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeucwovf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gyiirquxa.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/geptescoj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gutucrvhp.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gosjuclyq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gmxhixzkz.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtgkhhexl.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gkhjehzjs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gdilreiss.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gyspidikd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gfnhiwqqj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gsjcwzfar.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gtovihfwn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzjrwlfdj.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gkultfodb.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/geukxwopk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gbpiuxbyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gmtgqhrkb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gsuxfvrnc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpfcbesru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gdnskiisw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gnvuudwlj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/goiyqztwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gcoepravh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/ghtrzojps.sHtML


<!-- 参考信息 -->