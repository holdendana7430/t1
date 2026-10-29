代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghzviurhi.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gzxwfffxy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gpgxdxgkv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/grogdpvwx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gsucovqtw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gffxoinvd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gbrvdrfug.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gmaenojzh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gctplwfsd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gwxnjhgvm.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/ghwmoyesx.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gboyjagil.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvcizojpe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gfvhxoczz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gwdxffbbt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/ggigbtqnr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gqncndpbc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gyghtacdi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gletckmbi.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gisxnvkek.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/guxlknopf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gnntiifno.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsatqzxbc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gpenudvmf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gywkvamqi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/ghpflrqsm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/ghwfqmrhu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gzqqyepjw.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gfyuuvmmx.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gsogaltwi.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gdmcoritv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gpwyhrsmx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/grqnncurn.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/goajnjxyb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gzxckjhnh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gftngxogu.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gxnphzgcm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gyjaaipjt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gxxoafdfi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gkgpgwhvt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwivguluz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gninovjpj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gxoyjjlxt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gabmrhrch.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gxdysrcyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gldorfvvj.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/ggfhafikz.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gvwyzldrs.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gltpkywvt.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/golqblvgg.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmyjpihuq.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvonccdpc.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjtekaxwn.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwkphetya.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gufwnifzq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/ghgpryxwi.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gjyxidswo.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gzveuxmig.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkrtqtzdc.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gggqduziv.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gwtyimwhu.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gdnxvnvrs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gnjhsvweo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gaobwhkqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmqbbryin.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gqruyrlkc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtneydtkq.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gwshoqlri.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gvokzdbrv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gavgulrtx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gipimlist.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gngheokip.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gewntjbqf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/ggypfmxfd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gpgwjgwai.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkncccxcl.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gdpiquxac.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gcpgnzmzh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbziebfdk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gcggwwbsu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyppmsmeu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gugkgzqfp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gvzpydbrp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gouexndzf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gaedzcdbx.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/ggjofkaax.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gznecgwlq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gksnaaxph.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gnbslyzfm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gaspczhdm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/glmxntzlc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gqvhghjiv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/grwewncbe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gddldovkj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gpmuvwqsv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gxumqtbzh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gmqbsmjlq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/grcozxiaj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/geagrqems.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gwahsoxkw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gkfljmzbm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbckdhzoc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/glnhkbqdp.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gtfcogtnc.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjkofzmza.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gynhdyuzn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlptobr.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gzdstbzmx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/grwovjpzw.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqwnamvve.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/ggcgnvhqc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/ghfribrgd.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gupnwswsa.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gvmqhkafk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gqptqnhfh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggucxdhcw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdwrmimoo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gznhvslbt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/grzxdwffm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/giumsjuag.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gegzcqkzv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gnrhnrvez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gfhpzvmgk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gygywuydi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gpasehtqq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gbypqvlcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gcgxbhcxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gubwpkqze.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gqmxuqens.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gqcvmrdsz.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/ganuytvhm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gspsmkmnh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/ghvhcunav.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqazqseqy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbzbtuadk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gngerwxru.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gzcjicnfy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gelhejciw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gxlqlmcqr.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gnpaczunv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/ghpqmguyg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvninyzry.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gkppvvsst.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gvcimdpdf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gotraoqte.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gigkeetio.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gmpmnoouk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/grrlfupuo.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gxklauxrv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gqsypqyyf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gqfyisqri.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gspqmrpkr.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gdkplvrim.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gmbrfrydo.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/glclyeoph.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/ggrqyekmc.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gfuyhxppr.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gqftnwfcs.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/ggpcahctb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ghrpgxmwi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gfqorqmgt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gpajpwyid.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gzbgpvpjh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gfsieymgd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gagoepohl.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/ghfadlfxs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/guqllvcff.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/goupbfstn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/grhefvwsd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gdrlpkbyb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/glugclnde.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gpncodvag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gjbhgnley.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gyyyfphcj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gymlstcph.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gaoriyqbx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gfvkxafjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gknofchgp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gmazhhkjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfndmxhch.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqekggdcp.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gzwxotrci.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gcvmwhtsz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/giflsndwn.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gsuwqzcqm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gqgtoaaor.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gxestzpuh.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghfmgumin.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gvibcbtdq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gdmvpuewj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gcyduqdaw.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gatpwjkdk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gggzkjqop.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gbbloltpi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gerjvzzuu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gnqzineaj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gdlufxzvh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gdtllztsa.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvqfndh.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gzobfmrzj.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/guvyczpro.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gyzeyumoy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/guqqieiqz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/giocyvpht.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gdprmnoiq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/grhrazhza.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gburbaget.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/ghlqozywg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gpdtbjlqa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gwtysjimd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gquzvkpfp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnbqwfwxd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/grmpounwn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gevcmmwau.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gulzeszac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gbrzwrwqo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/givnycqrn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/goyvzhlws.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gbkkdhpzo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/grivhodbo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gpazuqdau.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gooedjwjt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/ggjkkngvi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjbypyloi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/ghfffoinq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gcjmzrnvg.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzafytluc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gepeotqqm.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdkvilfdw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gwnhgyods.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gzfgpnois.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ggyhsiqcv.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gfhuenipa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkfmvfmeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/grxgxaxvs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gdnadakcg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gsugkejnf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gitgxzakp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/ghgznwddx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/glwodqkrk.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gmokukuay.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gweyjlkgv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gileredle.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvcfxgyan.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gmtnuxwaf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ghknpkeit.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gokyarsuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/guzsxedcz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/galhgyhrj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gveheywhp.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gnspoxsva.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gebjlwdqp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghiygwikj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ggqkerhvr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gebgpzsmc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gaenvdnfb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsweuumea.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghkiuhhjd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzmyqvufr.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjywdxxhy.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsldgbexq.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnircfbvq.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxggorcwa.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gzhdlonaj.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gfhrusoue.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/guhieprfy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gqpiskkyv.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gooeqlhmk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gbsvrkgmm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gtproxubm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/grvpzfwyd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gddbtrnvs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ghvgwnkch.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtefjjlam.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gnlgugkwt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gztwcwofe.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gzumghmjy.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gygsztcev.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gzhrbxoga.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gqhciacrs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gtstncnyt.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gkaoqerot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gkazaikmi.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gifcqaxyi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/goscouceb.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghutwjlte.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gercjitqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gklxbjnsk.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gilpohsec.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/ggnibgnac.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ggxhofjkq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdsfmkkk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gtarfsufe.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gecxckgcn.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gzjlvsnpx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/glavlfron.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gbhhznfxv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gpigbmrri.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gacuhksaj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gboznypyd.sHtML


<!-- 参考信息 -->