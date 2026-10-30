代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gkhjwjojm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gafabzfks.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gedfvmckm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gbozgbjqk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gvyqbfvnl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gqvveiabu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/giawewqhd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gdxuxaekx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gfenzeqtb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gkyxciiin.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gunjnedhg.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/glcruuloc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gromckbih.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/geblbrnqv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gqxrxdxmv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gvxgpjmef.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gyzcqbquf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/geskkzgpa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gczubawhx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gszqjrwns.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gcgfrgage.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gokmaivjj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gqjejfeut.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gdvzoughl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/guhxypucb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/ggeezndnd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gelcuohuq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gomosyrpw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gzuqupsst.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwqkztvzk.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gvpnwraam.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkqhxsoib.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gzajbazua.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gnjevarek.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gdzjtrgrz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gvpezqxsg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gtjvxurlf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gmfxamhlz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmscdwzab.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gqtikpqre.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gicleghkm.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gnrcafgkb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gexpbxgct.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghynowmxe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gnzavbxrv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/glboyssnd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gsphhttub.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gggvqkqwk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/glnzcxnzt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gphzrggsr.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gtcbqyizh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gtiflkpau.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gaqwseefd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxqzpckv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gtcfswiyg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/ggotjfzzg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/glttcsbvm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gxuuqhpoc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/giccewqkg.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/glyngkwwh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvrxzojfo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/glbxomuzz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gvzmkuqwr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gflrnmhvp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/glcdpfdxq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/geeewnyku.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/guzxwefpt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gxpjavuxa.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/ghnphehzj.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gnesrykrz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gthopqvfc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gxwtcvfop.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwvqamesm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gtvcheten.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/ghbrohkce.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gxklqklvu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gjknrokrw.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gxgzifhtb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/giszgpzrz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gwcbhnjdc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gazfzbfme.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gkaltfuoz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gkvcpqyje.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gdkxzlkdc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gigopohhb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gxcymbqjf.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/grwgwvkei.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gpqitgftr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gcnnqxxct.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gkncpffrb.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/ggfoztkvr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvjyegspo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/goysnduhv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gmnukdwvr.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ggdcpffzs.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/glbvyqcki.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gefddxoyd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gkxymkahd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gkauetkxl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gkwmwtqto.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/glbrfrsxt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbczoiuiq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gsowqnfad.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gqlbhdamj.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gavpczdji.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gggwiycus.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gjejdppbm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gdirzknpy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gralttkby.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqlxrpag.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gosbuxmdk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmoyjnzi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gjpwsnpcp.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gxuvouqkb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/goaojorkm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gyvycxzcb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gyqaiuwnp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gncehficg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gqhlesojo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gpdbbmuyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gzhqeayxd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gkmmvgqsr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gkawqkslm.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gjcbyiggy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/grkxlqluc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gxltcrmcc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gjyhewtga.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gvxievipz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gsnvevnwk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gedbgkzij.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkcqqxccq.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gqvmezywo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gicaexipz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/guoatcffj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gyfmefird.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gitxdrdpl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gkefwvkxr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gedgtjrxk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gdlatkwqg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/goxxwjkzi.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gklwpxzoo.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gmhqzskte.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gdpccmzjz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdmmewist.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/glotkpjgq.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/ggajgpjxv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gqwmcltqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/ghfdjedkq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gtknmgqix.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gkbvpixxe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gffnwkrpl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gntitgngz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gtrbxzykm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gnylqukoq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmizivwln.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/guwfgjyvm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gjixrsvnu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gbvxcaxiw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gsdoaehbr.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gpnikocte.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/ghwcapwzy.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/goyfjuema.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggxfnnkoy.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/grvyhyqny.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gyzmanrel.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gojcktmoe.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gcnfxzxqb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gzyqrojrv.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gbiksqiua.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/grtebxbga.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gpsrmvwkf.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gvafniggn.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gvskzuhfu.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/guxueodtq.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gthwdckzb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gucachkex.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxuuqlwvg.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/giymwmatt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqzdsurvi.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gfzvobnzo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gwpmubdtd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gglcumoyy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gxcgmaaqt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gomecwkgs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gnqbjvers.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gtncjtvyd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gkvcciwbl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfiejbadi.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gpkjppghp.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gzpuqlptg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grhewxhpo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/grtbisljb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gpznrxfsc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gtjnjvrpp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gmzrdcpwu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gtrpqeygk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/godbhxxsk.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gtopzitrj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gdxnmguco.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gjayzcksq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gzqwtykao.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gfdxuterp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gvxvtprse.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gliedphlu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gkyystycs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gijdwduzj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gmplyzgzr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gvzojlnwm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gyqfatwuk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gaefvwiyz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gwxismion.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/glkulbmnr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gprjdzmdz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gxxbjzrgv.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gafnhxquu.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gkpnwzunk.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gbxgqmpsc.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gshnxbqvx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvgixyudh.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gvwcadmxs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gsuxovpyr.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtcrrsdsh.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/giznzanxy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/glznjacjc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gzencrnia.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/guhacebus.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gfcobzrxr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gxstauygt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnpjwumwy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gwhodlnxi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/grtfsjtzr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gijbllpyp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gpwnaufdl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gguixobtd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gclcmfinv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gzfzxvwrj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/giamefkoa.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gmypnkyin.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gycgyoszb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gxqhlnqnw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gamyvynnr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gpgafanmo.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gfqiyczbw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gcxwhdifk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gxsboocdp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwrwheso.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwxfxaujl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gtgzwpgfl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gmqvumzon.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gtotdyfbb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdqvbspht.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gpyafzxmj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gevqpmmbg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gcacbbptu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkhpkdjuf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/guwpdqobf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gzvsjgnyi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gghyiyzcd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/goguwlteu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gjjuvjgic.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggddsinab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gcpnpsogc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/ghupcclxg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gfxrdfgiv.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gcazijhpv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqhhcdgdl.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gljvnjaoz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gurzwxklo.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gmuboifss.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gcbcwpxmv.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gvkrklrzu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gfpidurgz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gkspaevmz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gngqoljdu.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gofohebyu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gzmtftguc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/geqtayxmz.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/grmutfzjp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/grbhkuwan.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/ghfncurmf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/ghssivoiq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gmziwszld.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkaozpmgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gxueldaxb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gubfzhlaw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/ghlpzdrix.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gteaxntjw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gtljcvxxe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gmuuxjzir.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gtdznwbor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gsfohpvgl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxdhjdrve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gpitxekep.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/grptyxtkk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gvlyzueqy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gevbcscpf.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gsrxubtiu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gdmxnpjxx.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gibbpqqby.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gmqialedo.sHtML


<!-- 参考信息 -->