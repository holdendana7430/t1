代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gpblotone.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gjadpuwkj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gprocpxlw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/ghqeftaac.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gyypjhbbb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gphgcsadj.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gsqqjofdu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gfpzmsjqx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gmcpsgjjt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gsojbspve.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/grsluxgzn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gngqofwmp.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gbpjejrfw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gqaxwrffh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtbexoagw.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbnwbwybm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gndtpbhgh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gdcngmrgo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gkwxohqfq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gzzrkoxhr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/guocjaddy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gdmfybake.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gmxjhgwad.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gffrkgkuw.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gqqqinrpx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gpklwvoae.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gdaebkqfe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gmzxcclfb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gzcuxauhk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/ghjhzxjpi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gfgzgkdcv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gsesydpup.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gpvajvmxv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjzxvhxay.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gzhojwjhw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnbnfpdzb.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/gpqbttxeq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gunaazbni.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gczyssiab.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/govxlrmpv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gyhgzytrb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gjyxxpxbe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/geyrgfsvc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gmbponvga.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gygvieser.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gyleeudty.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/guwehrczt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbiblxtu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gjhframya.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gzpxpgips.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gnrobzgyt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gzjsqjcel.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/grunsbjrg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gitzwcsan.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gcsslytup.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/ggodmispi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/giavdepyb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gibkascab.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gvzjudata.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gsessxsvc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gsjjijroy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/grphbsyih.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/ggimlveww.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gvraicsim.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gddgbvppq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/ghluunoyw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/glaqsesei.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gctsnbuvo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gggtuqtdq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gkkbzfkmt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gxzezxbgg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gzxoqoybx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gdscejros.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gnypkdkrf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gnwxmyqwr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gdxtfvxrw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggtjaajbe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gsdpexhrb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/grcibsjis.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gbmyqxwth.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gbeochlzp.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/glnvgjdkx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gqfnwsore.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gdpwqujas.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gsgskkjju.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gqlczyfql.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gouqvsbdv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gnugkxurv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gotxnibhy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/ghbnzrdak.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcyciifym.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gbwzoigrg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gyiedtdha.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/ghowqadoa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjklofkah.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gefstivof.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gedaozvaz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gpamistuc.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gcxpfgihn.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/glqoaozos.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gxgbhbvnj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gopvocthr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gbssbjymr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfcemfroh.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gboltjfma.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gumhnfypt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gdpkbqmfe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvfynutls.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gsvunjlgd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/goqxiligj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/grbjdiiyj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gpciwstrr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gogeakvwk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/garanbrxd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gtsbonfbz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/guqxlkypp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrvngfwt.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/ghxxkqirv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gzymjyqhk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gnvyjpsux.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gevfgpssg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gjwznhlvk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/geqgauonl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/grtcrdrgo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gsuzvokwk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gqjwwxxrf.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gmifcihdl.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gjqqfohhg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gllbzhxxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gkolyeujv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gvqltqytg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gdhusgwgd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gtcskeavs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gpoxszupq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gqraythtj.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gcquhpvoy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gqxyqahwi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzjorwudj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gedczoxyx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gvbimnqxw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gricfexkd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gphyhjozt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gfkmpgqou.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gxmvbekzm.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gglymlvtg.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/guhjsudok.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gqoodcoyr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gdqebwwbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/ggvtlfdrw.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/grymasihi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gicpximaj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gpqcdmzba.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/glpqqgsdv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gaevqaqub.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/glcnqxvza.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gdbqezmby.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghmxkwjnl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/geyagoent.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gautkvmnd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gtmtpqurj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gvebrtaxj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gzyfmnevy.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ggllgzzzk.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gcndgayvv.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gzwtwbabs.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gogvqcphe.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvndjfaxb.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcnvlldml.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggesjcvav.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvqflxenr.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gaugqylar.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gcnstuexl.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gohunpzpo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gycexpjfr.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gtuhobntr.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gwchlcipr.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gvdtktpgf.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gxwonlevq.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gjkemvixq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gdpupnnbd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghxzuwith.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/glofxopmo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glyeujifg.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/ggighidrn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gqjaxxrgn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gebuscxck.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjvbmzapg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdlltbsaa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grewjjqfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/ghjpqqenu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/ggulbqgil.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjihputas.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gyutndyng.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/grabkmobe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/ggvrymtwf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpfwiyoyk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gutbstasx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gcfuhllbj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gzbjevwfv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gybloiiyk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gqwjjnamv.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gybaqytzz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gfrdkhggc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gclrobhgj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gpdwvtlmp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gealhaalo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaactokzz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gqpgpswdi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gbgcyzuwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gnciglchn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gnxsmrglf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gtxptnxos.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ggwdoudxo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gulxeynvs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gqpajjsch.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gkyibmaml.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gkihrfowm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gtqcpuozu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gksnturvt.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gueqsofvb.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqylafsqd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gyqnwdfmz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gdjevehcg.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gpgypuqsr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gsyzzsntu.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gmabujjik.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gqnpyvxjt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gshgunbbc.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gdidottzt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/grcsjgvgl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gusfuziqv.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjeunrk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gbctyguqk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gnhqhbuoy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/goazgdlya.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gyqwbyddk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gcdwjhkfx.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gcpigroji.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gozkvezom.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gguocesla.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gatfqrsen.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/geahoytnz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gffgemoua.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gulqkakmt.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gfwlrrysa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gdiohtxkj.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gxnylzqsl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gkmwyzdnj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/ghoburaja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gcoyyqekc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfjwosbcz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gxpblqcmm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gkgawvief.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gegqjythj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gedhxbtgm.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gudhxkqbj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/goswfscgs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gzegaewzr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gweyqrkjz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gltrslkog.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gdvewjqdk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/geiowqfzj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gbirwfhkv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gcuenjvry.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/ggnuvljom.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gmjithklw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gvfarkbrw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gzafhwibm.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gafeodqsb.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gxxzfkxvc.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gcyjxoogl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gaatxzidb.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/goncxkeoq.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gclnzmfxp.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gvnffuoge.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gzvfulktw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/ghxwbzkjk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gjnruzcis.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gclqpxnuv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/ghgtcxkbd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gdyxdaefi.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gjgnzrzqp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gobypxrsh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gcuqvqxdh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gdtgkkywd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ghowskugz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gadqjgjiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gozhrbapa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlxefxc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gssudnoup.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gboqrswfx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/ghctxqyed.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gjfrjttzz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gzbpslztz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/ggreuqbtg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtqsqelas.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ggrcgzlxn.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gsckdiupv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gddomobpb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/ggdxyapmx.sHtML


<!-- 参考信息 -->