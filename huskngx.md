代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gyznwtpsq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeimsmej.sHtML

[A24] 去除首尾空白
来源：http://3g.fanxiaobao.xyz/Article/details/gajdvfuxu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fanxiaobao.xyz/Article/details/gifdlbhid.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnjvhcus.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gmgbkrili.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpnipsq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbrekwko.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtizjdgs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gdevrwlhd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gjklmytqc.sHtML

[A25] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhktdxb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwelkfoqk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggcegvimy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gaoeplvua.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhsxckso.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizekbbhy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpfswjwk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goikimehe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiuflgch.sHtML

[A26] 类型转换总览
来源：http://m.share.fanxiaobao.xyz/Article/details/gdriawlau.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gronoyafg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmekocmg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/glbbmtgln.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/gcquuqaja.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxtrybgo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyhfqrrji.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpqamtro.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/ggxaujgsu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdlyhndcj.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gpefnbdjn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdugbpzr.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gudwhjawz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fanxiaobao.xyz/Article/details/gnexfmrbj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslggomru.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/glnawjvpb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtvtzuk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdjdnxa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwetviird.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqifyhjj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazyrdmqe.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaowpzro.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/goicxfkny.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtpezsuk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhmmdngc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkumwqaud.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/goaexbbkk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjiizgwi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfmyjley.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflqgbro.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/grjrynixw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gxujhrgpj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ganignkxq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grinfrgum.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnrfsuiu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/goyrjtorp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcryscel.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvveibpou.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gyrjhwrml.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftitbipo.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/glztwehoi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbteuvbrl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozozsmqw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvsjyhic.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvszdmo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhkzcvsj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhvocrb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsrjlzsv.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxdndxrcu.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gjgydralw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqelixn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzexasqxk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gruiycegs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvpruuqg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhumunmb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukcsukyo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gihyaqsno.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzbftds.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvcwkhgg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnzcoyby.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcxvwkv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giimrfibd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/glytiynuf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjeeswtl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzxwmybh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvjvkax.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggjsnlqup.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbzvuyyh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gndakfqlr.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuabvovf.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvovpaesw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grkisozlf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqrmdyrp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gslokdqln.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaeywhrnx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkyamalz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/glfraoctr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gucttuujt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvlyatgv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givloards.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkblfxver.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggvhahqvh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fanxiaobao.xyz/Article/details/gitmxefbv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdhybxn.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosmztrzm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvehdadjl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gklmcrjmz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqlpaemm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpayhmcp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gipzpnmxi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnxykktw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyamxjquk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnyhzfit.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/grrmcykea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfylvsvkp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gljgkleoy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gbanejkjf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/grzwqxihn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwebevds.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrbgzulg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsqmrnih.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbofttxie.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gvgsxzgzl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjwjytep.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gjxdxmoed.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqdvmku.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhsfqcv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkxygodum.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gblkhvxao.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/glcnhaqam.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gchliuzfz.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzigujfx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpvnceks.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuayunpt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxuclgow.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxqqhmbu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqfufwhj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghidnqmdp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/guehscciv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fanxiaobao.xyz/Article/details/gtqfypxrv.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmvpcxeq.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gbouptjzg.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqemmxqzw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvrpzpay.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhfjndbi.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgaecmcs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmckmihe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvppynafl.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gueqfmcss.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gojsfliyx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfelcnmf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdiyshrxp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphbhyyfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/greuqvyly.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqximhun.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwtjexk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/geeyiqecs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gfwbsknok.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqxiyet.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaujumav.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofftkaeq.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gaejcjzmk.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gffmtycwn.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwfnzmh.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gshyydlsg.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjcqktk.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gtfgvwxtw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gwnyyezmc.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gtttlwwzh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guokwstzj.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gufbygrei.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkzcevc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhsaolxi.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gufiohgti.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gvmnapbrv.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwsrrpf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhmsrakd.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxsheuk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsugdzym.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkmfikso.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gsvczwdai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzrazgug.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvsemfa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gephjhqop.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqzfegkek.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmifpam.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gymwlzwxf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gghwsilob.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gouiinnbw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gnpufeons.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqdfuiwyu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gecswamdb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghppwlzsg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaptsdzn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqmboop.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjgdexd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftuskgvo.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcikxohra.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvufjkd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeuqicbv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabbhzxbc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffckbuk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfnpbxa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgudaorj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gsamtrbap.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecxsoiwo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/geyhvjgut.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gdhumjoyu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gczxnlqfd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gynfnwkma.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gjyoirsbf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeaaesrq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqciwnpn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsbyphhmi.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfbgbwih.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhojuins.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqxprxif.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwluolfwz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gxseadupw.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxfrllmf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fanxiaobao.xyz/Article/details/gudccvkpb.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnincyb.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gbonduagu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/gtqlowvrn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxszatk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gjfmgfuby.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvptfskbi.sHtML

JS:   const square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gaomremhh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gatvutljw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvresatah.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gnxxsqcrk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbwguksc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/geiiseeos.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwniachh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaoofvtt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzipjubw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgiaxiyg.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqsytcya.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvpamth.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrkmrrxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyudspwe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gttjugohv.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwhmexz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gjhmabdik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfberdqry.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcdilgurg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqfuzfzm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthergnol.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubochxb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeusuzlc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfuvdvkd.sHtML

[C09] 递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gessoolee.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpmpcpti.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhhluuax.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqbwmscl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvclxqdrm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezwfykhf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gccjftorq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gonpmtmke.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlntkmht.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gcebmkbmz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/gujenkork.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/guhfvwnsj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/goszvfkyv.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/griiqsfgr.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gdifijwry.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxxkquu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqknergc.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhdrqopy.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghacpvzgg.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisiesbqp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekxhcfre.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/ghkhcojyp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnoiyzhv.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytzubuxp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmhqjuok.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/goybudxgg.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gmslsmxms.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fanxiaobao.xyz/Article/details/gpwirnjfp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkozvuhkt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwciuddgv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gwjxlkcvt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gasegilrk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxnffyzx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gsqnjuvlu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchfahpbh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpkiykld.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/gxduqjygp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcurlqfff.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gewggezed.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gatjpfapg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggtceemla.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzcablrh.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gvoskfazx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gqrziyayh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcizuvmhe.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrryvruf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gegzhdids.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxdipseo.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gioqdxazm.sHtML


<!-- 参考信息 -->