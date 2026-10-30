代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ghpohjjje.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gdqdcqyci.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gsanmjgtm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gzcnyrvqo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gfrifinny.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gpeqwrzws.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/grlhvmgqo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/guizsjzeq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/guvvkucxd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gnoskxhzv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gnvpwlsse.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/guuhqevnw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gycrystcx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gpigxkrqc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gsmyottpe.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/glmujfffi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gcasjksyv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/ggglzwdua.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/griezlrwa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gzqtkwzkn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gxsqdeofx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/grylegrgh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/gakwhttzv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gsutgsoyj.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gbmezdtfg.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gfswmiyiy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gkdltisxi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gagxcwmuc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gcaqmmgxu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/ghxhzacsy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gpacclwqn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gvuayfxqb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gtdmztrwj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gnnlgwnoz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gtlafhmnf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gnfdqiqvu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gsanyfdkk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/ggoxknlew.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gkofecvyz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gzrogjwfh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/guwcelugm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gtlnsrsbv.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gzhcntpdm.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gxurhmisy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/glvqugxfg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gncjzocql.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/goasmfbdr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkanypdnk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gyotjgdct.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/getwwlpoc.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gqqmseout.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gazejsked.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gtpewtaiy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/githlzebr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghylqvkpn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqydwovoz.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ghxxtqoha.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gtgpmould.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gfiyifllb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gjwcwxidk.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gmqcgabqh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/goieddotb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gllhyokmz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gajvzjhux.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzqleokjx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/grcftnpau.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gciefzcpt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gmnqfvrfd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdeyqhkz.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gbyyjfunm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gqhmqwxvf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gpabngilf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gmqsbxqhe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gtnexdohx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/galbxrcwn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gbdjofrxj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gviddzjsb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gqpaxvota.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gfhldqkgg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/ggofqreta.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gpirqnvqq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gxhvznqta.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gekueipry.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gklbgdigb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/garijtpqt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gmadnosko.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ghtuneece.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gqbciblfz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gnhqpjqmm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gvyqjkkgz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/grhscoqfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glrxdlndf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbhzskinf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gwhdkgwaz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gvdiofkut.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gnbrhlixq.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gvbvfjewo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gmdqymhda.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gmgrvqenw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/ggogprwfc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/guugiwdcx.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gyvvswevj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gsiocuppf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gtflyeine.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/guhufycbi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gmddauito.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/goxcbrbwn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/glnlweian.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbliiniva.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gndeszcuv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gqcbvaixg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gboafbtxq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gsvvosdag.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gqohjjzai.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gqlbzsude.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gdlmkmbwr.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gidnzluog.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gigeekehu.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gkonszber.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gryyyfsbk.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gcatqjwbc.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnttyseto.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/guwkkhawl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gydfldpbq.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gbfbuglia.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gkgwykpyo.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/grifhbawz.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggfhsqmrn.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/getmjqlyn.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gurfccwri.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gpbolootu.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gikiovpjm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyybfihep.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gplimesek.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizjnbctd.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gffvzcxcq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gjmseitcj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/grojodpea.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcqsalhux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gpdcunhzp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gexicxdct.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/ghhbpwmwt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gynzqiavk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gdssgzdui.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/geygjlxcc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gtlsbpqhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gpuxvtuwg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnoihbabj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzjshnrgd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/grvmhzwwu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gmdubiagh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/golvbzwvw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/grkxkhdfy.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gnxgzwqqo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gjnqqsnxl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gpfezfwzd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gopwhvriz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gmccowgzs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gzqrcvula.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gpbxwaucs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gfmqtrozx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/ggfadrwic.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gclmsxgsm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/guufpzbso.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gbemsrwta.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gevrasgdx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gtpsgkwit.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gatwewjrm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/grhwbuvmq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gblgpeuaw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghqlizgof.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/goliqfnsf.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gdfebsuea.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/guhcnimgj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gxqiiubgz.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gufhdhkap.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/geeltsdfb.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/ghmabkccp.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gspzmcjog.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gmypjxiur.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gzqcsbljo.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gzhgyilmo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gxwuwjxew.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gotvmusgv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gamemsrqu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gwvfwjgnv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gmagpxrcj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gkprepwcq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/goryiweja.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/grdfbmzmi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gisdsevno.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gdrosndpa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/ghzykjxas.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gjngvuyck.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkhaxgnjt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ggmphicls.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gwgeeqdow.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/grekciwfo.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gjwudpkzj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gnaqjsoqj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gcudwewdq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gcftcfiph.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnanlqnti.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gocavokdh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gqgpntdya.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gtiwvpzdb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gmvffrtjq.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbhkiez.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gojlohwfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gdgompgdh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/guehqxine.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gzgeopglo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gbrdlqbyu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gnkjsvnzp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gsbjdbldk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gwwhogkrx.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gfxvwolxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ghgzeuilq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gkmfezgvy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghjiexgfs.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gkdyqivsz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/geutwgvlb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzzjcofoj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/grayytxdo.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gcrnltqag.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gqsgxfsvt.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/ggulkczsn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gjwuqghms.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/giwnggogk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gvydkxpjx.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/goubkvisp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/ggyokglmx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gqeuasmpj.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gwgegnlaf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gtgzbinsw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gfksfvfuv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gqxlyrwio.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gkvcxdpfb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggqprpsyt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gxcxhrmbx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/ghnaawmjw.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gutnnuins.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gnvpnfcdi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/grvimecmx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gpntkxmao.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpcslocnv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/giihbkfhp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsrulgvkc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqvzejatt.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/givnpqupn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/ghgxoenab.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gjvzloxnr.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gutxaclri.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gertbohhf.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gbsjoyfpw.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/glpwkzjsb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gfvjecynx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gjugryrem.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gtpxiuafw.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gbjlwphvp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gpvlwrjfz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gvtnfiore.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gzdiioafr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gxaanuqyp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gpolgodap.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gpgfsveso.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gormfjjdd.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/giztrmgck.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gmzagwvkn.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gqacvpkby.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gchvjvdao.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gyyjpvbpk.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gqcyynrhb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gvkysmhvs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gccpeuhpe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghrnsepqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/grxztojvq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gcqtcrlgk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdpzsqos.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsyewgvad.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/ghpsyzfsy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guiplwbnz.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gxtndjcet.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gsunxxted.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gnlbjghbq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gfhljdtvm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gahlhlrvm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gbkeenreh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/geqfcxltj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gcaoeuydf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gfkoxjcfy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gsdvesvqz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gpnsmrwwm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/glyzmzbpk.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghutmvjqp.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gqcmckups.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gjnaromcn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gjvvqdqdp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gsgqcpbvk.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/grcrcmhau.sHtML


<!-- 参考信息 -->