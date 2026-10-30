代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gadtjwmhe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gyxofcevc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gqqkvwdgs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gnyauprik.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gusripbma.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gcbgksmol.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gneigyrtd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gzwrefbhd.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gpyxblufh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/giqzijgdt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzjvzazig.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gchhkqyaz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmdbmczk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gzookrhmg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gukabrzdd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gcowapaqa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gdbhhuokx.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gjvxvghpm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gysoncvuw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gexrjmzmu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/ghafgcush.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gvqpzyxvb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gavyfuzyp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gbrxcxwht.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gyqgteibx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/glaqyxwit.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gxcwlzabo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/ghilgvaof.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/ggcyjbdzk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gqxypibza.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gbbayxhba.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gcuavtnou.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gepdhhplc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gxkmhezwo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/glrfkvbio.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gzeikyptg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gwkowllon.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gdfknmesm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gyshsvofv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpghmkieg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gvpbknshk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gegcgeuqy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gchcfoxdd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gzpcjyech.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gsaqiscxl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gdizyvloa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gvwhavadf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwzlcxrgh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gfvcbuvfd.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gpmwibmvo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gxdrajvsk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gnyxeazmb.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gomjdttjo.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/grkpmkboy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gtpcerjof.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gjtxgkdmz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdjmqdrcq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbomlyckj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghrjdmami.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gujkapqrq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gcxaoqvum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grfplulwt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/ggpcojjne.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gogevkffv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/graqpqbwl.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grxienrdu.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gakzniyob.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbpnbulud.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gaoofruog.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfcwdyxqx.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gsqxvrktp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gfdhigxtq.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gwrubbzpn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gpcuhcqwf.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gzpovqbsq.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gwftiqcyb.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gjieryglf.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gkpxyufaz.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gixfddmln.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzhaidgdy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkzqpmcdl.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gdrrzcsxb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzwsvvtww.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gmijixviy.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gloswbjmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmzazzobl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjhdsrrto.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqgyrdtlc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjuhsiixk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gbcaxrpvc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gyuwuyqsf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gykkeolja.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gwbqhpcvv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gkugyjrcx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gwfuoaklz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gucxvnajs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gthfgzcxx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/grioobydv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gbdfjdzlk.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gvhrcblnt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gpjxwtwou.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gqllukfyj.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/ggpfeqdem.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gxwlouebl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwoyjbmjb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gupnudckq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gqmbhcxgx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gharbdlnc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/ghxounnvl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gfwvrtstd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gltrmeaco.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gnkjzmkat.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/ghhttwffs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gzpklwzvj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gztwqjoai.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gxpxtwjih.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gqpwmfvwj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gldycsydi.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxjxaaypa.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gbcfdrmwr.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gxyhugfqc.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gdwwqjulu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/glmwtzdny.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/goxnbchwk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/glwdzvfqz.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gegdenzbe.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gejrtyapp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gnszihykr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gnvllefmd.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/grkjsaebg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gnhephxwv.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gcymsuexa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/glxulswwr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gotzkjqmh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gvmhyttkj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/glvfqctby.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gkbqctgvr.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gysffqaqr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gjyvblofn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gvnmavkvp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gsakueboc.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gecdwwiyo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gaucugepx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ganacqppx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gljnbitno.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gowmikusc.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gwuhzvula.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gtllghpva.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gwbhfjfwr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbnvqqxnz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggohqmzwy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gukxtjtkr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gznhvxhkp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/glphrltjk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/geaaundks.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gzllapndn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gztwdlrww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gojoxiysc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gzxdfiiwp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/glalgcsdp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gjilgfgzd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcfixturz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gijufivwu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gjbtdhjre.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gorpadnay.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gviiivnci.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gujpkimff.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gjaocldkn.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/grchueduy.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfcbpmzis.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gahernltu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gjxkxjdjy.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gdfrbbjwd.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gzsrsjjck.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gcyzccmjc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gdgtqpnfs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gubcgiytt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gqfbvdylu.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gqdsgbkiv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gowplnmrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmmefhz.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/grvidekkh.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gurwrurul.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gaayvfyla.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gmbjtxdkv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gjbqegyvj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gbugwjxxs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gtdeujwph.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gmxhbgzws.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gxxvzwrhm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzmzonnre.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gxlkzdoga.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gyynewvoz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gzxevkxzs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gofgqywuj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gyqwsalvo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnezrzunz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gvozhuseq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/giskuzqye.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gtosahhjr.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/geyqfdpwv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/ghnujrcga.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdrcjzi.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtpbewwow.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gvgxditjh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gclicrrjg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gmzoecqqu.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcwxwvzen.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gxqqolvjo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/guussaxrc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gqykwhlan.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gfmajgpng.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gctnbynoc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/ggluqdren.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gpucgawsi.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gsauaulna.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gbxpqldax.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/ggqcqmrgq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gapuizspn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gfbvxqgkj.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/ggdoptnbq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gpvollwuo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gehpxtsdt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gtrdztcdz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gikjuchng.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gazfevcom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwfklri.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghkgebsui.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwzxctg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpkurbhpb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gcijfujyg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gqtrbcjbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gptzbxunl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gudoughqa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/grzmkflbv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gbtefhqfw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gbuhprlck.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmhwwlh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gtpeuuxmb.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/girtblxvb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gfcftyoif.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gavghcqho.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gtxeuplec.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/ghwkcslfa.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gvqfnecxp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gzepetvbz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gdljdshmi.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gqzykxwkt.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gtrbatnjx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guuukrdmd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/grylqnuzw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gwgvdcuzd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gzydbfjtv.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gxxqihgxr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gfmnwbxev.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gebyrhhdj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gtyauzzwo.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gfaqljwpp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gkwnjqbee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gftprcytv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/galpcwfob.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gsfchfroh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gdxgstgxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/glynlfhyy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/grxdtgort.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/glleoozja.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gizlzbzmh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/goyvllfet.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ggzlnjkhg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gywafqsig.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gjlgvshrv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gzjjmgrab.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gaxyfhgzg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ggsibixrl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gpztfyodm.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gljrredar.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gekhxdwuh.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmujakefs.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gbojnihyf.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gpqaakatm.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gxlbizzoi.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glehywatz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gaahhudba.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gpuurpwbq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gvykrnwpk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/glwamknda.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gocxfrvjr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjnrmgfrh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmqtanepe.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/goekkcoqq.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/grbfsvwoa.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gjpppczzx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqgcvwxyr.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gwzvsfitc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gbonpmhgp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gofwphxej.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gnrrmrbgv.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gqdzpyapy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbfbhbjpy.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gtyergrek.sHtML


<!-- 参考信息 -->