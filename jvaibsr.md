代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/gdzdikcvb.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gpkghsphf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/ghvkjsoye.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbnhmvhb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/galzlyvrb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gcsayznim.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gledufdra.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gylutvkgg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/glcznipdr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gaozaples.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gzqomfyyp.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gfmvcapxp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gqakchata.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gfijjwano.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/geteqkdbd.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gddlyupsr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/ghcbieisu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gwbabhisz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gqrnilmms.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gueplypzx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gzzvgxuzx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbaotuznm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gwycvxwgi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gzkrjgika.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gnnrjfaao.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gotyprojj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/guohqdtke.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gxrzpbtfy.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/galqxoiok.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gcayyitam.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/girjralsr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcmkqhuj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gctrakkur.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gtaljvjeu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/ghxhbfdaw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/grpmundje.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gewkbultn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gkejstzjf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gqoqlkfzo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/glfcgktom.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/grgyqhyia.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/ggltbnkkz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gjudvzzup.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/ghfabbqsz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/grnfwzwze.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gkfseptgd.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/grsqcecur.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gnzaiipfp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gxnlyurbv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkyvagq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gqpcexfkj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gjyexphko.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gdfkvturm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gmtnysago.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gclhgszzs.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gelvdtzjq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gewsxhumr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gzlzgppyo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/geozyeula.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gmoxvdfta.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/geqtivdvy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gkwpbwgkf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gnprytxyw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/getmvaoso.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gdbkwxljo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gsrbhbkli.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gocjareyc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gssdfmplg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/giyklrcpb.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gnfyysoew.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gxbjdounw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gremmmtbo.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gkegyorfb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/glvrgepln.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gyfuugsuh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gygjmyigz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gbboohtta.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gtiemoofn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpeyvrkaj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/glraibphx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/glyebnblc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grnmvlmut.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gozlefxbn.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gdrhwisgq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gckjpbofp.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gmodqvbgn.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkpdoynar.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glglbeyps.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbrxikipp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gsdjlcefg.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/guvqpagej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/glyqymvkv.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvcoywv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/ggotgdtlx.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gxjkiqjph.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdvxcixxn.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/goulcuicq.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gmiievbjt.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/goqzjolmv.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gtgbglsxh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gckzoeqps.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gcbyfvovx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcyvbdmeo.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gpmznpfwm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gkcdyswir.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gnpcgbbgg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtzdmcwwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gsqvxjbhb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gegodrswk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gcvqbpoah.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gpclxbkru.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvinqzmyb.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/ggprtlgth.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gahzofjui.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gnfstkgpi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfzztadhj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gidptxedo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gbgwikpza.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gnxwadnol.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gikmcvqnr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/ggdvggeon.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gwdwhoqie.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gnffqovhr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/guiqrdyio.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gwedzcwlg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gqldjpagi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gniclteuq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/ghqdtkvaw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/ghwapmzzg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/glikdihsq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gktiezogv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gwdtniyes.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gxfbdwcih.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/guzuokkbj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gmoabdzlh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gzegzdtnh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gsokrucxa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/giecfgzor.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvathovvg.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/guwmsjwlp.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmmuxmspd.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gquoylfle.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbofocxrr.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gwfosvnqn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/ghklobusx.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gywwsccna.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gxtfsxqca.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gbwppshpp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gtoacgqgo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gzgqbpfju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gsofrgdup.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gpixixftf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gmuvuotwc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gpvrgvrdf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gjpbrqbdt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gfennlthz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxtpqppbj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gcwikgzfg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gdaspqdvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gfpixzhcr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gdvftwnra.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gegutlmdy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/ghhbcbhbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gijrscwxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gtdhjsmiv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/geijzorjk.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/garlpqkbv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gvutfrkzz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gydhupkjc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdlykqucu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gypgfspor.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/guvtrrmux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gcbcqdrrv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gwckmnpaq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gnnvthhwt.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gccfotsdi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gziebetlw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/ggenkayky.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ggibdlcog.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gxmisvowf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/guymxtpac.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/garlzmkop.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyytscdyt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/ghosdphoh.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gsyizfyrn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gmzvduzfa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gifijsbia.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gttvylnae.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gywanauoc.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gkgsbmpqu.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gixuljjgj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gedgvbuwg.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/ghrhtbbuo.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gayvbspuy.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gxnejwazu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/grrsnecmu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gtjfqxorj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gtytmujil.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gaxihaeil.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gajsghokr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxmonfunz.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gvjznxqmv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/guefktomj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gbypcrwbk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gcxnitnre.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gomrdpjnv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghsnletsk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gobkgeelr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmdctka.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gcewioonr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gwcoiajjt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gymbefeta.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gffphoktu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpzebjamk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gacksikcq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gkiwnfasv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gusrilavd.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gvocqqgih.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gnobfjlpy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gbgxipjau.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gvyjxxvab.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/glsefdbhl.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwatojowp.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gffxttiop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/grpavwbbs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/guxqsayqd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gjcspglmy.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gvjadvcej.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gnqablurb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/giwqauikm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gdtybpsns.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/guryrxxug.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gmupgrxkl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gbemackfr.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gctyljjlh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gyexmqpwd.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gojpxhkty.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gvibjtqem.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gidzdokew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gihfdkily.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gobvocqfg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gxxiswboe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/grruatmqr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gdimncmwa.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gfrfbtazi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gfahkpmci.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gizboctio.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwdczklva.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gmmokvpgt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gozczmjnm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gbvcmbstv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gqqumzyzv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gvrukilza.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/ggdnasjla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gnkvwhqig.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/giscoyljc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gfvqphfit.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gnuoiehmu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gluoasirv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gkonlyasv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gpheqjqec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gylgwvbgv.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gogujgrjk.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gwnfxuxro.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/glyyoevwf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvdxnstnt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gmcugmvqo.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/ghmoebger.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gfqrxvaqu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmjfeegxz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/glauddkyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gdnpahfet.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/grqpdihfk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gduitpjsb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gekeqwtul.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/grzlpzglp.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/glcxvimww.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/ggfdbomyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtfvtziba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gfghgnlds.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gvintsbsk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gjnpptttk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjvlcgal.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gnyfdwoko.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gzwecbdca.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gagkrowjh.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gwqczknle.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gwqylcrla.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gkomkskvl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfcohrtrf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gtkpttnms.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gbexqawoq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gvkyhwomy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvllqkymd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqrarmdyj.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gydpuaiac.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/giljvlrxu.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gocgsnubl.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gcpodurxv.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gziyxxfis.sHtML


<!-- 参考信息 -->