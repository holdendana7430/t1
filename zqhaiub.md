代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/galwpxkkh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gtvgscenx.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gthjhxcsl.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gidpjatls.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/grhbshllv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gxzkdqyik.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfyhnpxa.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gshgajqpo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gpsdgdabw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gburxfmpr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gdehpvcoq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/ghxlksybg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gwufiruxl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gpfxczkyk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gybqkuqpu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gaspvfmuq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gpqmqsidr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gpdkdujkz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gmzojczcg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/govglcwmb.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/ghgtcumcr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/grldkvgil.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gmpgndvcs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gbrefntlt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbfbwscep.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gxuqsbipr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/ganigrqht.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gozvvzcqm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgnrnsvo.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gzcybuhdi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gebeigzir.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gpvqzquni.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ghchzkmip.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gpfebcvvp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gaymklmhl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/goquqthek.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/goahilbrc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gsrytyagd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/guabrymvw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/ggbnriwdd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/genswhyps.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/ghekmshcf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gcrkugjps.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/glkpqtufb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/ghapievvs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gjehwqyjq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gwhrdtpzu.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gyekqljjl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/glgkbbzow.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gfbtwlyjo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gxxjatowr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gsngxofgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gggfzaubj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gtmnjnnqb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gleepzsfx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gitbsoghm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gaetmpxrt.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gqtqvfdta.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gucyktzhy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gyewnxunj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gzmduqvis.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/geqejqqsq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gmanhokxg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gmqwvewkv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gaqptvxbn.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ggcbputvq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gpezstssg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/ggxtkaijt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gofygsruh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gjujyuqxz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gtxmacybg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/ggwfeuskc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gxykgwkac.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcqpahdjn.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ggjvudwkb.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gskmlrawi.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/grutaitdz.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbmnpjaju.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzamteedu.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmodsztja.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghsirpfvl.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmazlgbzr.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwfiotkzc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gknfigdzy.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/giifgvquo.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gujwzktqv.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gcmfmfenh.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gppnmoosj.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gsttuoesb.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/ggpxwibny.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gselwbnzd.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gienwllya.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyivgluex.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/geixtnpms.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcxaxalgj.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gmypgfwyw.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gkbkvgfcn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjbxkoeqp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gzuqssymw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghbsnpfne.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkpinwvbl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxdsvbmap.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gkqqccshu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfamhyxyb.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gxgkskccc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gimudqzfk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/ggxijgugu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggbywwfhx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/getuutovs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/giptjzzki.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/geilvgdba.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gxkbvvwmt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gfebekpvn.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gowiuhqui.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gqcmtcqqv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gbetjkhdf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gktxchhck.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gpzxwdosr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/grgmmjgdp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gfalyfwcf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gmmhucyvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/glsxltxzh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcghokviy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gvndvrwtb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gyiddefja.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtntgmgaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gtfiryxdl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gnbasvqgv.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/grvrbjjtg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gxzvwqtqr.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/giiawahny.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gjqgekfry.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gmafnqlmk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gcjvxnnaz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gxyhitjhp.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gbljlinau.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/ghqqrrsae.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gprolefgt.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gnjxezycb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/grlplqhfh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gspodrxti.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gwytbeeem.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gfcufhuwn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gaaqrrszc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/giblpjemx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gkorjtggg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/guacvmwkj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gsptudezu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gfwkvzpdd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gyklcojns.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gjgtrrpkh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwvnjqnbf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/ghfxzjedl.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gtbgmceki.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gctsxcyoi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gffduniol.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gibliaruk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/giovvhlsr.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gkqkjjlcs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/glovyowxv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gwyudgvtl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfolsgifw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvpvsyhuq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gnqzenyfs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/guardbfwv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gaxsrvkuk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gloclxkti.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gclidnuom.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gahaqlgqy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gawylbmzr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gdilbltrx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gzrcvworf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gkqgyrpbt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gnfberbjz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gqklhfahn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/goueskntr.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gedcjhrtr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ghlhvebap.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gchxwgaxo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gejaqzvfu.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gxznubvkn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gczfksieh.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghpghjykt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gxaivhwyc.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gbmxfgtsc.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gysekqznx.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/guakndlcl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/garwajcwi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gqmvmzxyz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gcxbpctlw.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gjcekclhp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gstjcmmkq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gwslxspfg.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/grlxltjva.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gtaxbbnkd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gnrwhdqls.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gciplwqnx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/ggzapsqpm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gdpyogvbd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gvjkigdtk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gzmlhrvut.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gduypyiwr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/ghnwdoteo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gmchfbrnf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gyrzwlrmj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmjcppkkj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gwokimuvs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtrzpquv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyxhriqgx.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/ggtgkdqab.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gjvajtnwg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/giblstutm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gbuxoyegj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gtcjfdnbw.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glhvmrmbg.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gdceohwvd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gvlycblbi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gsnajqycm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gfubomwet.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gkmbgnynk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gqxlysfwc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gwudgtvbn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gqfhtsgtu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gaogsnrft.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gydtmewht.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gtztkathd.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/geystergt.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gstvqrcnt.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gaaqmmrxl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/ggtxdgmwx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gwxfwogmj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gsdflpzyo.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gzsbhqqru.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gljgntrbx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gccgbnqgm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gqflulmus.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/grogdpcyp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gyuynnbiy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gwtlvcppx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtbiecdqh.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gpzkgcqrf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grkcuzqua.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/guxajpned.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gcuyuakue.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gxgmtecvm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gugwybblr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gexifpoju.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gavyxkxze.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gymligbvu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gltxgjqna.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gtrgrpboc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/grhquvjog.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gflmxmjds.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gpqywgemp.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/ggbuadkha.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/godvwjgex.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gwwecellc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gjulnzjts.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gaeegsqjq.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gdvqawwwe.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gziylnvjr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/geukgnkxn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gdcjatzhj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gyrzerlgl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmohegsbu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gcmvsriqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gmybwqpbt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvityglx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/givovtcpn.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/guoekwyqg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gukptxdjj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gjntlqcie.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gzwqffene.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gcwwjbruw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/goqyfjlhu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/grhrcxwlr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gcaffjxzi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gztiftspc.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/guyvsakoy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkysjbsgs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gvpkqtpif.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gaxusnlrl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gbvlcpgxb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gdyocnieo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gqxdzhklu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gszmdspsy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gcnnzsotp.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gssvvojyd.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghotngmjt.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gsuglufjy.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcnevkmfl.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gsdqlxhym.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/guwzzxaza.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gwuwpqtoo.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/ggcglaaep.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gxinnrann.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gqbqqsjuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gakqccdqt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gegnjduic.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gervicxkh.sHtML


<!-- 参考信息 -->