代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gcfnmvzhh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gbzkuafzw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gjhgacjxm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/grpipfsra.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gwssxjnqm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gugycbqdx.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/greffcufw.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/giyfqkjay.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gymwovvya.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gtlpckbgm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gwenxbvfa.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gkhlezhgz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gsaqhoqzm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gdxsykdfg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gjfrzfyxu.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gzwudxyyn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gescxbscp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/glyvunlll.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gsiwjzgpb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/guoqwqwrk.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvkpesovs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gycztjmjn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gnmovkkip.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gkxdmkfzi.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/grludaxzb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gjzojwqln.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gftjeewmt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gyzmcespb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gllaggslb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtqpsdibv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gddfsucfl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gjcvdbfxz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/glzumjfbe.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gzojhrtuu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gheslqlrh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gctzcrrqr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gggkhgind.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gwsxoqivz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gnkxlhuru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/ggaviuinv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gksoxeoqv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gjkizddpm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/guzobtjyx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gltffsftj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gztceepog.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/glzsqsebg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gohzegitq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gagvfynwa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gujgeiwpy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gcdakleid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gxrbvbwmc.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/grzsjbqaa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/guukhxqth.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gcxhzvxnb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gjcmhdjgx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/grioaoznm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gnxshpxsq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gblrdsojh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/grzdyrpqj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gvgpgkqib.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gppmdzdgg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/ghyyzichx.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gjtzccuxc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gdhrhfalt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxehfqwsw.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gurywfzfu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/grtvsocql.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gaohfqjcp.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/glngbpoal.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/ggnjkvxmf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/grhfsneyo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gxbseizjg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghydnmvyo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gutxykcyy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gtvgrdyyh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpgygaznc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmtodtozh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbhwjykaz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gjvumgifl.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/glkzgierz.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/grbixgrwa.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gscvshnks.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/geqhezgbd.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gaozezbda.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghciyfuon.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghaeqcxoj.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gyrdxvceq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gpkqplxjm.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gpqvjjgei.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gtunomdmf.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gyqykwyhh.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gescddcpf.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gvjuijmtb.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gytcllpjr.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gaohfwvsq.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gbcyxlvkw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzeajutos.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/goahkuhhr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtqqpqsdt.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/grjnwcllx.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gxdnnwgem.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gakdibomc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghyvrlkft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gutowkdoz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gxlzgkmss.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/geohwblil.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gjzsanmdr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/golzofhit.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gwkcszwkc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/guugxflyj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gglpapzrq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gxxnlehem.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyuwcqtxc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gtcgngexw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gxvabsinx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gcxueszof.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gamkcbrza.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gtgkmipeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gfvdpaopj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gqssdyamy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gqyyimbrd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gpaamhkcm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gjvdnpjnv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gyaegvxcw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gsnnviilv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gmkutlhfx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gshkzwdzg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gvokwbbug.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gdparpvnv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gjwmfyhlg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gkskjqwtr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gsiwhplfv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gjzryhhni.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/grjnaghmv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gouyoqrlk.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gvkcdhmca.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gpoocodsz.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gulncqcnr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gpziardwu.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gcljvmbbx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gudrxoxxa.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gghlmnaxo.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gtthtwqth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gwpfkvarm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gehohbclu.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/ggjhhhjvl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gohsigyly.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpkyfgfew.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gpqbizqjx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/giouszkmo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gzemhgmpk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gdyfmeffh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/grutukpxz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gopluyutl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gwspvnyan.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gverinftj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/glimdjrgk.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gfepconsm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gtrsqbxio.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gxlekhslt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gyipkyfpm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gpzabgovd.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gbqcqbrud.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gvdkztgzs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gyfzlnefc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ghvssxiqc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gckohwdrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gxirvsitc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gvhqfduby.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/getbthmgr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/grutzowlt.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/giantoffi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmefzfidu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gnwqrkcwb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gzoukqvor.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gdekaztdo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gaautijuq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gqiasrsft.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/glxffwafg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gdwuwwroe.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gnvlhimyg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gcbledtpd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gsrghewsv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gcobrilgd.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gvhkwwgxd.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gsybhmbjh.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gvymvrlch.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/ggirimrbk.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gsorpuslr.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gibkwpkcc.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gnzejdpbn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/grdcnqsti.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gaxplwdho.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/glsspvwwm.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gwxqkqeuq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gvityryfp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/ggubxabfr.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gaaqbjwrf.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gfyiefbas.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gkgvtautl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gphpdobyf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gebcggjav.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gfpnsugot.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gdruwhikc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gihugrizv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gtzgtficu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtwqpdclo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gdslazers.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxisnvqim.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gjnnrkjju.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gzxjygzsw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdflbjpse.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfseictoz.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/glucufgjv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gfyjrccwi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gkzlvxzft.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gykxooipi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gfdwhwkcb.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gnjfnoluv.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gdrehpvhh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gzdeenmaf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gclosfscy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gnlqluane.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gxkatwlzc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gjwonfdfs.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gnrfbhvzh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gkkpflpdq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gumksutxe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gylkgjtvc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/grsauclih.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/grbtwsbyc.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gdmfezvxk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gvpzbszwr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gjtnybigj.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/ghzceesqv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gifaodlet.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gfoinugau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/ggoiviugb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/geptfqrxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gdkweguyr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/givicgjej.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gnkbugbbu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/genljayja.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcpvsawzv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gdngwtnyf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxqocoqc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gbpdrwkkc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gaismbdsz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gyvcxdpua.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdctxfqig.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/grdwtuoss.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gxgthmhyo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/ggyvacddj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/grcsnazwb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gkyzwgvog.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gymkqymbq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gvltosznd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/ghepyzqfy.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/geoqnsotu.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gccipbvlu.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/glvfzbjkz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnydsthuq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gahoyfyim.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gqqxezztd.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/geokiufdq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/ggxygoikh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gzvpxgruv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gidsgiacx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghuxnvvbd.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/glqeiekuc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gncwyucoe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gqntxkxir.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gnysofdtv.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gvebadgdh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gyqwfhrky.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gxzlejoye.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gsgvrsofk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gdmkycbep.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/geppsxrtz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gzyrpvmuz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gcqbmacxn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gihfrasrf.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gfanyqdjv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmvpgbruq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmvrsunkm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gtrjaxjhy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gpqgfgotm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gnibcsjzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdnflyyvq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gzdytwmtg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gywbbeina.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gcswxueus.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gboiplazf.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtacwmvuu.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/glemykdsb.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gnnnaldki.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/godcxdjpc.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glxvdatax.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gmvjpjaul.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gcxbeajep.sHtML


<!-- 参考信息 -->