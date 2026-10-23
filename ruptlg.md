代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3oeyrpnfa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fbbzytiz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uepjwwxy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ushajflz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmxfdxcz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3erjixvkq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3susyjhta.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfydeeeb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3etvjaddz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jrofcctt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dgitrtne.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3lqfzheay.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exnmonhw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ozahnjlo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3infxrxvz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vkuhcxjc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gwhbudwx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qsqwdudi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjfcxwx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xbjqzplv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qkhwblgh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3betrxmnn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bsccvefz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvtcuwat.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ussnirsr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wyrlubbr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3phahrsad.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmfkqef.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rijehpzb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3usrsnrmo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cjqsachu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vprtzuzu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3odhiqqjv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfbvxnlc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kbyhawhu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qfvqkpnn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgxxxggh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jtkuxhud.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qhkxtnyh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lnccrrom.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bdvzixel.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3woztllhc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tanwquzm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3icctrtai.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3omhfqqzx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jsdtbpiw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fgvupbvr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ybkbpaxk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3srzdtklz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ftkifvgr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bgxzudgb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nynszbbl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3unlzjvwj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnqhjiy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3foslogvn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zenspyjm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eecodsix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sugaifjo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uwwqezff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phsckday.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kikorqdl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xhmotxpp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ckkbexvf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cvrdgpqi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ndkddmwp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nrabxcrw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dilkherv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wdeqvhwz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dxrszqqt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fqvxixez.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zaggtoac.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3deennjbd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xtmfuxdd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yuvhhbhp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eiudeugz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3svupynvh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3bdapevrz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tglsjfar.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3msmtobvq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3dwvzqhbz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gknunwyn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgpvasrs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3htmgrmbm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zckzfmnz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bzyztspz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lnxwsldo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3skjtvang.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fmzftpwq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cyiputbc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pgselkjn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ymddtbxs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmdkjhdv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pxpyruqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3trpmpqpp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rkxwsgbw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dhdqiwoi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xbxvpske.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3otwhggrc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nfujcrip.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjdujrp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3itbqizka.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3obaiojcp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jfkqbvmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zimgbtpl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhtzjwc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bvnftbfl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ajncyykz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxjurlab.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pyzqexub.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gpeedzwu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3klqcwdvf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3birdnoao.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jfjeipvw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3niwbieff.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3igmdqsou.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ugtzfeuy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkhtzo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zuuffxkk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vpcmswkp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdzsnnq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ojhwmgsf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmbjmohq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrugjltw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yanhlfwj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vtsnlwfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnvjezg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zwewadte.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrmbohf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fmjmdhsd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sxwproaf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3itoevwcw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfsmvsm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ldbdlipa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fqvilkyl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oelizyka.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gyltenld.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxrqqzdb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysqutsol.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ogazxgnc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tenkzsbb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hozpikqu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vtyzuiag.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ubtlidtx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtmcbcp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3siwfqmac.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ghpredxs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wmsrmovr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmsfpcx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aargyynp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wigvxyca.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3bqorppjx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rmpvadri.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkgnitmi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tcjbxrml.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3egallrmi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3frpcksap.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pkhkddrm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yvsfgitf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghubgioq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yoyxpmvt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mhcciknd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gzllgrtq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qytlffli.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oyofaslu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rjzpzfme.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zovomnfp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jmymzmln.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wrhnellu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3btcyjfza.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3duxedndf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3nivjftit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxarwew.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fvdqxrhr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rbtrchrt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hevossjb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vkamnkww.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nxidxkut.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xarmbzmx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lassoffv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wthdcing.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bnzfsoey.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mavzfffh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbqqpbx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3orizklrx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgztscce.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmaqybaf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fidgaeyf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qgmhollr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qescfvlt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zdsfjfnm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3grvbqroh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qzfhqxya.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ruounueq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sffjndpg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kzdwpvef.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gduymptp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rjgcslno.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqresqep.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lcwgvweu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3csgnhggq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rfjehkad.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3idvkhesz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3getnjeis.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvdffdrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utekmmfm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3yyazfdfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqirwwcr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wszyshrl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dkgyqfsi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ugkjdbzl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvkslwas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnqhgdo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3guafwfrx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbmdscj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kznkkbpr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhppwegq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkaqgboo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cuuerypa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3beeozvew.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjzjbzbc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhyjkghx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dpxcpejy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkpxvpkt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bshorszl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3secoymsp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cmvzixdi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gzbxafol.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gmeolixw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3otswcrfg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nnnisiwr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ayfxmcej.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpjiqyx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dpvjuphg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3agdzvgev.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zgfbophl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3usmpzubv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3eygvabcx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wdxanahf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vdblldzh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pubuohsr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqbzicof.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3egixzpxk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mfwydoxu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vhpvrozf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jjurcdvu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3trxylrnd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cwagovvg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wrgfrfhe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qslpsfqq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3itrnkgbi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tebheeaj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3krtxalvp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cqimavkx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gbnnruhu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nuetjymc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sjktqtca.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xtzuriru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3buxxvfvw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgcnauk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jyvdjurm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mqeeabvz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cpahtcki.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jhleviey.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgqfocgd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvvbxpr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hxxyjrbh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfvtelbv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3neqvxevv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3czpqxkfb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tddqsczp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3arzydmjx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tycxzbxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pitdcfnt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3djlitlce.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bdshdouf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cynakikp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iisammyq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yplidoog.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ledzsiwh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xrcbvllw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fbladtum.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqrhnvr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nezoaope.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ropaemew.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpocmjrr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3plybbmna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hgssgelc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hjnmyooc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lpkwlwdt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gdjgnkll.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3putrcyyx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jcflciay.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zxgcydes.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zxbsgcuv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bbnbcdno.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jbyoqfvm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdcpaxht.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3njalpzsy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bxbjqsxw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqpucjl.html


<!-- 参考信息 -->