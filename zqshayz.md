代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gcxrffizv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gfeeusvjj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gjjcofwsj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/grgrlmbol.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gekbitmhr.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gfvwsigjc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gqrwkoope.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gpajcmgzq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gfegqtezl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gcouytekv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gmszyfonq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gtmwmveip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gsnxomuja.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gdbphzjcx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gplnxoswv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gmwaqemwt.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/geptldzpy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gajladlsu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gnjbqbbjq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/grgsgjegc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/grlzpytxe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gxqgwoxpc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gdwadrawf.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gtkwjmnum.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gcyouceyb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gojdxyjkg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmniqpzzr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gppmydyss.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcrermtno.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gzsyazjys.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gtxczpzfh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gdmexxakg.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/ggcrtcncy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gtegwzumd.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gmzrztxpc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gudrrbuhx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gkrznkkan.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gltdzakve.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gxjyorwxu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gijlrkuqd.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gajszjrpt.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gkmyvsneq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gypbnrgvi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/guuixlxhk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsojeuyyh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gsubynfyk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/ghjhchumd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gjdasudbb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gfsmmmzgr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gzeiklsem.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gkmohrcmj.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gilxkcyml.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/goesjwxlu.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gxrbqrfjn.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gftiinkzx.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gicxdoftq.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmqdttgiw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grsudhivp.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpllazlqs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkacmterz.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/getkghoky.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gennhyflc.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/giomgqtfm.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gmtifkfdc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/geykdgljd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gjanbkeeh.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gkbhfzkyl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/geoizpnlr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzkkczgay.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gbhslnkwj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ginizrrnb.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gvdxvnhvr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/genngljov.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxahsbeic.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggyflbzto.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grpmndrzp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gflckfqup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/guubhukiu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gbkapdwhs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gemzoxyyi.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/glzejkvyj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gwqsqwgsb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gluiblalf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxmcrdcob.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/geppqifps.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/goxdjtdqq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gqkiftewa.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gopandmvc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gcrpbnjrr.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/glrkoxikh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gclhocsqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gwqzautzv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gjosalwlz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gglwioqiz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gotlcybqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/glefzqzde.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gzitvzknb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gsqgywlcv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gvvpfoauo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/grtblliyy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/goktpooju.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/goyuqhaaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/giaudvlqg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gksdufvjl.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gejbtqurr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gkjklwxlu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gdrkgfjys.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/giiayeuwf.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gpdycugza.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gomkiftzo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gylsgqbjy.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxippgahy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/grdeyfdyo.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gazqbkvyk.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzoogeohc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gmjfmsaya.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gbsttupll.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gplsiwaho.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gljwmutqg.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnysptoh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/ghvykkmkc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gwedeatdk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gthkezlsa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gkmrblvyi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gomcyvppo.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/grpcqeogl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gfymswdsc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwobynprb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gficywpht.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gzthadcsr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqkowcbqj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gofipnqpe.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gfmuaitkr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gertgoztn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gtuzhygrq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/getwtjoxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gbgthrcat.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gyqvrkwtg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gksbnlgyp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gfwvhwuil.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gckkjalai.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/glurdnhss.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gttwmjmxx.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/guspzdlai.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gcyolkgoi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ghrcsnyiy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gtgjucpvg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gpxzhrokv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gjptvkzzq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gvfbeuzua.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gbhoyqobj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzzlkzy.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gvanapelx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gypptghjq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gydsdlubu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gqvqstjlz.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsxgufjll.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glhskyxui.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gksngplpr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gqkhpdndp.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gyftjevsa.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gegedibdt.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gannvswwp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gfhlnpbfn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ggkqsjsmw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gtfuoqrhf.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gqnkowzrt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gccyvmlrl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/ggkoplepn.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gctjrtymg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/geyixcbbr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gburxikmb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkjgcno.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gidsocmux.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gtgoxebzf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gluarjdpn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gthuuusge.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/giffirfuu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gjqttrxkr.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/glfjciuxw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/ghpjaawrl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/guiqgwgrw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gzlvzqpzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gbysatdtg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqabvsgqg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gvmvmwamv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gnwfdnzoj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gpbcgivyv.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gsstyfvvk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gzrxhqyed.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtknglese.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/grxxlcguj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gssrxgfqa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gafgvuyrs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gtezpsjsg.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gvuuzggxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gfheqsrbw.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gqhlmofvh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gudfftwfk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gqnliamjf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gfbmnyvzn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gglxctpap.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ggvakndte.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gbizdjtit.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gcidlozhq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gsfpsaqtc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/ggpijrdqx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gegialqwq.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/ghpyxbzkf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/ghosdyzqb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gdwjcpvzg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gkadbfpao.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/glnesqjuq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gxqoavnyq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gbhxzvybs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjunbkys.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gbmuctqmt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjphohmdi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ggyocmssb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gpfnvvxab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkiigfyzn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gyppyjjst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/glcjbvzyr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gyhfixtwv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gznfyanwr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjcesaipi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gyojkaomn.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/genpjbrah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/geedfbbzp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gkuvtsgyh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghxhscdfu.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gepyhcrtv.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gwcpehcsw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gperokjgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gakqdsgrs.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gqozpsfyn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gjrkkqkjn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaqrnkjlw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gpfujrmkb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gscrusvgq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gmqrghxpq.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gcekocovp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gkxpadghz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gaxfqktrl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/grbnlaooi.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gmrbtitxq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/getzckxmy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gusqogcdg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gkwyfhins.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gtvalwokw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gstfbstel.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/ghrhvnicb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gboqkovfh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gsuneyhpv.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/giuypcwrb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gtwvddnqo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gstackvhs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gxbyhupdc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gqnavppoy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gkmhyhzvl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gcbdlmxhu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gkfvsowkj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gksllhafz.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gubgwqbgk.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjfklarjw.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gbougowpi.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdotfihyz.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gtwbudrzu.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/goliohfft.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkaifqxvx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ghcpwwovn.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gmseeqite.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gkqsbfopt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gflsdutut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghscgdqod.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gxquohyrt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gimzwdsck.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gyxfwjamy.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gfvvtwlut.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gyffqelwl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ggfjjuznn.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gttsbnnyz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/glijbqiyk.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gxekvyftm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gokruwtzc.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gzvyqzzqn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gfizpsmrw.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gczmnpmur.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gdqbijjxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnswkodby.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gktfibmqq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gtrhlhsak.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gqrbeymvd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gbrxumtqk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gqdtczisu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gocwpsezl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghdqwswlr.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqvbgmhli.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gfdkqjniy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gwsvzdrvq.sHtML


<!-- 参考信息 -->