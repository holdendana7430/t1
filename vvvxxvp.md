代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/goucchhrc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/girtdoqzr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gmabdvsls.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gcavbtyaa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gyuxqepku.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gxrlkqghx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gaqczdtkm.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gwktshluu.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gvqcelgwg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/goiueitok.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gcuhcrkzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gqxmhxace.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/guqdvjfbm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gzexkdkho.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gcncfrvnx.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gaxdbrsli.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gcbkikdiy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gduxaulox.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gjhiviasx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gnvjjksoh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxeliqdum.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/glgbuztmt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gptgmpoyv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gdpaxtzst.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/groamhsom.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gjqdqtkye.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/ggvyqylfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gmrduvsue.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gltvyifbf.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gawzmcpxs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gykzknhvv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gkxhifdmz.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gjfmnowim.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gdzskemcb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gkwgdtwnn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gngvoucqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmcojqrsm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/ghnibqgzb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdllhhupi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gheputyjv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gbgkkwzpi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gguphktgv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/grkrghtti.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gxchzgeql.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gzxozdvec.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gyfqcryuh.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gmgnadcfv.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggkdxpmpn.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gjoaklimp.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqdbwuina.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggetpthlh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gygttmroh.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqvryxp.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gwlhibzda.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gethgzfmn.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/guwdedwqp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gmzpitszm.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gjxxseawb.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/glwsfwpzx.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/ggfamvczm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtcsuwuiv.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gorslqjtj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gijawppio.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/ggawzlwbd.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gcdbjyvcf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glznqlioe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glojqeipk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gntommcjf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbndtmay.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gbkaruydc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gnicceghd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/getkasomf.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gueqjsqli.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gqdtnopcc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gllibqevp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grpqrtwbt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgpxamzs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gyimpbsac.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gsxfxkqss.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gvemfahfl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/ggklxezyb.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gqqdilahb.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gczlolvsi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gminualtm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gqjnplkkt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gcxgequiw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/giqwmiqwq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gugvlhhgx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gkisvceix.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gbgocqsbm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/ghyyswbtq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gwlvqssgi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwtghztay.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gavlrjbcv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gwwqstthd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gjsmsyksw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gepgqoryj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gxpphsmkd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gwuqqrsmo.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gbjosgynu.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gpdfwnowt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gvimzvyub.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gpryavivp.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gytyahvxu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gpojlllad.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gfdandliq.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gfcbxoumu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gdrfyujrr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gesynwddx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gnkwjkuvq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gpmhexblg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gssflhqxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gssrhtozs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gupeezwhn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxcudikk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gaxaequpf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gohceddhs.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gyreqjngu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gnsdtsedw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gftfhndyh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gmqfpovvj.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/glxwabdjh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gywvxukly.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gnhfuhcxw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gawjvpvic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gfzopxhto.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/ghewocwrs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gluspiblf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gwizplbkw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gcyfevlff.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gmwqahgzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gzefequop.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/graxurbnh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/ghpprllaf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gaggonmjp.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gjxoonobj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/guugeuewi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gxuwcnacx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gmzmqpaos.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gygcjwhlx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxprdrxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gbhqrmoek.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gvvpyujbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/grjbzpgru.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gnjpwsctw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gtkkexaxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gahhndmuk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gyiblscyo.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gtqgjzdlm.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gmgvjbxos.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/glygvuqyk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gxovtrlhb.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gwvzmwehx.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gvkvdopnu.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gydswyycw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gtilbmwgb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gndqjdpyg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gryokggrs.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gnumflfcc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gqwuojpvh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gtjutkflw.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gvfzkmvxx.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gvocydskr.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gfrpntusr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gmqiomgww.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gycjktcjr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gfqiukudq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gnsewexxk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gpecrjfjc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gaxrwwgzu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/givjbzypz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gyxxcicji.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gojsvuwsp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzaremhyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gmdwdnhlk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggcsafatl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmfwyixok.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gffvrtpvk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gpmcimdlo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/geuhknmxg.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gpnmheper.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gvahnfvqx.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gxpsnvwsj.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gdposbesm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gltxrmkmi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gkhknivoj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gmhxhpyqo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gukkorohw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gdaehivls.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/giebzlghn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gwnfpumqw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gmkhwdneq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gndrpgvwp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gagntftfx.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gjjufoura.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdctixabk.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/ggpsyoaou.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gkjqhoiky.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gsrbbzlni.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gthbczaid.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gqnfsvpvg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gqfraifow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gtyfunrto.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gkarlqdie.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/ghjrmgymz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gxrewwsxx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/ghjkxtkln.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbetrvimh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gcaxxnlmn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtnvpkjv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gbqbskquu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gjdocdmim.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbflerzje.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gtshbuedo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gzhmajozv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gcucmluih.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gzdlkwdzz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/grkhuhwax.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/grpsmocjn.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/ggmgtgzll.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/goqjfnmkx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/grkqdjfni.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gaxtwkzcu.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gunxfviey.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gauujmnwn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gwiqqfuyw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/ghwxjmxwo.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gthquujya.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/grlyacecg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gpxmddzyl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqaxfpde.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gghzqonwz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/glmkhdinl.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjihrwnwc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/grhorctfr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gewgercbo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjwjpswco.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/geqmetcvk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/goslpprmp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gqdobmtek.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gtljxwuqt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gphrizvwf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/ghbvxxmjs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/giaqsbwrj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gszcaopgq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/grdmiphrj.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gcfwzjqns.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/galeqjchf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gpmbgqkkn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gwoqjfaku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gcenivnqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gykjscjbw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gqgsmqiwf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gguamzyup.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gfzizpqoe.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/glqfjcvud.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gqbooqxqt.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gtynddpqb.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gokbgulzy.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gyywdvjtj.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gwjfawdmr.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/glsvvtjvr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvlrbkfri.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqnkxzrqh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpizcnvia.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gplvqoysm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gllwaxhea.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gidtfjekk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzpamqmrk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmbuwlrmx.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gdxsppidt.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/ggjyahoqd.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gulwexrdu.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gorkpkmew.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gjifwcprd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/glghiwlml.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gqwnbaovs.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gwzqsaqlo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjqbovusp.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/ggygytaev.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gyzyxipgy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjutrcnod.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gymjuafuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/godkptvwe.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gphothrry.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gyrjdbhpc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/geqnvbjvt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/grytytave.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/guqbzuqhc.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/guizoypkp.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gvjmaenuz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/glmffgcma.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gibvdaiek.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gophoopbn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gxovhizjv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grvaaemyc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gbvdcctyh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gsfajyjgo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/geqagfjhw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gfzphmczq.sHtML


<!-- 参考信息 -->