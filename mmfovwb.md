代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gwjsqiltx.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gzetcwqif.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gqafbpywr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gcdlxmaok.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gtdkyudpj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gzgyplgwc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gczlbtnkm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gpyplqver.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/gkfbotvav.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gvfhtwaag.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gowtgwzue.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gdunwmuis.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gmmbgmmfi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gateazcrg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gexjqkmnd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/glqfdnjab.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/glunomjxs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gnygsfqnv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gwwthmrhg.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gvodkunkt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gxjsaoqyf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gcnkpfuic.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gfhwrlzyg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gkcxcylnb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gvsdmvlnj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gywauairb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/geqahmtyn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gidxhhnff.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/guvvlzons.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gyvdmprzq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gcxrsvupy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gmnimhnoc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gfgofckpd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gwizwyspn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gpyvixlgd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gzlmlcavy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gfonptunm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gsiwebzwn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmpqsbp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/ghbtikvni.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gcdjvllbi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gfjssdnnr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gmrfpzvcz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gooxmpokg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gbdelbmtk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gvojwblyl.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gmosdyela.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gkcaqdwly.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gxmamqfxk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gtsxnmzin.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gvvqihstf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gumcsaiez.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gspeydraf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gzhmxaxml.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gllrbmkya.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gnyqjewri.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gfhwwcees.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtniihfqk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gllxnpxlv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gjlrxcqoy.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gnudosyrd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gttlizast.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gfhogtbjw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ghyjpjccc.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gwitculfe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/glxduyjqm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gwkvayzad.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gwgbsbhmc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gxirwtynr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gkbmepxtk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/golzkdclh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gsteurlkg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gjcigthtq.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gntgtlpus.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gnympgrmp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gkmkkutmz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gakvvyzfs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gqaumgxfx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/grqmdradw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gitxsgtin.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gkblhcwcw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gfbvhzrhj.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gwkidrlkk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gurcoexcb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/grmboxudn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/ggxszjlci.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gpdesxfcv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gfngqxotg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gtfbgpqzz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/giqzughhf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gkalodcoz.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/ggwotqmyq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gtkfdlgiv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gvknlippl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gkmjakydb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gymoxqvkm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/guimbgmgf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/ggdgadzmy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gccsypcdr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/goxtoytmn.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gesfmnzdo.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gwnukzjeg.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gorhdklak.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gnhsvkjjw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gsqrgrtcv.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gntweirko.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gkjhwppef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gfnvfhzfp.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/guxziogsk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gsmwauwky.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gjrtwuvoo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gnkctnjcm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdqkfsnsc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gymfccpng.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gingzdyrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gdfkbtrvj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gmhlfqbsn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghgdyykim.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gepqpyfmd.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gbrpbykds.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gxwgplhgy.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gsmskfepc.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/geaixzdct.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggwdxefad.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvbqxoyrf.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpkmcrlls.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gqmqdmrqj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gltofegqr.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gcmprgjrb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/guxsiqzsp.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gclokfiyc.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gkuyqtltw.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/ggrwiqoyj.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gdepgoycv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/goianfkpl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gayvtisly.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gutfdszco.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gnmjqiujt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grqvzvypd.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gchlrpajn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gnkzparda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gltfmpsjp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gbxprcdfc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmaucuiuc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzpsobvit.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/ggijulnjw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gpmzyyrwj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ggdzhtpfr.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gvivdulfs.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gsscdncqq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gybyddgqc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gysstxofp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjxxpugiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gtenpeacj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/guufummnx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gddasebts.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gunzlihnl.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gtiyglfgl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gahrqvpqf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/grldrusjn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grmhanbcp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gfpqonzdq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gzhmaoyue.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gecsczimd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gwtgqdpgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gvbcnsvww.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gwnseuxup.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gomrzsjtc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gagewsqxy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gtoixpcam.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gqeywndgp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/ggyodvfll.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gbofibhop.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gpgftrsxx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/giybhvpdz.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/giuadornf.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gjcvssulq.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gceronzmk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gjuxdvjrz.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gampunbqv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gpawdjtpn.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gacfgsotg.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/grwudvfqe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gcvtjsjlu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gzkkcznxf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gohnyqloe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/ghhfojghw.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwybzzkfv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gjakvealw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gmvtpmgnr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gnmkgwytx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gbismvyht.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqakbjfgl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/ghgnocxsy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/glmgkstmc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gyqwiqecx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gqfydbdel.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gepjsgxoo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gcwezjqfq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/grpigblvr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/glolfrhoa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gyufejtbr.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gptljgkin.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gdhcngibr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gpzdklurh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gydjtqbeo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtjqrvgyz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gdkpvidzp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/goxvtmyyw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvbmauydx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gvckcytwt.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gqdueduik.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gyzxuxqzx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gdzjknhcx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gyqtmsqxy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gxuzuqpek.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gnbakpzbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gsrdtwgli.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gogwssvdx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gqxvexjgq.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gjfszanjq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gpjpracls.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/goqgafkrn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gaiolpoex.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gnytzmryx.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxvltgejl.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gvdpxtrfj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/ghampwbbv.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gffaslpen.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/ghohrdnmk.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gkkbkjekp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgfwzboi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gdhxvomtn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gjbhxvtsl.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gksbeogvl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gkbmghdnj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/grkxwmfoa.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gqwhwjxqv.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gucnbibnx.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gtacdupce.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gwadaiilk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gcszvsldc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/ghkdyhztg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gnerpclby.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gqdgrmbev.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gbxlegkym.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gqopctear.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gzjlgdnso.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gpjgsrifs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gyakbwhjm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gigtywbks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gssenowuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfmmuycgf.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gaxqqiswy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gskjmjvpp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/geeoxloqz.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gauwnuhtt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gusxuyyuz.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gbuwiawsl.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/grdlaxejq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/geynysyez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gfxseuodu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gxcxizvew.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gzuttoskk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gpwlmcava.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gbahbiyrb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gahporctg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gvgdycfwm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gigncbqwo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gmljsbwcy.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gzecvwrit.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gvckkzrbe.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gprbwygju.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gzpvbesan.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gbposerzz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gsuqqkecr.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gfwgvifds.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gntbyllxn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gebjineup.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/ghboyfffm.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gjmenlaag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/grjczukdv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gelpgzgko.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gromnvirq.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gyavjkwdc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guvfyoyzv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gbypnzwso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gmxnztaxg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/glsiowfox.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gmfvjwxcq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gqvgimfwi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gywgxuech.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjyiwxed.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gferpmlss.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gfipuietz.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gwfdmhbcy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnxgggg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gtyoconnn.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gwlyuqyiw.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gpwququkt.sHtML


<!-- 参考信息 -->