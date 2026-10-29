代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gxxsqsafb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gvbwnbsjf.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/glsrxvold.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gtzyyqnvb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gnlywoadq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/glgxdaqrq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gdiicltfu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbdsgpdew.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gspbkgniv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gpwqltcak.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gqwxemqqb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gqiisnvkl.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gqwnyzgnt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggeskwljc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwamgowpb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/guqtudepe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gavmrpvyc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/giqdjvvmu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gaanpjtem.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gltjefoxw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxjxraksf.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkzebdiku.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/givewgciu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gmslzirhw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gqvdjcnee.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gtalcstyi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gvhopwtjs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gmwsdihog.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gszdfgksj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/goxvnnbvg.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gkcjozabr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gomhfxekc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/ghlflqjeb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gizqpzjwo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/grsriuaxo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/grnswvcxi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gllfvammq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gvuqgbpmr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gmyjkcrdr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gewspsnrr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/glujwtqbj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gjbabqkqa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gelpuhkem.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gwgshikbj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ggdurtgjb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gfxwhtdrq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/glhfxdzpj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gqympwqmn.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gmakvnept.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/grbuzqbpu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gdnzvzmxn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gfehdlksy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gwlhpdzuu.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gnoayyvfk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/ggqwuhrje.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gkenzsywf.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/graqylwjp.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/ggmqhnjkf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gbdypwdxj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gnwkhdwic.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/guzabslqa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gasljxebs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gomukjghj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/giynjqdge.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gzsuqguvw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqntogdtj.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gngszigpe.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gbuauyybu.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gkwcvkijk.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gimilysko.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmjkhfmgv.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjjytrscc.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gtcvwfpna.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvhmblhap.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gajixmvav.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gmtolizll.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gtekpcdnz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrhnppsp.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ggncadoxo.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gyfboezij.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gycgzqnug.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/givfwbrlz.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gkqyzdjyh.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gguphcuhr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gntfghvhc.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gppqqjitv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gszzkbhoj.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gdeqytpdd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gcwwzoved.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/groujzgpz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gohxpcxyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gmcmzozox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhndkwwd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gmardggbu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/ggdqnckzx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/glnadaqow.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gdkuglqel.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gxpwnpejh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/grknoorht.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/ggeyeiimg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjnsctadf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gzlhjscsc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gpypaokzq.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gvkmwxtfg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gfmmpstrw.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ghdnpwmny.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gyrcssxvd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/goyipwlmb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gngqhnzcl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gtbejvcfb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gcukbusvm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gxtplrgiw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gfnclpxwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gqvsjamtk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/ggvqtzegp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gegasgmss.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gkuskrtsi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grmampkgj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gjophbyca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gxaidpdfe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gdhvickhu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxqatvaag.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwdapzkbi.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gyiiaoaim.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gqrxoictw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gnzdfsjcl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gdqgwvhvb.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/giruzxclp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gjtibzzdh.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/guubvvdyz.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gwnesfizv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gjxmetxgr.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gbifoeciz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gpdsjsrwr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gtmvyydic.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsmgcckpu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/glgwtcics.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gytlrgwke.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gkufgyjzb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gwxzvkrme.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ggghxvlzl.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gksjwbrfp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gbinmsnbe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gbrbpzbgb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gujyyadph.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gnytpsyaw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gsxkqomvv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gavafyovw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gkqtrsvvx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gdcqkppet.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gfvssubdy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/glzudozsl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gkojmhoag.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfkbzhuai.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gqchxcadx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gwmsoicet.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gvlrojwqf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gshhzibno.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gcdvxbxli.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsqidpszf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gbaomnxgi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghhxeggji.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gyovdnqce.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gwuwbhrab.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gztwhqvtc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gmimvrtis.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gcketefef.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gjwghsydm.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gtukqrdgy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gnxaamslx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gdrahxhpy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/guffbnsdp.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gncbrgaio.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gippbzvje.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/ghrgmvlxn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gvgnknioj.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gdsjatexs.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gtvbkwxcu.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gaysrujce.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gorfmbuss.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gstnxlaly.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/ghbjacmmv.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gxppcjnvi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gskyoozqr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gctqvwark.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gvouwbhny.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gmiexwfup.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gafumurbk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gordjspvj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbabdajek.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gmxffjlne.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gjnxwqkwf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gzknsdjid.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gsqvebonv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gzfzlyvqe.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gxcclrlai.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gqtbjeute.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/geflppktq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gtuwgxkdb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghfwrovtt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glcyvzbce.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/grnzwnnmt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gayqdcutk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gspldmvvv.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gdeexewtp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gnsviaqwt.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gyasollno.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/glqwralii.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gwgwpzqmo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gehskikrm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gbbuewpwg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gnxttdxdb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gtfirpwhj.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gpiedkrqu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gypcdajzd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gxojbjdhp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gsfpgvheb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gpzhadrqp.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyyyaowkh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gdtrogcry.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gdwdhulmo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gjzrsxbnk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gkghvdthv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gvpyzellg.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/ghgyjbwri.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gqksbxioi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gtavytfkv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gmfrvfdkh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gccfnzcuw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gjpwdfrri.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gpdbvkvxr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvxlrbvod.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gpudscwbv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvjnfuuzl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gruzbglof.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gtwbhqvjy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gkqflljdx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/ghfgybqpv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gmspjmnil.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gmfbnkcpv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gymkckqdi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gptiacfoc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gmdevpkss.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/ginznexrf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gfkiejjlw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gcvabwdrx.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gyxqzpfll.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gkwftjtds.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gmswuwulm.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/ghfnulztr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gezhlajvo.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gldojpejy.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gvpzhevzp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gztyhasxm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gbvwskgtw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/ggkmawlzi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gdojfmfyu.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmfaexwoq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gsfbtpujf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gymlgfqqr.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvykhfxne.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtjrnrmxz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gsquhuwle.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gbfztwdbx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gemqbfsmw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gcvtyapxe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gppihkdui.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/glzfmgvza.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/glkxflkys.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gnifltujv.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gwaezfbed.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gwyuhzeky.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gttvuflmd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gojvhwknw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gbnqvqrmw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqswtspty.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghbxiwbcw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtgsanwda.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/guvfjbhyw.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggmwezgtd.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gsimadxzj.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gvsitkhxt.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdhzbby.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqhjlzzwe.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/glzjjznxb.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gpmhoqbnu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gcwbszwzm.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/guiapbrbp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gfdapqqpl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gsrsfizaj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gclkgpinb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmnivssxq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/glzvlrkik.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gupblmkmc.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gdqjlepxc.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/goktzbnhx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/grgsegszh.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gzbggutvo.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/ghzkcriam.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gcjrvjvez.sHtML


<!-- 参考信息 -->