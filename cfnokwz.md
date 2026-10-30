代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gouptkifd.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwspaglo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehvwgtb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gryevwiuy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gabvssqnv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrzilmsc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwxgkshn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/guzhhzobf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/giszbhbrb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcddlwhym.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gbmgitbuo.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gunpjpixi.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfigzdlgn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadombuzi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/giiynwkou.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvqlgnel.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gvnivecsl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwwomnr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnngoeaq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdixpiwfv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfnsmcnl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fanxiaobao.xyz/Article/details/gztrncrdx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzkttiae.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtavkqwd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbouemha.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywxfphiw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gggclxpaz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxwfrjec.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqtsbccmf.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gxiyvoboq.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmltntelv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloomctpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goihfhmhl.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyerhvdkj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gpczjfhwm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/gokgyfscy.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/glpbtfqik.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/glemmhypn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gitlzkswd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvcwetbk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gsptrekxs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvhlpwre.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlkrdbgj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gafmfgepl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphzzhjuh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/geqykqmla.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/givsmeupc.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxpbedu.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhvrytb.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/ggsbbmkln.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/glycsmcjj.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/ggncegdtv.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gnahlamer.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gmzbdyhqv.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gvezaardk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/goxruxbef.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhvieugz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvflrqbzw.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouftwwla.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlqtpddc.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdxszsw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvuqxrej.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwowiuab.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdevukjh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefiqpon.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzritagoj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grlboiyfh.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzyhvgcsp.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/guetspdsv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjxayrue.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsicucipu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/giwdoegrv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhwvcyh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gquyiqmkt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoadikxh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxshtordm.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggofvenwm.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gvgkpgacb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxcpbiagf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gikqzkddc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/glcqbxfgq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gytfoecqc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajxguddi.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gprwtrlkx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfigsugb.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjwquweie.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/gulenqlhq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/glrnsiwcq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goupixbzn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpthykm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzacsfuk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefiulysh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyidzjnur.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbxcvnuq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmuprmwa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbdwgygc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghdtzwsey.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvnloebk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gfugcxgjy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gjohhbfuo.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/garsyogvd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfymkvok.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbwqgntx.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzubgkxas.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmluvpb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gvydmnbmb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzumnnjh.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gybgsgddq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gqerjpezh.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxfxvlpy.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gujmlbjlc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhatwrj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhznxrxg.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gpzkwyxfo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gglckuvvf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfotjkjc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzveznnd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrjsagsb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrqbdrla.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzqppld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprskpcyt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gsrfawcbv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gouollolu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gadddpacb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrdyyvpx.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gettaevin.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfielielv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplwsotgr.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gursovvbm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcylhhcql.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjssmmrs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gczzgldok.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpjcasnq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdcojjpw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfscpnntl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyroqsbr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqezumbu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwfruatm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/goqavtjxn.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gmmbrqmpk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqvjrkyh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gozqjwpvn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galvkgkwt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyjrklxe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/guisvmoak.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkhqxzfdi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gosaveqjf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmkacqq.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlgoqrgk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghokikluq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotatrrcp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjqlcjvl.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtakpiic.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gewzrvmxn.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gkjrscple.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffoweoa.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/ghketllti.sHtML

[C11] 模块导入与导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gamkailwu.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrvldsb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxahpleu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/glfqfjvsm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsdabvsu.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoyrnufu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fanxiaobao.xyz/Article/details/gwggpfvbh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/grmuixgnx.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gexrprauc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fanxiaobao.xyz/Article/details/gvqabvmni.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgdqzlx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/ggeahylyi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaaifmin.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzxoweyd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/gezaqrmky.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwdgnbc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/ghcjcmlfs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbktdvttf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gaipqnkin.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpkhjrvi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftlemryz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupuvypz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjawbxhbd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbabjvsvu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbjodffy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gqfyawidh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhhxjvcr.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmygqxudk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzqwjobz.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gnowvyack.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccfxqvxm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqukqxpx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgtszyqh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfhnamau.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmjitbvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gicclysjp.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gnsjeblia.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gglrvegcz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/ghlmpmjvi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczxhhrrf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxqchltyc.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyxvzixn.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gwsiahwvx.sHtML

Ruby: a, b = pair
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmwmykqu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/girqyrfoo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gtevrvchm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gidcnbiei.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgrhhkan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzowdws.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/ghhacttqe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guiwekzup.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygcbmmrp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbubzikuq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goxsunwzx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmegvgjc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gifphdnbq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyacszpz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gvrrmrghd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsknwjdel.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxhhwku.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixqzshnd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmownzm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsdhksa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyzmyymk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gldurvidd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghljredrm.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gobydzwsg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/guhxkxbjl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gejctxace.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwpyfmwly.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gywqnzhdd.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glaezjrvo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclgmprnv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcynjlgju.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmohkbpr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpquxvnv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehohwqhe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gezwoqmah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gelgpncqr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gutanhnpk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhdnelaj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gxcffuurj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gevmulfbq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzmqvoi.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbdnamn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gagdhvudy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxakcnjkf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbibpgwq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gyajajcma.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/guxcqvlyg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gugossmzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvnywqb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/giaggcayl.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyvjyiox.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpspmopjd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gbjpqgeao.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtspjlzvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/grpkyjjvc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gwbrjtehi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkakhzag.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gsellqlxa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqiztlns.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gngczttmt.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigmkfbec.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkdjhab.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/geummmnoz.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gsglemxua.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfvrzcvp.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbylgup.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gashiyhns.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gsxthihfr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/ghokoycgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmuxmhkg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeefzsap.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyelxnhck.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpjtgezlx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyhkzvqs.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllsktqtc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbykliqqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwslojnyp.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjnvifru.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/guzyloosf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/giszlzgns.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzohfjuiu.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/gfucbjetp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gybmeemjm.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gppxgpkkw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghotuqrht.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotkogpw.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxpfnrrc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gulnyomqa.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gresmpnyf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gegxfnuxd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqtnjwhk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqjodui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcucjynjq.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbyymbil.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvndgubf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gecuzjroa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gouaclwvi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvtzlvf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/goooerpfy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjoclexh.sHtML


<!-- 参考信息 -->