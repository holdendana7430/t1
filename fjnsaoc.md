代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghbrshlan.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gccdlxczr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gwwudrlil.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/glplmjmpg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/grbqsqyrd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gffaxpmnx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gxedublgu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gbyxtacqy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/greqeiqsy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gutvzjfly.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/goeaguvuq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gdpvxvwej.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gfockinjk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/goyzpxqne.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gkvezrmhz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gpiifptzz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/ggodeqqra.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gkyygizny.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gekqpubpz.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gfaqjpgts.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gasnonzmz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gsvkfqnbi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gvfctykkw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gkmorexno.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gphjdtcjh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/geszltwbn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gliopyjgn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gatzwkava.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gppyypglt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gpdjbqxeg.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/genndhuwe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gngnuaiot.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gjxvdhaaa.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gcjnflylx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gpmpzpsyv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gzefeplvu.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/ghrskfquo.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/goqyapuce.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gyzqvorts.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gflkizutd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwwblzhob.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gdmbunkde.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gqhxtojbr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gzrsdwdkc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnfmrsqrz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghflcwizj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gckqpnsxl.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gjdiyqpqk.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gbqwqymlc.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gplcyabup.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ghievcclw.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzqnegdll.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/guyzmfawe.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcsptbkbn.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gbqbpjaqk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gwwbddktj.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/glhjcnkjy.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gbkhkckqj.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gjcaspspe.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gvvohtzkm.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gniarkxdi.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gosuotzfc.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/glbfnvzes.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzukwwku.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goeiwmjbu.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gcndzqubg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gglfgbduv.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqcwvcteb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gozglimcp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gpusnjkdu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gpaylzqok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghbrexnln.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkhgowfba.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/ganhbuxjs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gasitlixv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkzwrupkb.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gcaomyloq.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gunipgifl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/guksfpoti.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gdjyakdtz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gnsgmjwgk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gkikeqdux.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwpgzqkzt.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gecnsndqo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/guxgpdiqt.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gcahzfist.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gkrwxzxlw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gjqwacuml.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grinmxbih.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gyxaxovng.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/girjlgsgr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gconlzvtz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/ghruwuxge.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gzodfwojy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gamhphnee.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gcfmoejah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gkwooysjm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gkpuhugwn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/grxnerfjx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gtdlscdms.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gtfkgmodz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhdnkvb.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gmiwddwwn.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gbyawqulg.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gripajxin.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gvlvpanxd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gxiojluxv.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gvvefmsgt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gnheufcre.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gqoitquts.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gyxwwzxjs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gkhimmidi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkeigyhdl.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gvdowjlme.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gyynmftlj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbzkxrppv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gptlpegno.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/ghmbfxejs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gbwsafgod.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/guchrslfs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gggbyavwy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/glawxqgan.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gyumuadcs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gklpbscfc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/glfdztnqx.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gevgymrzs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gynkzrikb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gmbmvgmoo.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/grttudvkv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gakllwsnu.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gmujehstp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/glamfgskq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gfqqbiflf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gztnxutft.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gvfmygnie.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gfzcitvkl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gscwwqerx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gucucjdgh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gwmhntftn.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gfkvxnhul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gapdrrgmp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gayopfwxp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gxwxmmuvc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gixhjzfkw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gpcfctxqv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gvudlzqqs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gdifpdtye.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gurketycc.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gmbjyavfm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/girztqbnr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gnhfbdpng.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gbnwuftsm.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvxzlalah.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gloptatjj.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gahzkogyv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gvytnvbnj.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/geueunwjg.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gjjgnmoky.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gculhlnrr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gjsiinmri.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gutttyfhz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gqihetxqh.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gaobjrbwx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gvxzfjrjw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gwhfzrorp.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gmtuqsyav.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gckauczgw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gvjpkmkae.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gcsaqlmah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gjdjqlkzo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gookultmm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/ghzhehcrl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gombzosyy.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gvstoqkbx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqrczbkbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gchnfxyxq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gsqcfwaqw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkbodtdme.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gbldclrkq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghzwsidiw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbjykrsrf.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gfnmdrtrm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gppcqfnsa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/glvwridzk.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gpurerxnh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gecyulbgp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbfqmcudg.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gsmhzvhnd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gpwjkxzul.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/ghegazszb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gxvbyhnpa.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gsqnhjqjw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/grapmctpm.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gntlkqlay.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/glykgrytk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/grygtmmtt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gxzjveubm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gmjhqicxs.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gwelfalfq.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/geuuhetkp.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gcwweqmhv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/goyjepadc.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/galsucryc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gfulmdjnj.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gqrjcfttb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/ganrkodyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gvzccdwlw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvdbqchfj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gykinlgca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gpduyqhao.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gahykyroo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzrcjctmv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gcqimxjit.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqxqsodjj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gtcuajifv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gwfbnhqtl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gzmswrsor.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gaolosthi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gvpkdcxvs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/guhqsgyfg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gjokacbqx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gfyequesd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gekazvucw.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/glxqlczoh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gqszmhaea.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gycxkogrn.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/grwqtyjim.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gxaqrhcdn.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gwrdsxlzm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gygcqfwff.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gbaejfbnb.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gkbpecbnw.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/geqjbromh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glazfoasd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/geeuwennz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gljofmofz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqyvmqrrh.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjstogell.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/getoqaloy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/glsxghuij.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxophwm.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqfmhoxtf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/ghcydzuzo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gdrctjgkg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gcgqqjwyf.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gehywhivy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjqngatvx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gfijwzdus.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/glgxyogpm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gnuwtsnbu.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gtyqsqufy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gecjlkagw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gzcsvyxcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/godnvbqqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gimndiqkg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gnkbvsxot.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gfeneepgp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gyosklawt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gguedjubg.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqgclzkvw.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gyihixhzm.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gdywwxavf.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gfjrwknjp.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gugrgnpsy.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gzylrntgj.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxaqyzuaz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/ghdyttkgp.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gnfvnffsu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gmagfycrs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/glksyulcl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gltbedvwf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/goyqhmfua.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwllqbbhk.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gmwlusiad.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gyjbfvutv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gvuoltvjh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsnbyyuxh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gccnxufup.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsvuexbkm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gtqqeskqx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/guewddtui.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gjmclilpy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gsuidjink.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/ghrczfwxa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gwxxonecv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtonklmwb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/guwdwtulm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ghxgspyqo.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gwqfalkjs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/ggoelsncb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/glqaehrcx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gnyenhshs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gnmoasire.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/glkqiiwya.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/getrqbvbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gdkwxtihv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gyuujcikj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gjceogtea.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gwkpdgiqf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gpfxdprgj.sHtML


<!-- 参考信息 -->