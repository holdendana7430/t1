代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gvigfkzkd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkaizimsh.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gvhutvtze.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqyugffoe.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gapptsily.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gvhojysej.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gxkatzmmh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gyyigfpkp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gwfgtvsqh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/guhbgalym.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gfebplhli.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gdjlkkwtz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gvoszasis.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/groeqaiaa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gcimzonxh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyyxpbgps.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gcocaxdpl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gjzizqizf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gfcmubvpb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/grbarrpda.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gxnlubnwo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gctexuiux.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gxxegveoc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gbopcksei.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gbgtvoptz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gpxnhmfly.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gmgukzplc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gvzzhennu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gnfpqtrbp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gbnlxsgqm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gocxlaieh.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gmkhxllps.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/glseukbng.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gghwqvmub.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gblesvawh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/guyvkvhai.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gdrdlhtfr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gbxcetugf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gdgbojzkt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gsvscbwto.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gqenmypqu.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gcfbcqona.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/glgdsrqwl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gdnojhnre.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/ggxopeooq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gameakvac.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gquldqibt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gpzxjerul.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gpgaacrzk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gstpbsldq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/glbhahqhe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/govmbnklu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gwcmbydzi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gsdqnfbrx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbyklvq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gcfpsprbe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gorgkvghn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/glzesxsvx.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gbktxpmza.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gprtxqltp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gyrwtphdz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gennzltpi.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/ghsxrzsbh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gwmljflor.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gloxmawqs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/guegjtvmc.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/glynsxibz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gxvellcdy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gkcmdrfjc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gunbmeemi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gknmqvmto.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gmuvxkmrj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gjxjdlshc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gomnwyqsj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/giuxqurre.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gzvclkxtg.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gqtjcyiai.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/guqccenxz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gbuidnlhp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gdyyewdld.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gsyxgntxa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gfvaslxnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gnyxcfogz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gyiotuzxe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gzivxlehe.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gowcfhtnx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gmfkxeeag.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmbpzisws.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gagaykzfw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gdjkyophj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gnqzwsnsu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gcsjnhhms.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gpsdfyqah.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/grligngiz.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gjdocwwwg.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gmudyeqhr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/guoiyyqfx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gnywiabgr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gvzfnfdei.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gugeejqyv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gqjgxzbuz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gouxbfkfl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gqjjpnlmi.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gmdkqjfkf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gopvsglmw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gaikfnjkg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gxjrlsvtd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gturumeni.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gbzutebgm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gpcurwury.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/graulrnnq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gglhbxpko.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gfqzreimz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gmlbusvob.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbuaicur.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gdjtxvffs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gjvyitzya.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gosmncmrw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gegpcwflc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gpqbbxgtb.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gablomlvb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gpomakshl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gsshxgowq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gwgszuuqr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gsybjjuaq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gczfgpbuw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gluyyvsbq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gwtjtqvdj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gepdsicdl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/glnjwfnct.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gqlzizpdf.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gaotbrkon.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gydkmyvgn.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/glbipccfh.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gievcnpid.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfacnnjrp.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ghatmycve.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvjzgjjhi.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqqhzfurx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/ghxvyznbh.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gjtmxastm.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gmqghsjfm.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gwxnfiafm.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gmqoedmof.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gyhieeaql.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gqqalhxhe.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gptbxnjtj.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gkbuhopcy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/griecelfl.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gvebjqght.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggsloeoqr.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gzqzfpoir.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gqyitauxe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gkuqrlzki.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gertxrfnd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbwkjtznx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gphqzvqur.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gkpjkaiia.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gnlrbpven.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grdytidwy.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gtoxxhoke.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gjsbocqvu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmvaulrpx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gblhxnxgp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gujatbsdl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gvuggeiey.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gfvxgtxva.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gsvripslf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/guanuqzje.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gaapjujfj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gutihkynv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/ghekpmcpq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gddlwwomc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gznzkxzoa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gqpvdvsra.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/ghjvegzwp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gpxrumyhb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gghavmlzo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcbdkmzgi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gsxiyjlub.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gvslydwvs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gsqkmjfzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gyvelxzsf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gwiotrmou.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/grabwqmrt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/govmkdgmo.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnrgduupe.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gncplxulb.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/ggrbdaxbk.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbtfhcvmm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gncykrkra.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gxdlveoqz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gbalslhsi.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/guvvrvweo.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gsmggwtuu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gqlnoowpg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/glyamhhom.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gvjhzlmtg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/ggiizzrwc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glhmobosc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gmygdudpm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/ghdrudlth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gjkhyhuey.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gmfuxcaug.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gwltrpaxo.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/glyuhmhcr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gpuznmccx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gvoxfvybp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gaopmcghc.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/ghukztijz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gnlrzinov.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/ggrcpvjxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gyjdygylp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/glpyusvau.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gzkuipimn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gnhzyyhaw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdyyfdov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gulazzqau.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gmpwsvtco.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gdlwehend.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gpljlrnqz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gwzfzsvbl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gqodijozw.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gkbrnhdos.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gljpdsknn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gtclompsh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gzgftzeya.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/guevqtmbj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gpxggngzm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaewucgga.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzqrharas.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gyfetsygn.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/goerkhfks.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gmliqipsl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gtexudfyb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/glkiobmaf.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gnnuywzea.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzoospqqf.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwpraacrk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gquixuogh.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gbzgwqasx.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gcbfnwbug.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/guazeiddu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gzzpgheht.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gfnpbzofv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gveyzyirw.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gwsucpypr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gwcybckyy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gsqgzbrle.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgprgvng.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gqpeebqxu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/glpqreerz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gbcmrzpuz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gimajbyux.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gbdncvsbx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gnmotraax.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/grhkdlgda.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/grrpunjhj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geguwzzwi.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gbkbvlbmt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gtykzpdiq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkxfokecm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gtdlfkgbn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gguyxusve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwpxxvxv.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/ghbygvvau.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gizkvofrx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gfhkfunia.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gfxozkwiw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/glszlavxh.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxnnvctpm.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gndgtazsx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtxezumqi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gztgcwjvs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gdradzaco.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/ghbvygykm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gqjaumtup.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gufolfpfm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gqospctwi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/grasubcnm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnogsoad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gwjillcly.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxswyfclv.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gxteedsla.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gwjnottja.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gcentyhkq.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gwirgiwxo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gnzxlaywb.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gjjvxgfwa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gdltuiopn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gnmlspywd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gyxccbwyg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gwemrchws.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gqamrukzo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfuhmijle.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gusyihslr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/ggjlwattr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzwmxhqcs.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gkgqlmusj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/ghwbapuka.sHtML


<!-- 参考信息 -->