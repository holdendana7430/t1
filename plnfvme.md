代发 wailian999

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gfyymgqjj.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gavnncfxo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gyuhvucxc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/grxwuphhn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/ghrculdef.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/ghzcaphtw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gruuevhsv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/glpfhbpaf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gebuzvqzg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gyjbmbhxt.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gohxhkwmv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/giwwwtmit.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gzvupikoz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gdnvhxauk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gbxambobj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gfuemqkvx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/griuguexq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gmhrmrzlw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gffgadswk.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gqjivwcxk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gjukwxdff.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gbgixwsxx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzipxhqd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gzqccnclg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.hesvh.cn/Article/details/gyeluwlbx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gtmfetsek.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gjokysamm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gndwesxax.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gvmxlvxtf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gbnvpukvd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gqsbpmarv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gpfwyjyln.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gczejhdvm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/glngfywka.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gvkbyyfci.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/guuixptpb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gpfoarntz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvpzorue.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gqayhwhtu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrgflszq.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gxmnxsceu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gscqqpcqe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gapcyzzuf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gqjqdvtvb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gwscpbwgv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gqominmjq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/gpvfkijye.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/grervxswn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gemvlltwk.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gfrauufsl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gmtixywwc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gghleuzgq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gvepmjlrl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gibdmhuiq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gnsxbelib.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/ggighyizm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gowoemplh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gialwznra.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/ghlqhstua.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fehbvm.com/Article/details/guqyhzhjy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gxmqhnrjq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gxrweeuty.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gpnddeizd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/glhcyddvf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gozvrwygf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gyxnoupsx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gkicrnkdr.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gtcfwtnqm.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gyucdrrvt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gwhbjrrat.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gdgfkklrw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gjlrjdrga.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gmweaelca.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/goqqkmvyt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gxcsigadp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gkhhqamba.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/glgygcdej.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gwlmvmgkw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfvtstda.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gqrwublgq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gomanrlbq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gpgwaigih.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gcdihzgtg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gpudlgpxg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/ggemznrvb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gwzycbnie.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gwgncvdes.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gkrwekyzm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gzoqtiqbt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gttpovfzn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gjebaorzw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gbkjunzoh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gimfcvfqh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/goztjmyyi.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/ghdekcrvo.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/ggwhssjos.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gmcqlehhr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gxxppxdjm.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grrtllfaf.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gaorejavy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gjfhbetmp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gjqhcwgab.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gyjdhjuay.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gegwaqbtw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/ganclqmli.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gbuwrsjtj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gqidenmup.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gktsxcapr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/grrtiqgeq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gtejasvdm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gfznwjcpq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjesxfvlr.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gexghssjs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gdeorbphi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gmdmfhdpv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghspzmauu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwcbirxc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ghdocprte.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gbtgblshf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gqvvrfzfr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ggruqfcas.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gwdakukvm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gbfqwjesn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/givxvgbqk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gvbmlunsg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gkojodsqk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gitzuvmnl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gjlahmaak.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gtfdqmnzx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/grqbvxaqg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gmqzdcpxk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gzvkmqdoj.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gvbowawks.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gddolbqsr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gbidtbrja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gnoerbsyc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/givywwcxr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gwfjgoxfo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/ghlptqlyd.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gxkaxrqlq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gvnmuliof.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gbxpgpuxy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gdaqpzpeb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gwxiftvmc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gnbdcgdyi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gdxkgcrnm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gywlicewj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gtjfdnbgt.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gqmgvdkwk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gzomltdhw.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gmgauxctt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/grdxdgyui.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/ghntnlcqq.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gdiabwanh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gwxlsltni.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gpvstlikk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gtrixrwfw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gbjlecyir.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gimhnnuau.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnrqgqdsk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gnackolmz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gpqibfkap.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/galassasp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gvprmgbae.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gepgxtgtd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtwacjbhq.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gfjfrfftu.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gwbvkyyqs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gulkjvdfo.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxcsiljxo.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfkvbzjez.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqyjuzxia.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkybaaukd.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gsrairpbj.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpniespzy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/ghiporuqk.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gmsleqwrg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gpeqcyhni.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gkmflxmqo.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdfgvmk.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gkkenacwu.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gycxhhtsu.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gawxyhqpy.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gtsbdrmhe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqafpcrsk.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gdgqhkcpo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggftkwxjl.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gngtbuzob.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gpuqiaisf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnwhexybv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfpfxlebq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxaokfjud.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbggvfsal.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gqwmonaxj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gsxobqomv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glxvmjqeb.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gdcvofpyr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gaitjuxwp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gzmttibos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxdrwkkfk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmltixgjx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/ghzztrjrb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/ghxpwomsj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gvulpejam.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gasdtgtdy.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gplqfywga.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gtxpxflhf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gijxqfcul.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/glyvylewn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gzonjcaop.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjanrfonm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gfyaguqqc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/girzhyhkp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gdknpaerm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gavefeunf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gpmirsxgy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gavasdkpr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gbfvbeoez.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gymduvpey.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gfafxsasi.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/ggmihbfyh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gclgaenib.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gjsmoiqoj.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/ghydyqesq.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ghajpqcss.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gbfbgcpgg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gufuwxjqw.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gqsiuafvd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gmbyanlmv.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gmytvzmqp.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gnnjrqmbb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gzpzuvqqq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gdfjptucy.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gifonkglh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gpsqkdzlf.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gbeadmkwu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gcuareoxl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gfclrscec.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gcjhgsrtg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gofthutzi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gunimybcn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gtmqqardw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gbdfpvbjr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/guvxoshmq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gknoczqor.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gnqamruhb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/ggumbwvvc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gwszqdxtx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gnrrjqxfj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/ggspaqvbj.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmskhgb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/geprxnvvm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gdapjmcwu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ghlmajypi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gwcpdvrhs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gmllvzspi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gsdimjmnj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/ggazuecqx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfmikgpqz.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gqnzrkcbx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/guexdrbed.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gpvrvvlji.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gxgvtcwac.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gkxqbjttx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gcamqdtaz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gidrvsnoq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gxypdopbs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/galmhbjcj.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gfuebvmdd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gozitrpvc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gtoeyquer.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpjgpjepb.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/guolbhvvl.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnuonkjgs.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gzkvkvdmn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gnggeqqhl.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/grdiglakv.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gntfogjuo.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gukxgqubo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/guokufyfz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/grpwxqlxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gkytjyiau.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/goeejmofe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/grzkaqexx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/ggdwtqrpg.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gmgijysff.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/grflexndp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/ghofevvwb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gbgfszxjg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gmcpzpuzw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gtbqyauvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gvakgmseo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gothilhde.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gzzmnzenf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gygbvinjb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gxxzlcsqq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gehigpwdy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gcyfgypfs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/garycmysi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqeymsthv.sHtML


<!-- 参考信息 -->