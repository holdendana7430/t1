代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gjsaftzsq.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gshrkzyso.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gmssyilyl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gfuddznqs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/ghanwfadr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gzicgvhdo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gtbuztxfg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gdlukwoev.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gxhueutxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gzcqskjmj.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gjmjgdhok.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/getfmzzfe.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gdogmwjcm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gtjzfwaha.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gcnolmxzy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gapuftdag.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gxtxwuafw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gnlswjywt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gdoxexelm.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gbtorxzmi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gpmrxzjux.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/govfajawk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gvfbmmcvo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gzlwytibh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/ggkfkqpkv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gboqnomyz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/ggnqgbmvg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gddstfgji.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/ghmkpwxoh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/ghuorgpmk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gcmdzhtee.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gmskydbqr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/givbrwqkv.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/goroisdhj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gdroevvpr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gyfwhrbay.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gpcfrejrx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/grnctjzqf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gvyidbted.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gdqwjtwvy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdfqxqxpb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghzzjyiyg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggozhjpoe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkwjgfxmc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gcatpwvar.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gqdqiibsb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gzvzysrgv.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gwiisrzeq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gklzidjhz.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gyrsolvfh.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvdlemf.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmydluy.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqqsavokq.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzvovehjx.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gatijhmmc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gyjmycghe.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gjipghqoc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gsicpxelt.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gkbaohpsw.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gmurdaqfu.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gqqtyiqph.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gbrczhjwg.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gtrfjehhn.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gwifnlebs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmvzhqvin.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gthugpggv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaywkqozy.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gamwzrwbc.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gndhmhuwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gysscgnyd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gwifemfkj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gikfqhqmm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbswrifdq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gadxrnqct.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gutleebfa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfsbjjkmd.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/ggsgrwanh.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/givhmcssm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gerrpoixd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvdffdphp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/glpfvwezj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gyznrbcgx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/ghfbnyebg.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gtbxyvwjl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/goztcaclx.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gjswsvrah.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gsyyiyexm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gusrdrfnu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/guhyzwfev.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ggnzhzguj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzoucsktm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gxzawkfgd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/ggigfwltk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gpwxqoagb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gtowygwbi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gzbvfyznb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gqpqvpyig.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsfnbzdra.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gicnjkrwg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gyarhtywe.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gryqqtjwy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ggjrdgxmx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gfuewoyux.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gosrqmgsc.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/glwioomyc.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gekewujim.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ggitfaxwp.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/grrumedpu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gsweenjaz.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gztiikahs.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gmsbfbzfs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/glmhaiyvk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gwcygtjqt.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gecewskqy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gnzyqaktn.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gzfljtddz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/ghxjutfgt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/goevgrlxw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gycvvmxyz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gmkvvnpku.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gzbqiasfh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gvcvccwxl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnbhloje.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/grcowjkas.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gyficmett.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gzhuyppsw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwlescvfu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/giyheqgxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gowhrnfqx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gyraelobx.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gsqnaoact.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gorygomcv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gdockpfrk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gnweexado.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ggeflrtox.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gzrjyzkgg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gicgezrqk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gpojrgfyj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ghikukxts.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gdqgnwvnr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gfpcbzmsf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gvddygfdv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gztgrbugm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/ghpiermbh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gugpwefuc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gxzsgydlw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbwyxnqhb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gjictlmaa.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gzrtddcic.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gutlxurpd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/ggknnqetv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gyigdqppn.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmvmapnwm.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/ggglvzitg.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/grffcdckn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gpygflifj.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggsxxsnqf.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/giyzylori.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gyybuapcl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/grrlbirwb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gnlkqazqe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gbqwtoesy.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/givnhlvge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/goszgtmli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gytxshsbr.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gtdombkwy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbhvmsx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gvjohoyyl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gqgtoyenx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gufzzbvse.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gjyfewrdu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/glcykyqft.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gmmzbgpka.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gujcyfyor.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gyvdvaqye.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gfngcpkww.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ggwayiblu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gohwhymel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/giorrylsx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggxellqso.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnmclpagn.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gxwguvvew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gollnqexs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/grvfggukp.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gtxwuolfz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gmksityau.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtsrkmliq.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gbcvkhpiv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gcxizcnbg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gkfdsyvfy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gbirhidxz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvzsupu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/ghpnetmcs.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gzcgjivnw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gwyyxnigc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/grdxnpgwq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gbdmlcbmn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/grhswrkxe.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/giewhreoe.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gadjcllqh.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gcavamaiu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/giwrtglqg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gogfeljsp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gybhgztvz.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/golfjmeto.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gzeolyusq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gkxactyxn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gwkxkqcow.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gpexgqebd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gmgdcjfcx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gjbjltrsz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfdyfbrko.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gevbvdrop.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulmfzjky.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gkmvdxjft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gnzdihhko.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzogaex.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxsfnpk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gzicylckf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gmoslqrkr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/giynofcqe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gbpjgaczh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gwfpcytuy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gosujxfhg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gahkgassh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gntvkasnk.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gnwzvvyeu.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gwomtkncw.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/geaeqhfxd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gxqaaraaq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbkqvivc.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/ghnhwgush.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gaxlnsjow.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gleodzfrw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/ghkxkfklw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/ggzaceoaz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ggjrbniql.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/geldpkelo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gbhopjulf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gtgtaujav.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gwwzlloou.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gidznvmay.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gkasgcgcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmrtuficv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gduuoooan.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gzcrnkkza.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gggollmfn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gyscvfkbm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gnziuzshz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gywsahwoj.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gsdesbgsd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gonpiorgf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnndgpzja.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkogslwwg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gsjrhlaxi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gkmujymmy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjyrgkp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/geddmqalv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gcasvpwym.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gdwonznkj.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gflmrczyn.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/guodyjknw.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/grymazisr.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/glmbpzowq.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gnaqmnhxs.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjbpaapnq.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gcorkzdtg.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gfmtphufq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/grwvkenly.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gxydxyhvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gvhqgnirp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gfyzjfxrr.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ghbrfeoji.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gryanecgp.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gpcxunric.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gbstgghgt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/ggomflfxo.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gegnjjasu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gqlcoqxch.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdvknymvf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gzoqhycza.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gunmkfvis.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghuwkvplz.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gbkkqeoqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/ggqrahnoa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gedpxgdno.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gzjsfopbd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gbfqupxsy.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gvndejyyc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ghnhwnsfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gooohhbsc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gnqauknrs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsfklouij.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gqlsuypqj.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guuvkshji.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gnrytkfsc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gehmesawg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gybitntkw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gsbczloib.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gnywtgvsm.sHtML


<!-- 参考信息 -->