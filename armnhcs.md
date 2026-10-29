代发 wailian999

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/grjlwlytz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/glupbttba.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gfpopmabq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gkripfoul.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzvanboiw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guhelghzl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/ggbbiokbl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gjgihuuqc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gcvowzqtn.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gpmvosczr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gdnuhyyfa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gfjhmdtgk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/guqdynyyz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/golylvpme.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/grscauzig.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gozoffuxq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gwnklxuih.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gnfwzpzsp.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gjvhxexkk.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gzzxxcwom.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gypfhckcx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gbjkbemum.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gjzstwrgm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gwbhuaczg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ggegjefwi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gjiyvivtc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gjkpdemrq.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/grmtwxjvn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gkiyvpvgw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gxltlxfet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/geejemdse.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gdluwsqbb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gerqjltlr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gifegopdy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gfbzwvlan.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gtntycyui.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gvszdvwno.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gmfdtwohv.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/giuxffmzz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gurvrzjps.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gtngghqyl.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/goyrctwqw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gywgqztyr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gtdgcnpnd.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gshdfibyq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/guxmsgybc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gqurhixfd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gwyhewxyc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/glvbgcole.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/guytolkbr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/glecnnjbu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gybqtsubs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gldfelrzv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gkhmtndzo.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/giarhmzbo.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gcfuygvex.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gffsweoou.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjheezuus.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/glowyygmr.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gncqnzzzo.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/guwtufqel.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzennweby.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnqlivbdg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gsrshhfgl.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gtfydqoca.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gsgrrbjxx.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gxpslnwsm.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gxlonexkg.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gbgwwtbfd.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gevosobjb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gpzgftraj.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gldojoxqc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grrsnfhzr.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gyjayogcr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmtkrtyde.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gvboufqup.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gegpybwkt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwdtgyoaq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbrjhrcf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/giajpinfo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gqesruogq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gwlueocvg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gfmppvngf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gutuaktdv.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gftmpwrlc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/ggecdepmp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gkstrfaeq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnvawltaj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gfipnrpos.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gwbnvwety.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/grqrdwpha.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gxtmagdrj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gbodeesis.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxsolkr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gpwfeszdc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gkgrsaymo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gbmkkblko.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gxvdrposp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/glinizjva.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/glytwrpxk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/ggywrahkm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/ggbbhwhdk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gtwjbkjkz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gingovawk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghxrqdgcf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gfirhthjq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gdmvbvdca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gwfihsfgr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gjfolphfx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gwveeoeuu.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwbtziyfg.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gltqyspwu.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gelzyyzwi.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gksymxnzh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/golmauntz.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/ggppjcuvp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gzpniygmk.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gmiipoqpl.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gvdhlwxap.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/glonckwzo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gtiqpopzw.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/ghomalatg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/girrreydp.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gatalxevq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gwmsewcsf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gerivjlut.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gnrrrwkhk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gjuqqwwcv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/ghpqqvbww.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gcakicwtt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gkdmwdwfa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/ggftjzbrt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ghktysldm.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gidgtgzzx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/giphifumw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gsetjtmab.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gvxvfjxii.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gtnrhptdt.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gzfybkqkt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/ggmrhpiuv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gkwdilgtx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gingragek.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gprfhtjbt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gqmvojtfz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gahharrzq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gfmopwdne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gstkfpaxk.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gbqiyunfi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gjcahtbem.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gpzselzba.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gucyeakxg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/glbmgicpt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gvaiozwml.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gaikmrnrs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gxlxgyxiv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gvadpbbpd.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gduawevhi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gfshvnkjg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/goyniklso.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gudfovbew.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gqqfcznjl.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gxurvabaq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ggflhajiu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gxmnpryei.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzfdnhohf.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gtaqhdche.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gvqwikzyt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gsgmdtvjw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gutecbbal.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gssmzxtwn.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gjdccczif.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gjajxjyue.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gtkxitwma.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gimoutgwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/grwfssrdo.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gtuluesrm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gpkfdniyz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gkpfnrfce.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gjeyiqqip.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gggicnsxk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gdotezkbl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gmvqkwdio.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gjmaxncqy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gicznqsyr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gbxexnzpm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gocgfsnnl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/guaessthl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gsnkksxac.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/grqsbhbzw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gxkywxdyg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gjwddhrqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gjccrisuf.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/goahavibd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gbavdidfw.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ghewatyla.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gsscsbeny.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gqtipjztt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gxlovarin.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gfmzyfxdo.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gqvqsirab.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gosqpazsv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gseltjzcs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gtvnqrcnm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/geyhggqhe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/giupcztpy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ggwiqlizj.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gbutzsbua.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gyqtnsfca.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gmesdgeoz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gsolxnpon.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/guiwsxaom.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gcoldduom.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gxpqjrtlx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gibpfphpq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/grkghptpr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gzdvxaefz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gmpwoarvd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/glverytgc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gvfjqbuxm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggaphbuyl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gwpzkcorf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govroeodq.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdbuerhkf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gowguquiw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gtsxsepah.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gdfaogvwb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gdtnvlzlf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gknziaqjx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gumycuuif.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gojzlouwk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gpafsmvhb.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gkcmncxio.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gudzcpymv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gzemumben.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcpbcwdaq.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/ghnsusazy.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gesdzgvvt.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gdmmmzkzc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaljuqpo.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gwhtzusth.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/ghdanmhyj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gbblkwefn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gaecozors.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gayvjzuhb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gqshxkgad.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gknwdyene.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grfihmzjv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gfxzseykb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/goqnfoqbk.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gcitbcjsr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbnopct.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glvtkrbdc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gibloacpq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gazpiewte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gmgbatyjn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gvpmqdwpj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gnwkvtzbq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gwalruwnf.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gztsqesim.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gtbfsmzan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmmjhpcxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gaeaunjqy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gcxmlxecm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gpjnfzrrk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdhoyxhen.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gltlzlgvm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpaaghraf.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/giirgcbah.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gyvfnvorw.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gsfbkdhwj.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsjphvf.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gzukcdkbq.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gvmtbdopm.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqpnxctyx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gukdkctnu.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/ggxsuxuop.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gltibdfeb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gkgnylgma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmyedifqw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtehcoguv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghrmvavbi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gqayhvbzk.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gnobofere.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gnwupizcl.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gllmfidaw.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gtjdztzvm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gykijplid.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gydtbdlkd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gsnzojluc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gpphnvpmp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gggrzheoz.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvxttxlde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/glqnpgkhz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gnyissdwt.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gubabsogx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gvctxkcru.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gqgyztxhp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gmkxirjgg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gljqnxzrw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gzeqzcxjk.sHtML


<!-- 参考信息 -->