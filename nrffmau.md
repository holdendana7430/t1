代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gadltujgi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gtpqxunyi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/giphpnqoi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gnekttbhq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grkqxfpip.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/geokthrci.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/grjmmdgck.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsmimpkhv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gxysybwjv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gxewyncjy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/guywtpavj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gsyflpetp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gebhtdjee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/ggeigipzr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gowdhavbx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gjqfuqjua.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gspzloxzh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gvxyeeekz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gcavjbldv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/ghhzdcmhw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/glqnwnheb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/goxxjgbos.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gxizwolsn.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gmmoltqno.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gkwuxwftb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/glgizjbev.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/giadyluaq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gbaoydref.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gfoacjbvi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gdewpmrhh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/ginzcozns.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/glewcpirl.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gsbiqvrmo.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gtqxbinqg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gubqkisuw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gkzszmyns.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gjqtzuxgl.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gvjxnxgvx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gpwrykcxu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gxqrymjif.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gimjedkfz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gwxmhfjgx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gmohgxmrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/goaclxnue.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gjfjsunyr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gyowzjdtw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/genurhroy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gisrtrwhl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gyhednipt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gsypfvbcm.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/givqnanaa.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gzcdxjzso.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gznhjcaaf.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjwpdnraz.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkekhrvpk.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfalmusyi.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gufnxijbd.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gdnerfdwo.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/glkatywvu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gsxrqddob.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gqdezsolm.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gkbohizln.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gxupfhxwz.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzjzzzupe.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/ghphyvdxk.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/grcrzumhf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gkuvmtgfx.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gnfazixil.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjdsawgej.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/ghxgfsihc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbtstbgwt.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gjysljpoo.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gguxyyopo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghfvypqsh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghpoaszav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzionmiuj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxwtisxpo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/ggaeibhql.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gzsbumxpl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gloiweanq.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/godkmhous.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gvzbemmfa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gherigzrt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glvpqhvuy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggfibietl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gdtrymlpl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gqomkkdtr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gpwuldrrn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gdnstylst.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/grqaqoaru.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbouzfsq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gchbgrieg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gfjwhuson.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gfrgpeajw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gnradbapa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gedaevcja.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gspqhcxbd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gqxtcjmwo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gjuhtaptn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gvmqmtxmf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/grxbtwwlv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gaudkvrkx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gmkmhcrxh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gdixewtwa.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gosokjtib.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvwhshxmf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnipdepoy.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/ghqbxdirk.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gmjreqsgo.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gmcwsjppv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gfjocinel.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gjhyeczmd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gwsfphqwb.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gmjetmrtm.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/geejvyfng.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/giqrwoxsu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/glclrqdju.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/giczhfkcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzykohm.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gbgcdnqlp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gtmuqdomu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gsppojjfh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gysoedrmi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gapajiulm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gvauqebkz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gwfarmobz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmngpuxb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gmrdjsnmp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gxaquqlih.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gznayrlbi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gxnssqfbe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gpeifqryx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/ghzwjwepl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gjwvhqhzj.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/guucqacoy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/goqrkcweg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gbbskocvk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdkaobnue.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gwcjgotby.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gmqktmrzc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gklukhyzv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gsbcynxqj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gdgjapohv.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gedjoerxw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gygjpiztu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grdeetdmf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gumtwszjk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/geavgtmar.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gdeeidhva.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gvaehemsp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gjxekfojm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gqbezkcya.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gfjsurwgo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/ggapguygx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gskarothm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/ghbgwszhk.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gdrahuqgv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gsmwzvcfj.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/garlfernw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gnbxiyuoe.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gdcnxixun.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/ggplmfvnz.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gtfkigthz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gigagrpwt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gzlmhlbpk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gcztwqrmn.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gggewahxu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/grdkrjnus.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gqkwfvyfd.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gccupdmrm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gpzgtndos.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gmdhjivdi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gotccfsgm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/goqnlvejp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gfgoxwuqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ggcujwggx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gvpswdvnm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gurtnxxld.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gftlbwjon.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gptaflvrq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gousddmfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkdlprvim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gbfvlwsbf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzvbswqxb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnijlyjcm.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gidhekorl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/ggjzfzrcd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gnjymszaf.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/goryifuvx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/goqomvqnw.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gwfhdxzkz.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gydqvceim.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gfdefcbmk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gslfcbied.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gskapjewu.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gqaoiiumg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gppgpvdsv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsthokqcc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/ggoajttrl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gdjcthikm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/givnsigbn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnvazhuqz.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gatpaxotz.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gplxzesol.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gicfjbepr.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcmxhjkjf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gaybgqzve.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gzrttwzup.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gxezciaip.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gtqnyahbz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gwiztyrhj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gnrifaamd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/grqkeuzfr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gypkvgwhi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gtvshqgjg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkdyrddiv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/giihwokkx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjeirmxea.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gydfnyzpa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gfhraucdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gsgtqqbys.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/givhijbwl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/guzhkvlzv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/galmgvuvh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gvtkykzqs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gunbslyjt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gwqxtsuwj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/ghlctqwyz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gugjuqbhm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gcyspoetk.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gmmnpeggi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkvdbzcy.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gbkhpezbi.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/guyzvhpxb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gidrzczhz.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gideqlkdc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gbiswqvja.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gawlwwytl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gzkcjeqbe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gvckmfmae.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gwobxcmvp.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gxiwrnurn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/glkflvsxv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/geeseimag.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/goaspmgvo.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gqmjqknwm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gpflppgay.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzuclvhyk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gsllywoaf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gmkxjnqcu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gdwenmdfm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gcpljowev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gtcumjljr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gvkpmsqxo.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/givxpewhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmlgvyfnd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gwhbhadgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqzbaqlxf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ggvyiwnfh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gbjoptkwe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gcbepvntq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggpbtvefi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gwuqwtbjx.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gbhseyubn.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxohrcypj.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/ggzxkhvae.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gwblopmkv.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gnrwpqhky.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gddxiybnf.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghgygyhre.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gwcfecsbd.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gionsosml.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/grrlhftco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gypwjxeyn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gcykmkjcm.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnvuwuroj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/glmybltlo.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvulktw.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gcbirtshd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/guoiiyldd.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gsnmvrgjt.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gfsvlztwm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gnhldsfgt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/grjzmlbob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/guaoguzjg.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/geyvyeupq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/geenmstqa.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdnbryqab.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gzwkuygyv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gyaxpsqwq.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gumesmzpb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gvwcpvotu.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gjlvdkcwo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/ghbnzprrn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gjggyebhn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gvnhwgveg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gcutaalgs.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gipgpyjso.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gfbpzrgrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gqhvddzzg.sHtML


<!-- 参考信息 -->