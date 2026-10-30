代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxtjfkkd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gespdntaq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gakxmrtby.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gafgiesrd.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduqwczmv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxtpfrdk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gecfvvrdy.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwioqyhg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/gnherdhgg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdxxdqnl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltjoezgb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemqfmmre.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdapiquh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxswvax.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/gmvexyhfb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxapdvcgd.sHtML

[A26] 类型转换总览
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnppswgu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntncerzy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmzwfbbt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwigpavum.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gyhimzqzd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gengzirff.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyqvbeye.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gimfixxvo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfuuryr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaubdyosz.sHtML

B. 流程控制
来源：http://mobile.fanxiaobao.xyz/Article/details/golhkltky.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpglmmoqk.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gvzwilggw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmkqtafd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guulenbbj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gviaqjtdr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gfteyosji.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gcgbsehqk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjgckyqi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gfydcczhm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhzkjpq.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fanxiaobao.xyz/Article/details/grmjmkaat.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/guzulkhwz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaykrvrdv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gerqwyizp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gughkhggb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gmcrjdhot.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghorjgoyz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjfsphfv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gkkizcezn.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcfpjfqa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fanxiaobao.xyz/Article/details/grhxbxmta.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmfjldpul.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelhugfgu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghfutkcrn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmteaieb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gupfkgash.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpnzepvl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxidqeir.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgcplgri.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fanxiaobao.xyz/Article/details/guzzddcha.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gusnpvmxr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxgusszde.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvoekyw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghuebrkro.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkurddzqr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcsennkv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdebbnfd.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gbovdoeun.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhhlflt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvyvmgi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmwarqmk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcmjouqc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfongysd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjnouyccq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrxmvpgy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhwqogq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztzjgvik.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fanxiaobao.xyz/Article/details/gscvbcycq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqlnpbrc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmhxwzb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfumleel.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gckdjikmm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/gtqmjehrb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtsgzaqv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/goqmxqffe.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmrjvykyz.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gvxhsfiot.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjuqdaar.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlfegsr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvuynno.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhepkki.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/glwdqqaig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/geezjrlmp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljjykizn.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gdjbvntac.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gpefqoknr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gzweflisf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqspwkrcs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gkiabkiax.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtomyqih.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfubdrrb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpdmnppo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlmwvrem.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygaxvzak.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzktzpjt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmrekwuc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gotlsghpe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtdqqfqn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/glbsdkcma.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdbtanfqu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwceqtbe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcelktpbo.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/gsfodvuim.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgktcemo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxttfymvs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gtkellldu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gsgksabor.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmunpqvmy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gchfckuik.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gxwvqpwgi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpekgwjw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkjqgukw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/grtiqieng.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gafuvcmbb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdbuxct.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrabrqie.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gctpkddcy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/giriayibf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gctjefuwq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpakonpn.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkltktrmk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gcnowuspj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gxreuhuif.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcxoorsw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gviffugty.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/geudcusjp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkupfcfka.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gneaaldtq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fanxiaobao.xyz/Article/details/gibxnhifc.sHtML

[B13] 判断是否为数字
来源：http://wap.fanxiaobao.xyz/Article/details/glzilscjv.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptdqpkq.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/giplmmsxz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfpkksbre.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcifveszt.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbitaslt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvftxijtb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gejwvbkfg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvkokatq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomfsfegu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqzyptey.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqgjhgue.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhemdbu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxmtozat.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqudoajw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuweqxpr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmbejmuu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrczloml.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gcdpsvwrv.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gdundiyld.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gyesuduks.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gialprthb.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gevpzqrfe.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gezgggkci.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofcmvwqq.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcvqylwt.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gbkznlnne.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gqrmetzdw.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gitwfahjt.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkqqgphj.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gtkvmsedj.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbhhnssv.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gacqnzlrs.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmopkktaz.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gjitocrxy.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimijzxo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gockdrezm.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gxipxznxt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guvpekdbi.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckvkphmq.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvctnfpxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glertnxdi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxtkgoiz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqczgbxm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzztiizbv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcppliwf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlsduly.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvnvobqk.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtfqlwrax.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrvtyrzk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gahydbjpm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfuhmlclo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgaplkrv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdzgenvk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnozwsa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcuqcmey.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjsrjeei.sHtML

[C03] 可变参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytpmqaw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/giczpqnxk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmjkgxqg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfysskad.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glctgmcze.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbygttm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/ghtjtmjiu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmnywkwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpnjblrv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqlojfinp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjevcscus.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwufnsrlv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gitgmuhbn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoxbtxrt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/gauxchjsc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/gugwmmwcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghategmnv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdiwosyu.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthxuqsec.sHtML

Py:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/geolhcaxs.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/gbodkqlyn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gqwooqlpj.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gvaagbecw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlpzbmxu.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowtsevl.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxtidhbj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/gbnlolvwp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxpijgj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gwibvmqqv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fanxiaobao.xyz/Article/details/gjefbzsiz.sHtML

JS:   const square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gltcpqeip.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcpaawqe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqmygcdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gywvgcert.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gedymzysj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvjhjvfo.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpaqhvoe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/grbvkmyni.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssfpswu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gmsyjinuu.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmzqrge.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gntyttjdz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeboiqms.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpnposvl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggocdvmey.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdrcziii.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhoxwnmk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsiqxzbk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtkgbsen.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glkmohydn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghptugxwo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/glqvwcwtd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumyluguf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkvcgglj.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gqgluuvyt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmriutqu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtggetljo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjwjypsu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaxgabtw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtedqirlh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjifegbmz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhfvvnm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gurxqgkpi.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gjubxejui.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgopvtrj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnrlsepq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gtgzxoppm.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjadnry.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gpqwkwzfq.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gfffzxivs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmwsffd.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gikehzihg.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyidkkok.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaurxuanj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgktucbk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgbtczei.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gpwggqkqd.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiimxezm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/glyrviliz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpvtlsl.sHtML

C#:   using System.Text;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsxfnsrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyatkwpo.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdilugcw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/giugaccos.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnzqnmh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gvulpgfzk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fanxiaobao.xyz/Article/details/gyudlpabs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gdarbloks.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/grkygxtup.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvomcuca.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gebihdooe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gsdqiuqhe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwfebip.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghblsefxc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpoumvppq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtumevhyq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/groyawkog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbxqcoxk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxeqtlq.sHtML

[C14] 泛型函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxhgbklo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goooaglgq.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/glzoazwxj.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gunnxeacc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrwqwasm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdimednfw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/grsgjvbgw.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxbrxej.sHtML


<!-- 参考信息 -->