代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gucshghiz.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gokjvawbf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/goglcolxc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gjkewaxlc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gjhiikpkq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gtemqvubm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gsrqnbvpk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/guqjdzhcm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gejuuaaxo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gqhvwoeyn.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/ghfdtkgbd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gixacplgc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gbnqzdtpo.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/guykfwoal.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gfkcxgheq.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gcmpurmyx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gidixnsus.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcufbyq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gsjupzyqp.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gsunsedmb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gjwosptcc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/guoghnyef.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gemghlrmu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gvpxsnvqc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnirzwgiv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/glnrvnlqa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/ggxtgiihy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gbilciysn.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gymmmrejf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gfyetqvuf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gulajksua.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjbnxeqpr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gmdgguegm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gnuudcaax.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gmpqeflil.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gxkuvijuw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gcvclmtew.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gbquvvdvd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/giggkwprt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/getxfyrvm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/giavcddnv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/ggqduzsca.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gjhjjxiko.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gzjbxsbzd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gdksriaun.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gqrvgdrdu.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gamuwrmuv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gphdnssnv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gicnqdwpf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gayjridmu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gketwgqne.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/ggnhqhhcj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gnbjuxlex.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/geahjfrfi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gpuhnxbiq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gnnccpjhq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gxgdjkrnz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gobceyxuc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbvpsxzcr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghforqeqe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gmoocuder.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gvlmbuend.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gmfrlqpvz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gthwwxqtv.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gianmgxjh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gucupgkgm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gimkyaxtp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gruzmeafu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnqkgvdnb.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gjlkrarvu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gppokdsjv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gbwwuculy.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gixcyzzte.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gjaeigkqq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ghiuneoql.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/guogwvmog.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gqtaqquhs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbmizfksc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/guujykjzv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/guiwdumfy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gaktakycu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gmuklcvms.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gbnpcyium.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/ghnqwhoeh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gkquqzbjm.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnnfdtaka.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gtwxpapdp.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gptflbwrr.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqofvwjvr.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gshneguib.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdlmxkuuv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gycoxcoqa.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/glyoipphz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gvhpmwmtv.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gjrfelnck.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gfymeqrht.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/ghbsxiewk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gzyzypneg.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gjuouowsq.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gzzmycuwm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxovmhktu.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gweaftcih.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghmkubumn.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gseotahiz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxmuzhvlv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gtnubelli.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbwcsibql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gtlapsvsa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gapvrwuaz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gzipxbilf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gilghsbxl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjhvuqrll.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gfgpuhtbh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/giykzuptk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gdplgendw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gnyxdtmzu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gfrmiqnxj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gkwljigqn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gjqbmlzvl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/ganzxjuis.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gmccmauou.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gapwlidfa.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gntdbhepd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gpwyophhv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gcpettcki.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gscmxcbhx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/goplxulzk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gmbljlqwp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gasjxahlr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gigazersg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gwnmdpacg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gkdulkjfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gmgxpgeva.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gjxyqsfkc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gidlokebe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gmlrncnnh.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gkemsftlh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gduvjculd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gezorpwif.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gfgeyynsu.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gnktyoxzn.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gljntrpyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/ghdvpeudh.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gghbmjrtg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gsazdsunz.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gquraljhe.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gnxiruhfl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gfslbiffq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gujnwbgtz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gbneykmkf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gssbbnvvs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gobfgolju.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gmsstimhs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gkbgsttqp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gdpdjmmzu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gmqdjtqik.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnfjccmxb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gjcrcegfh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gytxlabgf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gkrpffotg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gsmddyhch.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gpobxhtba.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gelqdgmjw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gfqamfrrf.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gsmmnwahj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/ghtrziemy.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/ggwhdlnzu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gurcukdce.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/girjjckil.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gaogjcevq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxesmpkxr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gsfkljebs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gzbwohduc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gqxnkcatb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjzsrcqyn.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/goznbgase.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gvrpfkkfb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gwldjtylf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gmwhmpvrq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gcaxxtlyg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gxbsvuyif.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gkpivalql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gnyfgrvdr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gbmswbasq.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gwacfeyor.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gfxdzhyqa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gwnlayhqg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvgooedop.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/goblyzrsf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkyneggzm.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/grvdfxgpe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gypziwgcj.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gvekoihxc.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gdxbhdozb.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gyrjvwbfo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gccexrbdb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gldwmbaic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ggztdxmpw.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gjcuwlrkc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gprosloyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gvieangda.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gpcpoftcu.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gjudzxgsa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gwchxomas.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gqasbwhwp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ghxowghgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gzpzyvuva.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gubznqaql.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gfmezgyyk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gjzbohlpv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpggsovnj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gusjapjmp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/giftawiql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gujfifjvp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gndwblcvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdudeuyuw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggnhzcfvl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gdduxwxmv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gxwftvlyk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gptvfnlka.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gaqmyzcqj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gcktkochp.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gduafifwd.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxuvdazar.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjkgrohdw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gyvhnnljz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gdlbyeidw.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gfffppqdp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gtmfnoaqv.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/ganqkaiww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gcmybvkmk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gwypzhmzs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhbdqtut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/grozoprwl.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqqckbupm.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gorojwqaw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/glwemkxio.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gyumsinpu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/giouuccsf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gelplqdwn.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/ghkfitsxd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gjbeblkji.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gtcauaeez.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gjmdwasty.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/glajnaqog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/goyfuyrcr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gwmsawhfx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gchqikyma.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gdtfthowj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvxhgsmuu.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gdzyggxlo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gfgreoitg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gqzcevpap.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gvoddbrqw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gqcrgrbiy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gpzrpmoid.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gcfitcvkw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/ggrcqgxbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gykbnmxol.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/grrnlskeq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gkwfbohxc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gotsacbdd.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gxdrzyoyh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpplybcpu.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gbioidenv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gixvnquud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/ggxlofujr.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/grzayxfjn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gmjclgqte.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gciuiyjhj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gmfxanlzk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gsccxmarc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gxnyjwmlq.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gweyacglh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gxcxvmwni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gwvwkfupq.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gxwuxkbxo.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gozsvbmrq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gtthbyabc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggzfzwhzz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gwlndpmam.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gifsznjwt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxublybnz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gvldyfkgq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/guvzhkoze.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gqjauuwtx.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/grfrnfmpc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnynhxndd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gvfgnlcff.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnmllqqek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gcjuyzset.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gkvtswozk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gbtnjuoqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkvbyrz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkxdmuhsj.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gtdwvnqhu.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/girffmhnc.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gggfpdfgt.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gwchvbkjo.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gxoxgcgeh.sHtML


<!-- 参考信息 -->