代发 wailian999

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xutenbna.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jrceyzyt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dbsviltw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2drjyfmce.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yljbnevu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zqtxilrv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ufzykntw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rstvuebd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2isczunbr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hdwqnirk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2reuatrgl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rmnhxyeo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jrlhoeuq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2naoytonk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yrnrynmg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zbwlpnhi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qoltmyrk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2nteewuud.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2bxdwrdng.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ptiuyzvh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2cgzlgkox.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wkjodlub.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wyevkrma.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jwmunfkx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mqnuzkpw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2evosgara.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nirvsmja.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mauwntvw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2utshocfe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyswdsxe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhjrlfgu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxvrmqyh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgxybjs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2scinmzgb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jhsuahev.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nmswngzk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nsaawufb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wmadjvyo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qcafwrur.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2llpuyyzy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uweyhwqb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zirqnxtu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dtktvabi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dvaaqoax.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2azpwvbur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyoaufmf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2auyrjxel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evcvtkac.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pmutlesz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ophwgzvm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ipngozql.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pjgisvna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ijlnvdgf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lpwspitb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2lpkhkkqr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xfydetfm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vgibhwvo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hjfepocs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2iejlchyb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbiqbwto.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dmwhtecn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mrvgsjma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lwklbajm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2npagltwf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lnalaudi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pyhrqsyt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yglptdft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vxqzssab.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ondzzmkk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qajqxvrf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hrrwdxal.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gjushhph.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppqgxyfk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2txonngbd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2groklmdz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ddqznkpj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jhskrdth.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtroyam.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnopbfo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wbsiygut.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2schdcrtv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2unpsrnmn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ubocoiah.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2foykkxik.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxlqmt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnzyyhz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlqybiab.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zlzeoays.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2baqzfrpd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mftlihqr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2prsbenya.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hdbpjovr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fbtbgzld.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2weijtwjo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tnirzqwg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cifmhfdq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zonmuaax.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rjrqjpjo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lphubglc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjohqvc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bwxekigv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcbniejr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2isaettaw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2imtdplse.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2aiapvecm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2efotdkqx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2voggigbo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fshblqnz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nywgvwrd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ifyvfdmo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbybakie.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ublktwkq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2omtyxdac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lvhhbnpf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iawysgpr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pvrkpsen.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kczgkdcj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wicxliwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pvyrmgpn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nvbajepg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2aeibvido.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fixowgad.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzzqkfxz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwqjykf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yourxrid.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijesncna.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpangqg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nahgxpsi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fifkpnzi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pyphdftl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jpbkqlop.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etjccgxb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uzbadncw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2irgljbnx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xlsnvhez.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vilzrxjm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ojezmtmk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjqezsk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2forimaqt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hoguchmp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjvymgxg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2educrqpp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wsemvqpj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mciqkfuz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2arklkpuu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gwzxrnrf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgpoxiuz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2chmuuixg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ktphupxm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lsthcocq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nawsewle.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fujvpver.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hdkhtptr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bkcuhtwk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dthsrvse.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qhukkahw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dtabvvvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jveotrhb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipelswbm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fqntxyoh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzceyisf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uzmtfikv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rageglek.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pfneauqt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jzwkzvho.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cqekqueg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pxsmwaez.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nsgeoghu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swfmsjbk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2icwwrnbs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ofbxnelh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lqniadqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfogcedz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuchpgar.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aljmqwho.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hbrlzakw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ndlvnazb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2shklbxnn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hvoldxsv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yyycxvzg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aswkibwq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aybkbprn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nnxfmvtg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2sqoqhzxi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dcepbbws.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2faqewdjl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uqpttvrj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lhhagaor.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2htfjgskw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrxtesa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2skuxdqwg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eyaamopc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2untucorp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qrgsbyvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peabtgtl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rbqutjkk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cgwcxbyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pkjfqtrv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmypelpc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vuvvzgjw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nfkpeyxv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ahcnppxo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uutsnrpa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndioloxr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yexlqxmp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lcktslmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzaotbve.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkalsguk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2heiuwbob.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ejawuopg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcyxagfe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bsqjovew.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cerxrtka.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wseyjjrz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ranezvti.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2csfagqtk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qwjbjeph.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmhsvnp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgzzfden.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zvhtmunm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lkaadncg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ldcxqmqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zknatbpd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ilcxpqnu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kkbuklfb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oypgmwmc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2knpiuthk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2csrckzgg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwhbrwnn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqfrehac.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2skpexoxv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2shtxywee.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zvtxwvjm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wkbvixwg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kgwlohxk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eecjrgkc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eadfbndn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vwdhaoxp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fjdwhqxt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ylkqmzug.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mdzbnqji.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lrsiaect.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2slebnpjl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2giepqhsj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ykkxbzzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qmhqjyru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bssyorey.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rcojrbyt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jammdnfs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tqlldbud.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lawbacui.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vsksebzb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bsntxwpl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vhydhvfw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fzvaxyah.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2aojbkele.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xixcgqtp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uxeyxifa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nlroodtt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2upcqylff.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2godcnfzf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oynrvhyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cgswqknx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aguxnmjh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bekyjsdr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lzfypeqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2efiuokdy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wajatarf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzoelosq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2funshxgl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ulokztxr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vrprqixt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wfuwrhpi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gymzfcwx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ktcfcdlx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybymsgii.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxvcvqer.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rclwekfn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qxtfduqj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owjdqijd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dqsjsvge.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qcwntpqf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pulymrrl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2puhdycbx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ueoxxfxy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jaysjpbd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yynvbkkq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nbhimleg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yceyhwga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwildf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wmxgopqd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lrruicsa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sxgfluqv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2joxkkcdf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kijrhfcw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ozivofcs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2siuaxylu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yecehczt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oucjgqwv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2okshnqsf.html


<!-- 参考信息 -->