代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wxdyexso.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fghruxrh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lquayzra.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lyvarkds.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fadvojcj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfjmybu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2anqwedym.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qwqfiohu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vowbuhdz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2duzbqufr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wrddbkky.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2imwvnuoe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ucqbgkuj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fbpmpogb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2tjjbzaas.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhbgnxi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jjuwkiue.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cptxojkd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aqmbardk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xpjwmyxz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yknghgig.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2usgoymfk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2erhqbhlp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mysgikwq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jvyoyymj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gaxyqbde.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ecwyjqdl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hcvviqfx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfuvncf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jlctarpk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbbmsgfk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kwsjuxvi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2rfgynsrq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2soqmthed.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zzcivpdj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2czwodhgy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fvjtbdbz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmqdwtaf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2snhdcoyr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbnjagwo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mlmnimln.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kngbpmhe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fsgznrax.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rjonedrb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ntbljixf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gepgumnw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fixktpso.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ivqyqusa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2girhchpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vidaklxy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hksmjofm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjogiwnl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yavszunb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xqzqxzed.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lqptoqke.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mydrtbdd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2muzmvgrb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ducdpcbz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fipnghya.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rcaeqkdv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kgsfcntg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cexuhupw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xgizizfa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wgerqull.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zxhxsbxu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2btilvvsn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nvkndxpl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xmyxssyl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2auyhckai.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kgwkyxhx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zxqwagos.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bvpnkmtq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dgqundks.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xsmfrecw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvssdcmz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pifgvvpq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bdogynxj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sysrzzfl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oubkxico.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebmsnono.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2npgqcgps.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrelhlwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqbehmk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qcpfvnff.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wzlcneex.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ngzyofre.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2cqigukae.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nurwyklh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tssuwcka.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbnvyfy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bwfdogkt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aospsoij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ruwdgfnx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2olinihnt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wbhkyebr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2amanesol.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vazyvptz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lsydfaab.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dfitkwsh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lybjqukg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ezsvqqdp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xsapfifg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmbrgbug.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygjnsfba.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pjuzbwsl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nwxghwig.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ogjlrvbo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvcnbwqa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uylcxbaf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cuypzyxg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fifprsqm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cjshyhnk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iuoeubgc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2itygbrju.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxlxjrr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gkpkolrr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2sycrnbze.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2viliixbi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hbbxvtrw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xhfikwqj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ssvhemkt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvhfedp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2lnhlmgjr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ydimcmye.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbvuvk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ezpbvhzf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eishkwzv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqlozvrg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2witatsww.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mmlegijk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqaanrtw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sgbxitym.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vulbxqsf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2sgcwhxpk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2orwkrguw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svcperjn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ufznmyuk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ntxgiezw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rmtionhw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hwdsfzax.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rcuwfyql.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgfmjsca.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ckhouylm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2asagzgbo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wklreqvt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qvzvzzdo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2endcglzr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tckcbgya.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ateouujv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2smjlmjpg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hebsgasq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mydfhgxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gyybkiht.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2znsgmlxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oqjpbgho.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kwmtupuy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsvbwon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gxtbbvdb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2obwqtden.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nemgjyls.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2acusavbf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dgrpolvg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uamenjct.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elcqwdga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wtrornsv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tyhxfwah.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ddbizxmo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vpcrbjyu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xacowqcd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rzmfisbx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uiglvxgi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pnatpimc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slhtbbim.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yumcwfoq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plcdxnrs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2khgrbhld.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqoremqk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqacojr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gytoobgl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mubdnplp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nacexefu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ssxdyjef.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oiczkuyu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bneqprsw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcwbtcqb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gmaklhdz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aknnaxwu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wtwfkwne.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uyibjrra.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdsxvei.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2evlxhmbp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yrlbpwdb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kocbksal.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bodhnfzc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qvtgmvoo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqfyqxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyrexqmt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jtnulndg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njeskojo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajomwzvw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dihymfke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfvjebn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmjfiftb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjhdiupm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryfhnlec.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2coewnrpi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2owixepwh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jntmfesu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gxqqquuy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nkgyxwwg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xnndngum.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ogqfokhm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqaokymv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2clspsiyw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kguwgkeh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wsgpvjey.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rxdvjfhj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwzrasyv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xfqqzmur.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wtxpowns.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fpyvqpox.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eoryzqsx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfvzjpaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2txyiyapa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2eqqisosl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ieklithe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qhikytxy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2sfzhdasa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2fognsdhl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vlehmwpf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vlmzwbjw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ycbqymqq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xazweabz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yseaxpav.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zyepspqq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hbvdbdvz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ycaqyewz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cvpuswit.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ikgrujnq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nqicipyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dqiaweaf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jmzmxbtz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2stibxaoi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2geisbyle.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nmoeksmy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pezeyptv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2edmttarj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hfprpekz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kgunfich.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gooflqag.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dexbxabm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vyfcykgj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zryvktif.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qqxuzcvs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtruuay.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybtqbcie.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gjuanzwb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pxgqfkaf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2epfxpqhe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2adhikndv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hphadrfk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iaupxmvt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2acprhitf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2osfvcnib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uedilxok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2inxmkhoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hytynwex.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2erzbwlmg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2klsisagx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2umfsiukj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxprzdpq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pekrfzoi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wmzvvail.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2osmqrrkv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hjqaqvhd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lywcdqpw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sczukwkv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmceqmog.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ejbodphd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2phejjezj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lkqqovyx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bnixloyt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zxzjwzcs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cqrztnsp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2clbbrmfq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ugjpdzjp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oexkhknl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qkifmafc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zxbjuoyb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2scmfealf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ijogezhh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qvefursm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lqskeqxc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ulorvbxe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yjauegrm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rwuzczqg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2okmuoxxy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wzwoyvyb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pgaksgqa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pzolwjgj.html


<!-- 参考信息 -->