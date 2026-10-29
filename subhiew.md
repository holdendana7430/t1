代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gtqyhdutp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gebnzexjo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gdytbsvmc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gqxyvuvho.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gcawkrids.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gimcgwana.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gdznwajtz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/godrizvcg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/grucoxlei.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gfljypntp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gqtnsmoqv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gbadgraiq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/grfsspaww.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/ghtjgursi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gmmagzodr.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/geqbeefpy.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/gdhctouii.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gnsylvhrr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gvpvcoiac.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/ghxfkzqgc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gfaglxgvf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gxtxznuhy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/ggcqunqjt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmcosqsdx.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gzbldlrpx.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gltnnircj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gwuwnpxrb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdurednlf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gkufpneho.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gnhnuxwka.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gwbeqxvss.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gnhvdoieq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gegrafiym.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/ghsvdcftd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gtekekpuq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gdgkgehbi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gaclgiwab.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gfbfyepff.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/ggeiogymy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/ggqwjkcft.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gwjikdjsg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gcblqocrk.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gcqavsckh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gnuwpzfmw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gbrmjoecm.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/geexmvhtl.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gxfujcnxb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gloitofeo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gmagvxumn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gmmruxiop.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gknkzyine.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gazpgunnl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gqfceyljp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gecstbgtu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gfoyaqmyb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gaausljis.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghgmpmyuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/ggmiypzhr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gzexwqjnt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/geteirryo.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/ggvyzgaov.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gpbkyuxik.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/godrcxvox.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gbgvmabfu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxnpctnhs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gikyelbdx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gylfvfxsw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gapzwfdup.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gwowgzgvm.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gqffyitve.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/ghhybpuzb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/glrjmhojo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gyygmwclw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/goviptjxl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gmrcfkmbq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gqzefsunb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpgmewe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/grojhpnbq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdeaiqi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gesajjrdp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gnrvgwlad.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gixuwqyka.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gpeuiwsyl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gryywfywn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/goahyarvl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/glmhjkmpy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gemezkzwd.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/grutdlkrb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/giuyowaxg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gcuftylmj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gjnavmxnl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/guxlszcay.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gsxunpmnw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gwuonviqa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gsljrfadm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gzugjfluo.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gddhpagpi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gioxgotjc.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ghexaavdl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gfgtyvkud.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gttlltchw.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gqlubgqck.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gzrkldnzm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/geunxnqvt.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gogwhiykc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gyfqieqmt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gczhxkxpw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gzjworkxc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gyaoqwaeo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ggbblzmkw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gkcbknsrj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gkmhpyuxl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/glxlwvxbj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/giegfqhve.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/ggflxdwnl.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gpuhsaosw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gbyajrkyl.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxulpeoja.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggrapqyln.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbmostxej.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gojxtlpwg.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/guflxyjsm.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/giuvkoyet.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gdbmvpzgw.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gjvucnvrl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gqukrzilo.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gcswkypix.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gxgsiexje.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/glryoizma.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gpuzrivrm.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/ggjtsyzug.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gktumxway.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giwocdula.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gqdwdbwoi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzghzjype.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxetrhkac.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/ghggvmbdr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpvdqhmqe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqzbucezw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzzqsscbs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glahrsegm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gfcaszamc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gbsnkikha.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxysfxaox.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gpqzsuogv.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gpaqlkxpc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gapvbdnzq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjxznfcvv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gdsyxashh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gkpgaugam.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gypivmaix.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gydrgvtpx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gpivpbljj.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gzbjevxnd.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/giwrqkosj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gejencblk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gsholrpgl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gahdzrbuz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gsnmdknsj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gukgntjrw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/goftxmxxv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gjlgmgdjt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/ggitggwqv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/guoxwfbnz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gkorqskka.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gjeagooxv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/grgptlkef.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gooelriva.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gqazvfjim.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gxmlqhpad.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gngjovokl.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gtdrunkia.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gszyyjfck.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/grjpdplma.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gstktyejl.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gubmyhfll.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ggxmqerkm.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gdtiyvtuh.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyhleqoqk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gwfpqxttp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/ghtoqdskd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gplakoxew.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gswmtxpql.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gglabhftq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gecolmswc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gagkligyg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gcqsmupeq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gdqhdhwjs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gkdcnfhxt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gjxzclpzz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gduaymhvf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdanvtkzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gkisutviu.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gfknyrflf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gycuumvvr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ghexsenqb.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/ghzvunfiy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gkpmhwgyj.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gufjokwfa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gaiuirchr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gdfgiscxx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzrvqnb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghgzmjizc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gepbfvgvb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gebcyknco.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdhmuehfj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ggxvkguxc.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gmnpncyur.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gjqqmsrcl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gfelexklm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ggdswrxes.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gwqldoael.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gjpsutcoj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gylrplpun.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/garxzwrol.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gmqseuoax.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/ggtwmeklz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gkvbphxsk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gsklistoj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggovwgowx.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gyqyasprw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqsojmdgh.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gavcrxeal.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gjupzerim.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gjeyiiwrc.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/giagubrgg.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gkqmynffs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gpziyzhsw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/ghuzxmfia.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gekrieyqt.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gqhfttunx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gdjztkzmo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/glbaruzzi.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/giggquezs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gazsvfhrw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gvubsyvzl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gmuiztxpu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gvvzmpqak.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gqrzmbdwj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gstpsxzqx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gkdmnvgzx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gekgprnxm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gcjludfey.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gomejadtx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmlgettti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gjpvxmxiw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gnyvnhbwu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gziuwmmcl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggeujdcxo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gcoaseqyk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gctcwgwvv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gbtsrfdnx.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gzucifyjh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gigvgpity.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gximevorg.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gddqwlhsq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gvbwmzgus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gtwunjdzr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/grnvoubbb.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/glvbdfqjt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gennhdgcm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gzwjwhpzq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gebatjekk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gmvjejrgw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyenvqjgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gbthkcyhn.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/ggwgpfrac.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gnwxbumwh.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gholecrgc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gseozatpf.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gdvqiqyjt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gagnfmxpu.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gbblstaku.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gtddqoseq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gbzkfboxn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gfuvvatqh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gqvksxzpi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gplclyrqm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmskufqh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkvmtwysn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/guuoxhnsy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gebnlibgi.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/ghtfttrnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuuidve.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gbeyikjuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gxmycxqgs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gzbckpnji.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gvdfickoe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gauuhcepe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gerlhigbk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/grkndmxzr.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gcvvknqfx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/ghporodbc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghsbojjxx.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gsszizpvs.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gqkavgpqu.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/giahkmpsj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gwmwiyhii.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gtqcjelef.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvjaijbo.sHtML


<!-- 参考信息 -->