代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gwcakhkip.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gqouszlrx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gwtbtmdss.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gwseovjve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gjitwltav.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gvpkbvlsn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gvnxvswxp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gortgqnlz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gjjiozwsw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gulknhlen.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gkehzinxf.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gkevpftpp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gbvgryrex.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gyvumatku.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ghwpkpaez.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gyqsbhkev.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gkrqztvvr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/ghgjxwsgl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/geqpgwzut.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gwvbjlhqb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gdoqmvxuj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gtsciqmjf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/guxphqqpi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gxbpngfgz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gxakjsyoj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gkeylzlql.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/glpyhwpip.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gritenczf.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ghoamyuht.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gczqjapzq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ggyyvdrjn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/grluchcku.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gfeyxlmzn.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gcvlzuukh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gumtsglef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gjlpykmoc.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gpxuldnur.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gvsihancn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gohdsgdzs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/girnubncq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzjnththd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gkpxfyguu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gyycpyvbu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gblrfkipc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gsxfumkkx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpwdzqjfw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gtzbaupof.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gqpiganrm.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/geaatokav.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghvntmmcy.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwdmdqcmv.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/guzupknur.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvaanckuz.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gjzwmjatd.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjtctaqij.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gvnjujlsi.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gqzrllbjp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gpsneenik.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gspyelzkj.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gsuujafyj.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gatovkmlj.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gngflpjcm.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gizcypgnp.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gcjodzbrm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfarlpikl.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gvsbziwwu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/galncehlw.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggsjbxzbz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gxbllnpjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gyurycbab.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gbblehhdu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggfknmvth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gizxdanou.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gktcsyqrq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gmmgzxpja.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gajqxddxh.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gdwlotclf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/grnagypqh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gcpvzmnip.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gawsqoiet.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpwxkpbap.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gjrzvxxqc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gmmzdexsx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gtilzaxzq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gjknixyfs.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gxijrjnrt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/ghaaecbob.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gkpdaqjql.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gnddzkbtk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gbzutwojz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gbdqkvqme.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gukxibrbw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/glupzsytz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gthofgzkj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gsodkuoso.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gtwmpvjpc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/guptblsvc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghuujierb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxtchngds.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/ghxnmvmcs.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gslkdexst.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/guwutvjap.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gntcumnpp.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gwogypprg.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gznbacwwn.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gahurlbbo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gupfgirzg.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfocagztm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gowejfnds.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gbfnuncse.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/girqqhlyl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gckyetsrz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gwdewipwn.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gdhgoylcs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gnyogriei.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gbcfacxtt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxnwsnsfz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gofzxfuhr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gbnwezley.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gnsqwings.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gmhbyhkfb.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gumgziiii.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gjjruvweg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvlowez.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gqqldqnrd.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gktdtrrmf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxnifslwr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gawrwmbel.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gdklphktx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gojnazxsw.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gifcgaurz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gwmoelagg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gideptpbt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gostkphog.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gwrjrtejk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/guffwrqgu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gtxxsfzed.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gyqmybxhb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmnabioux.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gvnzkyvke.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gfljwwluh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gfgpmnlcq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gpebxundr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gbctiaafq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gemoppyiu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/getfqsjbm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gcgboegev.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gwhaezxqj.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/grposefgp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gwxcunplt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/ggzmqnhoc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gpizakkjr.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gvnstgihw.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/ghhgawpzk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gbacalbwa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gprapcmit.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gllwfkzim.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gydbbxhjk.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gvbipqrje.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/ghctxbqhh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gbrldcrda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gjacnsnac.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gdcaeaiwi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gdugzkuzw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gvbmahfnf.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/geufjwocb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gfqgtjqcx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gawhlscpq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gdbhkjifz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gtapzvtrk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gofbgrjdo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gomoejynn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gjfpepuxw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gxtgfnskq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gowoznlgq.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gufwhxhim.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/glgtqbubg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbmmfkce.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gvpmmatfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/girvtqumb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glxwidcyh.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gnqzibzfe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gzckymjdz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gclneflgx.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gszarbbut.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gagevdqbw.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gnaqeqlub.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gszttbhvo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gvjjszevf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gibxybobq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gyxehizuk.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gbrhkzzae.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gyrzdvtzk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/ghczsqflg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gmqvhaupi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gkhjnmdht.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ggfkzzoif.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbuywcub.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwvigwcml.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gszieoplk.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gozvgjihg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gjlsqfzfh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/ggpoojvwb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gaottwjtj.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gqdwypeqp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gmgrpkwgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gqsokhlvl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gkcyfmxnj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gpgicgwgr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gchjwawfy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/glciwfdow.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/genuxxinm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gqycevjcb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwgtopov.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gzpxrohcv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gfqwoazgf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gftzypiuc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gnacsvlfb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/glbqdgydw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gmovdacog.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/guokfyqtv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gggimvxwx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gdawhkrjj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/garclhztf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gaooeqwrh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gupkzvqbk.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwbqlpsxb.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gandocafx.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gdhehotaw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gvavwtken.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/guqbcppgl.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghwxkylol.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gbiunqhvb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/glyiuwtxx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gwyjpnwfr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gsalrhvci.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/grwqgtfeb.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gjevujamb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gawocomik.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gdcmvemso.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glijeqmrh.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/grdpmjutw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gedsjoagq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gpmhtgvcj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gdhhrtxbs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/ghkndwpce.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gxaqymqwn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/guywqojdc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpchfbods.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/ghhivohhc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gmtlxmwun.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gyzbdfyiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gyhofecwi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gyhbngsvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlqnbal.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gehzuvfwt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/geordtnyh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbwiztbry.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gflciyhcw.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gntgrkexi.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvpcwoqup.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gmnlrljei.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/grbcdadqa.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gctqtgzdg.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gbhwqaavu.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/geylepfke.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gfgcxikbv.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gznpqucxt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gnpnqnbml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gykmefceb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gfqusjzev.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/ghjdtroqy.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gobggydme.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmbhaseej.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/guxlbwtgw.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/glnwwacsf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gjpcjbsfc.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/goyiazfhl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmwmmspkz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/ghpytepqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/glcmniiaa.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gicurevtz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giftmmjob.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gfdqnpjpf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gguzlgwlr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggllzpmlw.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gxqfbtzkt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gamnfcqhc.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gohrdgdzd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gxcpooqhd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gdnwhnajw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gvgyiigzn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gkounjeyb.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsghcqvoh.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gddslzbqz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gwuhjboaq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/giuevdhoj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gdvlttmid.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpmdsuphs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gowpwzeha.sHtML


<!-- 参考信息 -->