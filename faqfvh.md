代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbszzu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vzozmnap.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ibdnviha.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lojcfxui.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxmuufrh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ixfkcboz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2bxhxvcil.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xgtzukwj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2enoebbme.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xuqombli.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kldrrbtl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zvrxcfle.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jywjhevw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vnzkerfh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pyvnvvtn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ssndekiy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2olxqoghi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzgxkjj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jlwrzbsm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqaciksc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2glibcsnt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bhgxvnku.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nifgwsnh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qwsltxxb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcphfnur.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uaafuyay.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bgekoleb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jdggibgf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkmljckx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2aoephpuj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2txxnbxgk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2diavltpu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qwlucixr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2htzzzoyh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjfjnbz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtjjqmy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pucnbnnp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iaepaouz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mynlnirq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jzjvnxhj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tfqtcgyx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2byfipawj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ativnpac.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nofogyav.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kerwdmlw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nngdcshi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qcdjihsz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hqauscet.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lvxyncmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmavylzt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tqfinktc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oezbbaex.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nnebwlzx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wzywsqfp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2whpguwuy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gvyyukrc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2budyxzpx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ftpwzqsf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwjmfik.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2eutybssj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vtwauhnw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gzfbbbwd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nqqhdxpl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2awxrliwe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kohevqjq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2abmuojgc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nespjbqj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2grfehgxe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2szqcnsdy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mcpjignx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cmiunkbf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bwjtvybg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2znsxfebm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpkvssl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qlrsclxx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmeejfn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iiyyphza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bvfbxtpb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mzvosaer.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bugxeybf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cricabeh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvahrnj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lxnevzcl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxjosph.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2psrvszom.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qurjirra.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fdvftbpc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfwbgeu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xtzpdeww.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2cqywebbf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtfywhvp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2figqkzvr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ramyxlzk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjtuddb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2aldppomg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gzfcbtcc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fhleegih.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wehwboln.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cafwsehz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gxpzzzfh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uazumbei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wvsqjhiq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2taxhhqgt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sgjfcygg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2alboyrnt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnimvgf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2crwktupv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgwsiwyt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iimqtmld.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2allgjaey.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuygznq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jbypingr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lzqynntb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ockfelbe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wbzcdzzw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ullsuafo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hzeztotk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vwbmvrrf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hblocggw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2veerabvl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbiadndg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zuxfxkpg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2igikkttv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptvwdoho.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2iyaepvmg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2emzkuktx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tjuwzwme.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kewlunji.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmtjqlou.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dzsfrzkb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cgzzwtfq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dsddktpj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jarpolbz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cyhfylld.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rfyehemt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhoaqukd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qqpbokul.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2muoqhyjp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2narmxigv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zfolfhcg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vwfouefl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zwcdxznw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zeoicenr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wuzfswxd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wwwmdshl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dumqcwby.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umayszad.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nivwolkf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2btvwffog.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qzfpwocd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2iecuhonj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygegqkyw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yvszydig.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2owpkjocw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jtffplwr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rhqawqhq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ekohitnm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ozdoivru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vtldfqve.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wexjzlky.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2apsrafvg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pbuyzdcs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohwxcfpr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vynuvhxh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mqkobcsg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hxfbtule.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bbmxqfkh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjdhhoy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ehclluji.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lpvooixj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qvjmwmam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ynaoflbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msvzpmfe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tjjubpos.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gflqcnyi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ivfrprwn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hegsshkb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zsacecjo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2erbizmmp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fctizaha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2assmzrkm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bjdmbsem.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wdcohhhx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2spfguato.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fuljlgnb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dxfspijp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pqjaigsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rbsugfry.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zqlhozwj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjaiaiay.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhxlxwqs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yagymwyt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ndciciol.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2utvwdvxc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2djlajmxm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2npxsupyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msszldlz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mvddafnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xndwttmm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qzcezumh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fjmtoevh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hphopvxh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sunvwmxb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fagxwlzx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnyoghyf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ebwzvqzf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mmakdogm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqhsvda.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ocvzczsk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yrgwlshj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xklpzpzi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dtpqzslh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2opjximxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2igzyvrtn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijpnmovu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fzgzdkbb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sfxfwqxa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2opgfxsgm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2saibcrgk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2adaigenk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rpncmlat.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zmsxguis.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dezadllz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbwqwlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tzqodoaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ftgqqtoc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdkqupge.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkazdmcg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hwwmkwnv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vobrjtgg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xywrejeb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tdxrbtyz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gejxmqzl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzhtyrt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2satkkgda.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qmkmqasc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rzyadzwi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tilftdor.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2judqensy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ngniosea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2taazjeug.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2slyjnbjj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nfzpzbnx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mkelhibh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ofxpenxp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2piavptfb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ioctjlez.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2huftjmfo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyrkekey.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2otdneegi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nkuvlndh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pfzmbmet.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oenrultu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hevzrljp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nwqjhzjr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykwkhapf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vtthmhjm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aiuuvgsb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mefkjalb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jaxyawfi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2penjjtvo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ljvzwsrf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hstxezat.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dpeyabhq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2berurnag.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssrdniup.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfpgxqgq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kufszdzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rupmjmgw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2adrqxbqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qznmzuqz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jbtpjvva.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wktobfnk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xkpyhfct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mzrtjpde.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mhowrajz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2icpbnxxv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzolkuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2phbaplxd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nabeufbv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgdiek.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zhzglkcc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ebglonvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ewfyijgr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2obgtrpfz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2foljbyxi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yahkdyhq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wfqimebg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bpglakok.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mklzyoir.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ulxmlidz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oonmgvls.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jfjvlnzd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fdwjmupi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bpezzyfi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2crlukkwq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tywcoeen.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2avupunlp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ygvwliso.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zxjbesmq.html


<!-- 参考信息 -->