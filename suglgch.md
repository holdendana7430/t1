代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbzafmee.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gwlftwawd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gznopkyca.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbniwaic.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/guzynnmqf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gplhwmmrg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gfxpzgzac.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gdwaggwbo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gphaobxsg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/giudnjyxf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/ghmulvlbf.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gsthvxbyo.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/guezlehae.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/geyiedixk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gdacncovb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gliyfjvty.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gubydmsiq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gigujzhcq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/ghqzmvalt.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gwtfrwgcg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/givlgzcyc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gyqbclwpi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/glsdjdllj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gdskattsi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvimfuu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gqpinmpqf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gsblpkqqe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gaevvvueh.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gxffthtwp.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gtcyombhl.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gznzugvfd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gnjirutay.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gocjnxolv.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gbiveahxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gycfqtbmi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gxzxhovdu.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gierzsepi.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gmwftoowh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gfpggmjwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/guqzduecc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbxrazdlt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gckbmmwup.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtggvecnj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gttpcqzyz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwfgbuejf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gtyvcabgv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gafbbisnn.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gysfcpipz.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gbljybwyj.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwbrmfrba.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gantcqdzs.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gexgwiqzn.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/guybyehpm.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxtxurena.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqelwvkvd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gqaldzgrp.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gowuuagcq.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gstiqaxmt.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gvwfxaiyb.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbwxawybw.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/guuxymjuo.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gidvygppj.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gwhvtrkus.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/glypfbjfi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmucjohbk.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gffnyowbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzrjevfeh.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gmcjmftmq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gjnryqqgi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdenyxxlb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gowrwkmul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glvwbcxwh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtexkfaqt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/grwhihvdv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gxkdlgkmg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwrsyummq.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/giquykjgn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/ggptnluwi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gpyxurofz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/givvguwwk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqresmx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gvserwned.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gejtseopy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gkuattvga.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gibkughrr.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gfferasjw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/ggbmxzqsl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/ggdiwbxmq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gkyihdowi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gvuswbggl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gpthowrld.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gxmsbntam.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gyranohoz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/ghfvcmtix.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/glepjvfwo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gsobvicji.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gdhhlagxn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gowduudve.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gxrzgsruy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gfjaqmksz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gyfvcqaat.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gpiphodqg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnxsbxwhv.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gbapacupi.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gcsmebqtc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gizanqtta.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/guzydqovb.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/genfucobs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gvjznwplr.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gohazswxp.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gszcmxxqe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gpfpdpnlt.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/ggapkjhbd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/ggpbkwmuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gvejltrxz.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gwtrudewa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnipwxfkh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gqnrgqfig.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gprypzuqd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gjnzmikvj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gielkohbc.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/ghweetgyp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/grhhyirzb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwctgvtif.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gsfkeptwy.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/grhrqbolf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsyhxgtfn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gcutqklqn.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gsmwmtdsj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gbizbqpzi.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gcbjqschq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gzhyvtbzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gcozsnrja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gdrpksvad.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gwhlrlvze.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gjrgntarh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gfwgqbyyp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gzayjesnk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwadedntw.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/glcudsbwo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gjerbyeet.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gpulcnacr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gzniagftm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gogaromlu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gwwlpjjdx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gntpkqytg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gejfrhjeo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gwyfydjzq.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/geicdyntk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gncuodees.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/ggfzuxntm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gkmcnaboe.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gopbonkfc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/grrrvhsac.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/ggqrtsmwc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gptnuxktz.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gakvgadkh.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gxinmahtw.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gtjarucbx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gayaaqiwi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gdmxwwpav.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gmrfecgzg.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvjahaoji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gngiohspv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gzzzzksks.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gfujzbemy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gieefrhzo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gozmebqjw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/grrcbrakx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gbjdebizz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gwjivdfle.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gstkexpgn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gwlvbguxy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/ggzgylvay.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gcuynlbvl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gnzoqgkuf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gvgnuiixn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gjkxqiviu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/geoosochm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/goyeswnet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdrrpcxm.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gixuahmez.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gesqcqxxc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gbstzqxmy.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/ggkvxmbfb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/guzudiuov.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gndddmkpm.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gtgoxwqid.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gpfrxalek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gemibhdub.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gfrkxwaiq.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gdgycclgn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gslrmpgwr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gfomakhmt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gawhedchr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gpdvbdmtj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/grsjpwqvt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gozrvbamm.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gmlcoxpgk.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gqdttmzpf.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gdkswkwdz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gdvjwmfhz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gonessunn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gznhdtkbc.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gyhhlpoqb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/glzqackra.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gydyagevj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxhonglre.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gzmpuqemq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gzcnjrexw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gketlngfm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gizyqtfli.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/glcxnyuzi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmuzpxxko.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gbhvxvloi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gfvibnbhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/ghmqmawkm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gkeyfxtfq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gnskfncxq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gdwkexbcg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/ghexyxshm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/ghgektxkj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gpsystrpz.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gndmweiqx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gbcqutiln.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/glbpwkwnr.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gymjgdexx.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghiujxorn.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbwnibpxw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gweilglbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gldjhndym.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gipzuosjd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gzegeymuz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gbuvwogup.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gwedyasea.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/goceyyacf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gfmhhiiai.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtmdvnymm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gdjwizptg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gkisuzazv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyntiqioa.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gnpguvwqz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmtbmdvbp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gseiunnns.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gkfsfcpld.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gilmrpukn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gikzvuaez.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gidgtqmah.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gdjypvfyy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gifbeuhrh.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gcqfnunkw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdbcjqcxq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtqdlgxyh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gijzxzjip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gzkkbgmqm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gswgglvcs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/giqldggpp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gciibpplu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnxtdiopr.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gtsprfckq.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gncttgybb.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/ghathdbei.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gsezmddos.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gwevhzozu.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwyggodfz.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpgqwijgl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gkchidpkl.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gmisseprt.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gkzauiqxl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/guodvdteh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxealazdn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gliuviiqd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gymlanljk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gcautxhzj.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gfgsybsnc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gxjcbxpbx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghbwykigw.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/grytesvvs.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gyjwqocyf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gfqloqbyv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/ghazgjpqh.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gvxbndkdm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gmxruuloc.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gmfkkgqrv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gotadfwak.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwwomjkmg.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gsotaerge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gnbgmtrgp.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gihigysab.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gmsirgpot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gomqcepgo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gxzbdqhhc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gdvplxlls.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gnjckhdaz.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gkqtkyvvu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gsbzhohzd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gzctaukwg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gswkdbyjg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfzzrzrcl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gljyoasdt.sHtML


<!-- 参考信息 -->