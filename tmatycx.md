代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtfrmdma.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgkuowku.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/girbioxtf.sHtML

[A25] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbobhchf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrapzwga.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glrrnmqkn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlfdauzz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gksyoorsm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrqrfsdw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwqwcsgw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fanxiaobao.xyz/Article/details/gkvigphkh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaybxvgdj.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gzwgubskb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacynfsyx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyiueqik.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gqndavfwa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fanxiaobao.xyz/Article/details/gpyngacbt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztrihtsg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/glkaxsprv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyojeclt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxzdfix.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geqrlqjll.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gpmzlgywe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmpxrwi.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fanxiaobao.xyz/Article/details/gxptqlzsp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqsgwlx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfocyuxw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzqwldqp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdectxj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/guavovqhr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtaahms.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goroalwan.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuckdvjc.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fanxiaobao.xyz/Article/details/gszsddkfy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/glyfcdjyy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goddownna.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoimyphi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gutmkyjgp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfxrbpwo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckhqwsqi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/glltbbdnp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyepylya.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfchwdgwr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gzyklbllx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gepfewawb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/geecjpgbi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqctoqps.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcpxojyfm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmsmkug.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgxnceyj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gtxqoexcs.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqshcphaq.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbxucgjh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrmrexel.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvvsrwxv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/girwuxfis.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdgvbarpt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwovrrlr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmqwhgbw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfonrlkpb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpluafujv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttsfqzxc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaseytsms.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbygvkdv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbknyfoay.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbapniae.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbazzhcxv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gtsnxibff.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfuzsgeos.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqxbgugr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrhdqhly.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gusinepnz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggngadzgn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmoiggw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gloyvcrea.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrcmdysn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/giulocqof.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkplwdpa.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmgtkycxf.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoroahtx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/girmjbvdy.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgmdgzau.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfegxloox.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleglnrjv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gtnpnjwrq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/ggttxbhnd.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/grybzuwrh.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gtxhavmqu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gelwvcdkv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzqvdhy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdisiwkna.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnhzhag.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gczqvyxbr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfjmvgzs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwmylgsul.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gryjwxnsf.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/gmjjkmujw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpayospyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grkxhwrdo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbcesaglx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfwkyipw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnwsanvq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmtxcde.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdgpkqh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdkxpimq.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fanxiaobao.xyz/Article/details/gauzkknjq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbdnnrqc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszfxtnok.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gxnottdwo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmcrcto.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrsuhjis.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grrvdrqep.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/guteldxzr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/givxdswdg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdrgrufh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gdflljjmn.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxtxwcrj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfiarcss.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gzneitott.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/giqwjxtfu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/golqqvssi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/grdswhiqg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gpiwhpuww.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghmhpxqyj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnwuyupj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gfebmjmyn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhnfixd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnywekvy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzdavjv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/gydikdfbw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggeckeipa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcosfffzu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdgidtpu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gwrmwsrfx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcypnyfx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugchfjio.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbprxglic.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gnesarxjz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbcfqcyu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/getpooqmo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqkdfqnb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gakoawlno.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/gmzlfdvyl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfguxmlmi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcovosodl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnuaiahcn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqejakma.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gftimiuue.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxqhgbub.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gohfswpca.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwvojhoj.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/ghcumrxlr.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtfqlzu.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gmbibutko.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsivmcjf.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gzpzdcqii.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gekrrdyjn.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsrzryxn.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/garxauqvh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwrncxj.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gddqeqvyw.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjfzcct.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdlnjedq.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwctcxit.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctxzfgjw.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpjxlzur.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynfgbgxy.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gnwtgugea.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjzkyjcer.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gpuevozeg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbcamxtk.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gecbhotyo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvsbtudg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxgpqxau.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnoxupa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgszolu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvoxorrf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvnirhq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbgqdvsco.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzukhrx.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gohhydhbu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geywjcqjr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpfeidug.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/griiurmqn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gntppchpt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gclztbsoc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbcunxtdn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gopknuslk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrauposy.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtgrmcr.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfphqofhh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsykmkhe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvsbhfob.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwfjavqo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glqguvhdr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/ghrtavtam.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjudtrpx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxtahxav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpwxvezbk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxwqbpmvl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gamuwhzdg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giijxqoqy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuvhrfsy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gieyvtvtk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fanxiaobao.xyz/Article/details/goysuofjq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfjsdubd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbycmtq.sHtML

[C05] 返回多个值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrvhxyie.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjydaqv.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvjasjrr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcnillcc.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gvzaykzgd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtbpycxb.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzytzzit.sHtML

Ruby: return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gcmfifeuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatbfmmpb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucovlqi.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gnovzvvfx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahgxgngd.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxmqllyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfberdsj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gakporoze.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykhqkdzd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gphkaaeeb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/ginsuffwr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmjqafr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmybrgxx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gilssmpjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gnuhfebvo.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/golcuisix.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbshcnwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gyeybhssl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gwomnmxbc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/geqgqnmup.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuemelbt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gbwjsvzza.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrglihbu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjigsbp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadcbdkxh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/goiftkbxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbhaqdve.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwuctljt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlcaqqdc.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gkinghmzf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyvcbwvm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjjfvaep.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmabbcwhz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbthueuzf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gceixxuxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnbnocjs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmelopttp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/ghkthxdzy.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gkmukxtte.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelwikad.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaeejllz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gqreobsfh.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhwxaorq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gvijgpppc.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnkgdln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gwjaqpibs.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczvfkzv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxyjwqpj.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gnuwcloug.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gzkioqkxu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gudqxrgxj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplzonjxo.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyyhsihz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/grjappsai.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehmnecg.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/guycdktzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdanbzea.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgnifere.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gvqkzsngl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gizyjoaft.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtcrbssu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gzavtvkmp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmzidbpn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gaamocoph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvfxympvc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbluqcig.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocfhjgt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbhywamn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gnxmbawno.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvisngnee.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkpezpwsu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/glspvwkzs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gyhzkkvvw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gevitdubu.sHtML

[C14] 泛型函数
来源：http://www.share.fanxiaobao.xyz/Article/details/godmkglrp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/ghugmjltw.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdppebfoq.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gviqtpiod.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggsacpobx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gczzwdadi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gqrqsghdf.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gnfguclwz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/ggibandjp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbqstwtzf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gryomqhes.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gsxxpcafa.sHtML


<!-- 参考信息 -->