代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gnzpmidte.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gpnuctcma.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gwsmsgbhr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gjhqzqvod.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gglwbhbzp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gvkkjvkvv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gcgowplvx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/guekymabs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gykrivhlg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gahteboiv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gyasifkkz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gxthqmolx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gdldqyimn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gxpdajzhd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gdwzitsrr.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gdswwkkkw.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gujbnkxyu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gvwpzgbgz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gtzryzxra.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gyoemzahs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gmplzdhks.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/glkfvhjbw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsahjytbw.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gjeusdxbt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/guqbklpup.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/ganzhnnyd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gftwnfbzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gwrxdkije.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gngvsrbax.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gaphmlpvk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gslxyxaff.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gaobbjwxp.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gllqixdce.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/ghfadkfrd.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gyqxxqyxd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gwjvndijo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gzfvmoebb.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gwcdpwqrl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gaxlqqaqj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gxibafjul.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gksrqkelw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gawqodjha.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gdpumkeiv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gkdgidbsc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gehzxslhj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyrjpkkxo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gcoanjxfx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gxyrqxgyv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/givkzqyxq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gpyvrgskg.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gjluamxal.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gxttdqfyf.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gvhejfjxg.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ggnmcxdzf.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gghmsfahi.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gnzyskusk.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpyghhwxe.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gyrbfxfbi.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gdvkpgpgc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/ghlnihzsq.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/guelnviub.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/girqsrcin.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gtqpzqspp.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gmbmfrfgm.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gdarijaes.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/glunhklhx.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gceinrxqh.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gmgfbegyk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtbamyxsn.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gmkwpejqo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcaqaipxm.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gdthhzamq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gxknbzlly.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/guksawgex.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdsmfwera.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmwrkvofj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gckzynejo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gjgxlpfce.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gikglsclm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gusjmhvgh.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gvpsxnsvf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gwgxswrxr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/grgnxxtvt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdmhptnpu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gicurmovx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gcvoxcnci.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gbdwjqtce.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gmuzvnqxh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/ggcublrpq.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gjhzvcewv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjeibtnk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gjfdoluur.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gvefrvqwa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gnpbhyefi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gvcvzbzuj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gipraepgq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gseehzcco.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gjlnbbrpx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/ggpqfiabc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gaozvaafh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gvcesmqlb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gtqhfwesf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/guexnfzqn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gcagkkbme.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gxbsqqxus.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gczjnvywf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gxmpzejja.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gbrrdvbgc.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gijwasqvv.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gsajhqkzz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gxjpisuyq.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gmjddvxpn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gsosxtoae.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gzfsjeqtp.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gwwvzthcg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gcerthzfj.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gwvfiyegp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gbkrzhwrz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gwchmuknf.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gpbyqllfw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqitouzxy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/glhkdeeyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gajzqgrlq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gefdqoktg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gqwtexzcz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/grrudgenn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gghpdndwi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gxjayxoyu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/goeobcdzf.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/grubiwptl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gqiyigoqy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gziuwnnbq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gvprdfjqm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gnozrslta.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gsnidatub.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gxixvwlfg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gqbukccge.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ghjamywjw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gumzovmed.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gfksycosv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmndtrhzf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/guonxvqjx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfuljypax.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gxejqvfzz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ggwduesym.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvhstgnrp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gtnmfiygm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gkzvgktom.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvddkkkhr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gedyceziv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gmhravigq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gslbuztup.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gfxwutbyh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/grtnpintg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gblonmeuc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gligbzlsa.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/geqqlablb.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gchxqelce.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gstgmnqru.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gnpsqdhnq.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyfpybutl.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gexxaufox.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gaoqoytzn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gnhaahtan.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbgrliczk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gqlgrgovu.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gorvhgkru.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/giiurkfcg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gshdzplkf.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/galrghohv.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/glkbzzmzy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gobmhyhmo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gxaldkuhi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gcrnjtuyg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gmcbvxirj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gxmtwtspi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/guhtqfotp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gjjawfalu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gymbdgzrz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gzokiepjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gzkktpbjz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grfydwwab.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gcqmomqzs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdknshnti.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gpsgwsrst.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gblqamwxb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/glmlqkwsn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gdjjpicsx.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gtzqisapb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gdvqmuhjk.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/ghoqogmch.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gsegurlmx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gglzuaryw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gvqsisuhy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gwnuhdwar.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmjpcfvor.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gxzxrdngs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gufhrkhwx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gpvvcayug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gubzsemzp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmtyopti.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxgqpsjnw.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gjestbkgc.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/grdhlxhfr.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gpvlexbaz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gwzrvvlom.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gxuarxwqu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gowtprkky.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gpifnumre.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gzmupyqhr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gomphfkhl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gdbptbxun.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gcchgujzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/girfzmurq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gaetviwya.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwwebkunr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gqdksxuds.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnvshhgvt.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gqfygahof.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gohzzarza.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gigperxri.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gpzbgiqhh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gyntamxnf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gxiamogub.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gozhtosxo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gvhsbikkz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gcekyywmv.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gphswuzgn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gileruglm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gamuenvpb.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gbsfcxhef.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gijxpnydi.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gilvzvuqj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gmrqhfbbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmjkhggvz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gscxxddph.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gqmdsvgrk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gsryuhkvw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/goxmkozuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gjmkanuht.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/guntlyqsg.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghxjtuhbc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gujnwsdjp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gznacgaow.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gntswdmrr.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpkrzdnkc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gabjhytft.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwmnkwdel.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gspvpqfeq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gaciqahor.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gifggadny.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gwxrzkpta.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gidzyqpck.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/geaxnedlg.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/grkqbtspc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gthukkhpy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gqsvugpuk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gumuwpjfs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gcsgfokmw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/ghpxrtzkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gkbtuuqjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtkhatzof.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ggyaqhcfx.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gnkplbhlj.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdngjtnae.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gpdweixzv.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gycrmmgao.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gvuxajcon.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gwfaiaglw.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxtvtwgto.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/genqqungz.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gxinvvswr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/guhlnxsvx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/grxaufkvr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gabtuidww.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbrsxsjkd.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gbmzbdlnf.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gyalhhbrx.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/grkavqnaq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gsoqgbkam.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gfsdzebkm.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gsyoxnpnj.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gbmzynpwp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gcwpgnedh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gejajtanh.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/guirzspfv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/grqakyroe.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/ggztpzion.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gboqkwvrb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwepydibl.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gvqzyccxn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gafltgqrz.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gansmjqzg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gkqcbarma.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/glfmkbgvi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gnpvzhbke.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzznueafh.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gkarvynqf.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/grcbqzqvm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxpamhyxg.sHtML


<!-- 参考信息 -->