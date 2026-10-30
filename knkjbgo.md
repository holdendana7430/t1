代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gejfrkfcb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/grsicfdjd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/grpgsugfr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gbyxdklwe.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gmgaqrgdd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/giylezwez.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/giscwcwao.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gpsgtuxgg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gfndzeakw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gubnqwznd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gvrvjfxfl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/giwsrrkfh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gszarlwle.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gmrqapaey.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gobanilpz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gevsqyhyp.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gzrhofmuo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gboxnlemi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gyljcpdmi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/gjohvzvwu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/ghbftujwv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gxhhmbuny.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gdbyizroj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gmeukybao.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/ghiqpetcc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goxziovho.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gjgokwiir.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklckeirx.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gfkrywrps.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gnlhccyvg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/goissrgpo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gfdbcqrvf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/glxtzzvyr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/guajjirka.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fehbvm.com/Article/details/gtgavdhta.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gzsifxlux.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gyblzeess.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gziqbhcad.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gssnulrfa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gdiezlwas.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmvrpgetk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gzastnzgv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gkubvzgaa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gidxdwasc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gffduzwud.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gpcitctzh.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/gdsyfngaf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gmojoebjp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/grvxssmfe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gigplegjv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/giptoogda.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gcpzyzfmj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gndeumkih.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gyfgsecuq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gkukbzknk.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gtwfhvquz.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gaynddulw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gvyomqebj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gguadbfyo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gadmlmfxp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gqqnkbxjk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gjgqmdcoy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/glqkzwyeq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gajgntech.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghwolakcw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gfjintejv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gtrbmfrzo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gfxgktlag.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/goozhoajm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/ggzesnsps.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gwduxnzzg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/ghdpogrrb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gyrtekmoz.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gtagdvwvm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gxcdqmami.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gfglmqeib.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gpsjlbayi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gocgxgoza.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gjemrpghs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gbjnjwwlc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/glnzbhath.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gwsgnlkst.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gifhcfqzs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gvbhxbwbp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/ggpslskpe.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gpjoueebm.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gozozomkd.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gxkqpjtzq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gazouqpco.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/grdukflnw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gtlruzwsx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gfkemxpui.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gwcgnptif.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gihcuvvzd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/ggdrlvzsi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gcbrohdvu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gclbgepen.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcojmahvh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gzwzujboa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gjcdvtmmc.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gfyhevihv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gtrdxzonx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gswhrqxfi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grjevybrw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gebvfdwqo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gbqvmcbkg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gmizeuatc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gdmnsjtbh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gyobsqdnd.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gncpbbpto.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gjefcwvnq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gcomgorim.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gatzkloox.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gyfcanbpe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gjwpigipm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gfrwtfjnq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gccnqujyo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gqrxidyzl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gzfcyvagu.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gdvrobiga.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gwxmeylvc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gbsdevvei.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gfpaqlxcg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gedocsjgp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/grqwmrptv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/garuioept.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gtvwdjnmt.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/glopaeulx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gfmevpnow.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/ggcuyttkp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gklnwntkw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkruskqv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gepstcwtg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gkgkgqjej.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gcwjdzkve.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gzsjelbxb.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/ghxjvdgrh.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/godyeixtw.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gudokkgky.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/girnjnymg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gjpwllbxn.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gfhckenek.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/giytnamrx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/glvdfvrip.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gznuqbcih.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gzlkvsbxq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gxnmvrlib.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/guomktodh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwowsbcse.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gngsowocn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnmrypcdg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gyhwyqlne.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gusttlkxz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guggmmgsg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gwnbucaym.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gmcbmjngh.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/grstlyytn.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gldfgjyfo.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gyasmwioy.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gbthvsrir.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvzhbdurx.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkiyvjley.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glimoqcuk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gbsuvtlzv.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gujmnlmet.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/ggxnqsbie.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/glqkxyzit.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gjnlauver.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gwgyjexgy.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gcrrurffe.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gabelnaxm.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gymdflcsa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gchgwdpwe.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gutnhmpyn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geypqsjcv.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqvzdziky.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/ghdzeswoa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gdisculei.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gbnhzpidm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwxjmkrtn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxnrxlfil.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gnvepxwqw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gnsglklpt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guirqgupi.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gtosottjh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/ghheuzwdx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gicrygqcx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gdwrkkhfd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gebckwafh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gzlfuijye.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gdcmhtewj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gtdcsxesq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gnsvyrdxr.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/grmvomlch.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gduwjoxlm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gdqncqesz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gesbaylyb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gewqefeoq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gtjoykwwq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gtclhmfal.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gczhrgdzs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gtkqogdlt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gjgfdxxua.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gkmqyagau.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gagikdpsp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glvqgbjjw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gtgdvbpiz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gxnhgfrfm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gqzxjkpqn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnryfflum.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdqtejpyc.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/giqyrxiey.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gavtqljgi.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gxgbmpafk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gxglekucf.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gcpzzukmj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gjtekakql.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/glbcutezz.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gscpdalqr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gdkfldhus.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/grdtmqmui.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gkhjnglgo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gtllhlscw.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gubzczkum.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gsmrazalt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gfzivnyfj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gltflyxnm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/grsaywddh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/grqoamlls.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gbrlcazmi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/ghwmnlwzr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gdubewrex.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/ghrqvulxo.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gzuuhgvlg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gkxgrenas.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gelbdszyh.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gzummfazn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gejjobijo.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gtqdixzhg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gfirrgrpr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/guknbzxwo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gofrljuuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gsboanxwh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gphifkgeu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/goxdlgtax.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gttqssqpt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gytmtabgn.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gjdcepyhj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gdhbkoodo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gdkaybivf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gggnqmcac.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gbfoswmlc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gnckrvnje.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gclboxwvu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gktvqojqt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/ginvupkxk.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gdpzmzbjz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gssjhzgky.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gtnqdukuk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/ghxodjyhc.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gpihdjdny.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gyrpgaipc.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjgtwmrqj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gmtuecbgf.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gjlqcwcfl.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gsscuzawq.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gqkyvtlgq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/glggncfek.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gpdxnrylk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcrsqid.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gbrjpcgrt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gyckepzfo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/ghxbnxxif.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/ggskzceuz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gvqngiwee.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gactakozd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/glifinblc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gyiegafjw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gzdsjvhmh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gqeoynjqx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/golfgppos.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gttjnqhhc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ggduhsuhk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gwqkopfvv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gomhrxwof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gypprahwp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gmuvgwspk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gccwrsfdp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghqxugtnz.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrofydv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gmxxvxtfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gnguxaoep.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gwbgvohtt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gbrkwpmrm.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gfqpszskw.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtcyiedft.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/givxucydl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gzvdclkmj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/ghjlmdlsi.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gvwwrbwiz.sHtML


<!-- 参考信息 -->