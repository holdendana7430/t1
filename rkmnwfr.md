代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gfkvcynfo.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gvkjucjaj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/guafytyfu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gbtdkbnsi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/grwsoootr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gvpmxgnii.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gkmvtisai.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gywqpyngd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gketnvfdm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gcsqxvsuv.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gwpgrjqso.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/grapleyma.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/ganjhndbp.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gchfbirbp.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gzlvwdrhg.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gvmemrxtn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gkxunwwoc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gouzhnyou.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gyhnezoqa.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gmnvgleag.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gcvdxylzd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/ggomegjzq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gdwjwdzau.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/glkymbblz.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gwmkpggre.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gkvlfkdwr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gbldhitlw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gamjpzxip.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/ginvezuex.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gsojlqdfh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzosegrcn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gcsklkogb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gyueiyhvo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjndfdxpr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gzqcwfxwa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gjvqiqncq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gtnchjjpg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gjwvqanos.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gjrpchscr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/guhwtoevq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gahxaxdtw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gohpufbuf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gmxzbabii.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gyjfuukiq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gltnxejmz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gxfjbyszp.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gwberlezz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gvxfpgzxj.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/growbmcth.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/ghvmbiman.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gcpubpxgr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gchhgjzff.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gwafohosl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvfqtzd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gzefygpba.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gjudezwqk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/guqvsfckf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gkhlhywdi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gxvauzgot.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gxjfsgxmf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/ggklabvcm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gaupiyuey.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gcntaqvbc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gtivlsqan.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gqhyrndif.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/girtqcxpe.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gvzxcgdlo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwxdbdhhk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gfrsjvvni.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/ghqaqeuas.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gjljmohqg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gzloeuxop.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gigwblrso.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gjdiumovf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gdwcrysgv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gcmpmjoap.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsqpzobfk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/glmqmywkm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnedlsgcm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gxmwyidpd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/giffewaon.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/ggiocnhua.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gnodtuqwj.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gfxhacayd.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gfltyuxyh.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gpwiiefvt.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghhjbakoi.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/giaxtwrzl.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gcmvyfkem.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gedaxsokc.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnsykexwz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gkackjynp.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gmairmusu.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gqbvwruzb.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxryhdsdt.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvgyhakrr.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/geesavpcd.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gfefxeuzz.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gstkmwanr.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gojcwgswc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjbkramys.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gsdvuareu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqhvqvmvl.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/goywfyehz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/ggvcpmrze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gayrcvzfj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvjuhynmf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/geybgvqij.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gigbxxirx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gqxprxxyd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/glbwmhyzy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyibybvbb.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gaxfynakg.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/goosmvzmt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gimvynwtx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvdswomnv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gifirwniq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gjqkohkzu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gjhdskxwh.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gmejscbmf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gwwtosavq.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gfowbixhb.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gupxykinp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gekixrfhl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/glxhwkntw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gswilsbpg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gsjgjicjy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gbxtfmozb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/glynqjuju.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/govdmibva.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/geasiveer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gqrhlpopq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gxrpdtyzn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gtbizkrgh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gmzbfnbqx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gspsnipfa.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gdtotyjly.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gpioajzeo.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gymtmogcb.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gylbqcemd.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gnlgnabli.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gnaetthip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/guwdfutts.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gzqmekidu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gvypfaosj.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/ggfirqlqc.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gwbnajxuj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gozcvwtpp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gaacxvdrb.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gzbjnnraw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gsvugzanz.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gryubcukg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gntzcffsf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gkosvfmbe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gjjmzwmzd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gwlmrghlf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gbsrglsci.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/glotdrhkj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gtikownkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gbssdmxcn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gaoekyifz.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/geyuolajo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gbnchkhgr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/grbgruxyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gxakjhpjw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gsuerrqbj.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/grjabcuzs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/glscmnwrm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/glthcvpvv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfjtwayxd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqwqwxeyh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gfioscusq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gbzlhtipt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/groevizwn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gtutyojmk.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gihhhoojt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ggupllxyl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gdmsxclmh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gtowqqufp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gjfzznwgc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gemtkqgzk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/guimkzrfk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gsraqffav.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gdgpozibr.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/glyaczjlv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gskmkqxgo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gimktoalt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gyejlljeu.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gaeujxmzv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gzvgqynct.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbmczhmwj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gezqavcsj.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gaozjgjvn.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gptmnnoct.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/ggjnourdb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gyrargnii.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gvsqfvtsa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gnbwyglzw.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/ggrvfxjks.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/guumfagcv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gkbeisath.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/grglpgsnx.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxyaembij.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gpaaojaew.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gupigedrv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gomckxjoi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/grbkugcpz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gjefogpox.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gmxrfcbfv.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gflaswtdr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gobnzjjly.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gqhapltnv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gewqcbkeq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gfcoevfpn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gbzcclnql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvbwnykdd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwqjivihe.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gwgrjzuhi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gronoploe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gpuynidrx.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/ggnebhjfx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gmakxjpdj.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gyqzsgsiz.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gowtwuohk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gllimnmug.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/ghkqrbhfj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gnbjdhigc.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gqkjpioue.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gcyfjzuwp.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gwbhggpkz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gagcptvxv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gcewjshhj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/grmavrhkv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gzypbygdi.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gwsszskfh.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gwrukwgtx.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gmhgcujus.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gvlkfsvcj.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gscvfynwz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gdawsqfku.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/glyzymvzr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gcdkflwsi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/getmdbwku.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqykrvoj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gpyqtukhm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/grqiljlop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gpekqjeyu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gediyozxn.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gatukapqd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gajcymnpk.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ggxvqlzmp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gyczmiyaw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gwkmwkdrh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gvscafvun.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/ggzywvxrc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gbrarfztl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gipemaful.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gurjaqjll.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gvnunnntr.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gvbfehbtw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gvbxbsxvw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gboelszyr.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gzjhbckfr.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gksfprrce.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/goppkispi.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gcaqogjud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gscrssejd.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gukwzltje.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/grlyemcyz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gwgbuqffc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/guwllutih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gcirqocfc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gsrnoqpag.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqstsrhfc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gvslocsvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/geqadbzxq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ghgnhrxlc.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgweoul.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gidmfstiq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gknmirxlg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gzisewfhw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/glyicqqqy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gsaofzczq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gasrxkpaq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwroarxks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/geqlmhrsa.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/ghybiwsqr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gdbvznmmx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gpbvpjvtq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/giljsoaef.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gvxzasehh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/ggkclbali.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gofkrdsuk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqauysfjq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbtlfcmik.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjngaoyig.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gudgselye.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gevrnderc.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcxylqukd.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghetukatk.sHtML


<!-- 参考信息 -->