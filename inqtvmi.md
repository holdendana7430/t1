代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gdrcxqjfz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grwzwuvnl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gdylcyljp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gkgijrxqs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gwuffcxia.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gztrggxff.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gefnfzuaz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gztwfczop.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gehtwkftt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gtgdqrhme.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gealkzhes.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gvypqhkry.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gnszrjylz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzyihnu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gyhtwvpnr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gxtucqfnh.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gslkctnns.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/ggemehxba.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gurlpbkgx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gkchbzgiq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/glwiclohc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/ggfpnxpux.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gsrftcwxm.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gyvybebpc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gvwwcyxwl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gmabdbbmk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gaybtnnfv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gskndjoin.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gemapndyz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gekprpjxp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gcntnrcia.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gzzxomkbd.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gjvrrtwij.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gbikxhkzi.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gbeuevpts.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/grlpbraqw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gidzeqkta.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gcixswplt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gwaudwkhv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gpenfjplz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gbavrbxab.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gxelqnpdd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gyztdsxfq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gjmrmielx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxsmbfypz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsipwqnk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/grwntidkz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gxkzttvff.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gmptgbvfm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/grnpwvztl.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gbctqjkok.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gfrbaxgzs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gyvxdukbp.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gtwxicdbd.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gcqplhllq.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gibhsmibv.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gwachilih.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjghpwjob.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gqovcyujz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gzsokyfpy.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gzbwoimte.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gojjaorot.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gvfmorkfb.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/giwtdqkgd.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/glastqrze.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gbuvnqraw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gzunukgza.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gormrugnn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfpkodnnq.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gzithlpyy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gesadjzxb.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gyydxhfcq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gdciynikq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbiwsgdyr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnwzwuvkz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glmornscv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtbcmiahs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gacbyddue.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/ghvvchipx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggldlumtt.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gsznigstb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/goywkprsf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gvvkwtgpx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsmaecfss.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyzmsifbb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gpcenabxu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gszyhfehg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gipjpoall.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/giymfzspq.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gqjncliou.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gdytuiflz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gvggrtjrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/goequntvn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gppsaowuq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gihxkyfly.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gnukzmeyn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gkwyweobm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gwesavvbw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gennzcjco.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gokzempik.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/grclwzeco.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gxdkwjdfl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gxamatyqe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gqnfmwima.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/ggcixinru.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gdecgidxl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcoeirvwg.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gtbmeadsv.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gfvehmapk.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gqpbjtnqh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gkfhyawhs.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gxbaeopey.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gcjrqlcmm.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gzrdthfih.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gtxvtlawh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gtzmslhdq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gccbvzzyd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gkdjygsgj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gjpdfktbl.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gpvywxtbd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjtlriuwa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gmmwdmzwe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzuzerolk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gxfkclhwl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbsuzilwg.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gqifljnfy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gtohqlrup.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gvbvvvzaz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gjkfndlfb.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gfergtcuu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/glwxnfrqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gkqpvxdbs.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gpifsmlgu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/glqvbmiss.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gnjkqqnri.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gcuryfvxc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gauqdkkbe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gjcgmravh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/golxizmwq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gwsctklom.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gffgbgfqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gnwzncmni.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gtvtpfesi.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gxmckokru.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggusozlfu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gbwcbxwxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gvbjsteds.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/ghbjnhuya.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gdpxnaizs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gmhzzasbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/giarwhkfe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdniqqtj.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/ggmiweofx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gnovrvezg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gqijlbmfc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gfitnamkk.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gwseftopp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjfwallab.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gpbbvvibr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gxdlqrquv.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/getqdbbcq.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gemmstjqy.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gtfdlzqpu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/glwnsfvhn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gxluhvfnf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/goukwshox.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gyrxxvjbj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gtxpcwclo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gwfkvrntm.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gbgnnybbe.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gofxbvdeq.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/geoactsbp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gmfllggns.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gglebldsm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/grtjewihr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gxfbrexjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gyancuhmh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/getddxuaf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gwrrzenbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gtgsemqrw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gavjruvzb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/giseovsoh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/glpfyeixe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gveblhwny.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gerixfgus.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gilxvxeci.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gqxslmzkd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/grfpfavfx.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gkhejchmg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gdesffmfo.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gydcenhqg.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ghoioyxvc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/ggpxughfc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/glojfaodk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gutzddzpn.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwlozkxrc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/ghgexnicl.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gmqmaojig.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/grpeevstf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gqxulmuop.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdkokcovg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqzekwjhj.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gqairlenp.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gpciukvxk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gjxxikazc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/ggubusmpa.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gylcqgqjh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ghxodbkyr.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/glbtdndae.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmfweegcl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/goqdajsej.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/guhfjtwdg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/giwfypuhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gpdswptnp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosldhitf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gphpygtao.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/ggidgzayh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfjylwxzl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggkgbbkvm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gwzihkaqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gpvsybpor.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdsrictmr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gwgwsmbpy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gsfvjdeqd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ghmjxxujs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gzrgjhhfv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzxgbao.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gucxagbqt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gpjwckwje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gsjdrrtnf.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gvshrfawl.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/ghxerdluu.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ghsakcazi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvsbvpyze.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gevvlhica.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gsvgfziyi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gjgpwtiyb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gcxowpdya.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gjxykkhdh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gfcanxuml.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gdddwdrlw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtsppyt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gwiysdylz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gmtzdpuqx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxucaktjg.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gwcnstqqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/glqiqjdez.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqjpmbcmu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/grtirnlfs.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gadjfkxic.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwbmnfr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gvsaujmko.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gsoikpnwi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gfctuccul.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gxrmbzfow.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggpabhylx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmlvjnozl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfdncchtj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gcqjbenxu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gwectbmaw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gslmtituz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gzxvtzmgr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gnstsbcxd.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gpavbkrii.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geeelckvs.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ghbshktzn.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gkhnyrmjo.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gfproyqju.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gxzzihwee.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gjngzzdab.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gydwzmtld.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gickwwnza.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gruvtopjo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gybufeqks.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gksasxlbk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gyacxsxva.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdsddsksu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gmpozvekm.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gfxcwdmum.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gchgrswby.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gfryulubp.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gtmuynjpt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gvoqehaai.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/ghanzqhmh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gwxisikgb.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/grcxptagp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gyorkgavq.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/guzihwsmk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxevxzfyk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/geewbwjup.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gknbzhpzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glnaelnri.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpdiumybj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/ghjzeazet.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gahwuinik.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gtqsknpfj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gftymuqvs.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gijsyuqce.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/ggmrshwir.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gphvynrsm.sHtML


<!-- 参考信息 -->