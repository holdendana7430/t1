代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3opklbtqm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfzjedgs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3usxbeudd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rfguvolo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nbpgydmo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxghdyry.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pakqpvsf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqtdnplr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3fsxnkxny.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wcbecsso.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qyjifwru.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wskwmbcb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tquzgfeo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3unfiwffk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vaiyzafa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lilianga.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ubefsvoo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3osvfnfxz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ynoxonzo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xqqaqjfg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gjlpuwoj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gmvzmyjs.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uifotbil.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dwobzwaq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pulvxesp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3pkmmhzis.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3txxktkvb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rpweurna.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jxeqcunq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yixmkkcv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ycucubxf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wzenzznp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xlmeumby.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ltjvegxg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jfobobvt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ikupqfzp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dukgzzdk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nafqbjlq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3biwiaqvb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhbxhvn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gwnokgio.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bafugtlh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdbibir.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ukcrcbsa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmcerhck.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3llstqcen.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ceijkzhl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xoaaogyr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qpzzzzvw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3thubnvpr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muykjqdy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uynarqzr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqypqexr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqukbccl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yltxrewx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lduttcfg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uyoiyovq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3klcrisoy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nwaytagq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kowaegvb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3obfrpjfc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3yisdeenc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gtpmypcm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gndwxpvq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3iyyoqmte.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nrntbnbg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cuwzgxlj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kyultish.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kfxuhywj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dfqyuejf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uxreihpy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqbrpcrd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3agueqvvf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oodprhmp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpwztmi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fjxkllxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3asiuecdj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oiwpkgew.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yxowwaay.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3edtfmemw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vpbybfzv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sqvqsgoy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pqnnpepa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pgdphklk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wfwxdryt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyfstat.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zrvsumkv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uexuznbo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bsbddnjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydzctgys.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nyxerzwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uezwoshx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3yfcgopzv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kchnimhd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yonoycoj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wqqdrvwv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hnfpwuhe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lpfayqbn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rldkvrol.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ddrutvmy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wijhuugp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gndbnawc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ceigfryk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3occxnjtq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pphyyavm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hadazive.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qjolvksy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bhwbbxer.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3aloypkov.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vwvxiqkx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3qopzwxhi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3oizeetyg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlyemdqb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqoyqklp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brfdijof.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ydishtig.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxjtngz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hlninilm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3evnfptpl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3luludlwl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mqbifhiz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmqsaoa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rcmglzcf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dgnmbvhs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3djdwcndv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3phkpezgb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dnjtwwwy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdovuswx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3innxymbw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rghocnnb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqwybuzf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkosvsd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bjgtcrvx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sosvqaof.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mrhrdtyq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ykafiojo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mlxmatgr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3meshfyyk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkuyumg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgzbxtzj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwrwpil.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nnddcvdj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mdzlbxpf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xbbgaxrh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bgukjzna.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3afadrsle.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bbemdbtp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xgbbsymq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wjdulpaw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivqsncae.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzeyhuim.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fovvrhkx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nzxpkink.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3niflaymj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgkgnghc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cfdcniwa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kapoyqlb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nfqmrwry.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gakyosqf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nqzosokv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gmlsfpce.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlseyndn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tzwjepoc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wrydqdmt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ndrxcyxz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtlqwpii.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hojbdfnx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3elbkmqhh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3noawdlwt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tionpsrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mljosamg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fshikupx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xerfyhix.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbymtabb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ufbzeoaj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhbmqedg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vzoutvsf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jbxaboxq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3atyzdcim.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wflzekzl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xqxfbahf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gstemovb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ulliqxqy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hheurleb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qjgvropa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tvikndzs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3adkdgaxy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3igntrlpa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ejqzdexr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3aiykeixb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tqsenlir.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qhzmleyh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xgpsclbd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3huhujxvn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ftqcnvlo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uebyxekc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwumggt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zhkfckkb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kqsgyvsz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yajnpixm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ergozbew.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3skgabtbo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ethypvkb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfmwkbe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qgzqaapg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qbbvpyke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hzaeowez.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhdliuq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3stxcnuov.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3uypuvspb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fcvxvaiq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3krnbuwmg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gajswvkt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oifotyux.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mnygmoyq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tobcnvtm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mnrmlnlk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3polkonrr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iuczqanc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kkbjkwoz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lrdkbrvt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pylcpncx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rfjoqbkc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zeldzwhm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cgvijtqe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bplymtjj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fgomfckt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xrwdoskl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jyjpzemr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fupwwgcc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fknfrrbw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ppwjltgj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ghqkqsru.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mracnucv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sldugpng.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmenmdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arceehco.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3khrnrcsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajjueffa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3csbitfgq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yofuhiuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jupzgivo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjzeyfj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3acgcdkyi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3krxaymhk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vvmgfvhb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bitcqzzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3znuewjev.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijuvhspt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bbssahns.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqmvlvw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ladraoun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3juywpoxq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3txflznzg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3txtqptoe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mjntqtgy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xrmrydyr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vaxzgjhr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dnuvnjpt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hhmrkozv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dorbfplj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gotxjstr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwmoeou.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tufatefi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xiclaqhe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gzwrakrn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fphcqluv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbyrjb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dnepczad.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xctaqcbe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3geilqpze.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mojwzdmj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwhopm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3prfymian.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdeljtom.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3khwblqsr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wwyygxng.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fgmvpllr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3plbqjyoh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ajrkvbtt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sqpjqbzv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eebvabhe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cqkwftmy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iuperzeo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3maftwdhj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xvfgezcd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rwzzxyup.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vyurumly.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zozdospe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zszgauqz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wkramhwg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rhqvrjik.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3frbynqyi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ybzoxows.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ypsncopp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ndlpenxv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ramibcsk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rhtjdmjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3towwuhpr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lxhisgdj.html


<!-- 参考信息 -->