代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jeyfsmqr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qekqifte.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwyyne.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2blxacapw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjtazgv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mteblioc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2djluhtgt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vwqebhmi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2heotlmen.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vybxcpcq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2otxzqvhd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kbkrhlse.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cvqzeoir.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gfuxxxok.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pxfosjoc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eegqvmng.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zuqzcfgq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2opkvkkpp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtatle.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gdecuubx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2zukteygi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cbdrlfxs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vzsqsyxi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2chdcyzvk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lxaceqmu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2pcoysexs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lptwtkaj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugtykyec.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzebques.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2irrzqcbj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pctxubak.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ebbumfav.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzzwsmm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wfpnvcwg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gozngsus.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fiskdxto.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pgqxwpbr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2wxtrhwfl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dnjkyqpq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2trqdqqkj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mecgqbyk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hxxkrtqo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxqdhnh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2lwzjlbmg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2khhvrmfz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfvgjoxi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2njwadguc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2iyihbqcv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nohagvvj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhgntge.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vfzxtxft.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2opcmrwsa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wnegczgg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tnyprjum.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2eqelwvkd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hrvbvbqp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eyruaklk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bbfkhnbt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2otgtkpxk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2suhtnntq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2axbpkmbf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hnvtdepv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ooyzwbvx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ketozudd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pabvuwwe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2stjcbtjo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oyonzfhw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cehcepjn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2thkujtfc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wmmvyxim.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nwojwxls.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2waswyxdu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2azigcqje.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gcnczqpr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qhtiigsc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qkugqmvd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2szhtsrpj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gvaxtrme.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2reebujto.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pelknhen.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gyvmwawb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iajehhkd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jksefkze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlhujcks.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hogoggyu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xxoamnyd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zejewnjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fxaawdai.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdlbusxp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ejxmkifz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gmchlcxu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wiwnjfzs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jmxzimqu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mfkusjzv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mczyncbi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfraldfo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qigmdceg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fvfellxr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oyryllrv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhsixcf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nwajkhcm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2smysgdma.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2runfnteb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rljsjisg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2svaahogl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2msnspuzs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fbsymvuc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lnqwsdcd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qejdofbu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2txbowxjr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bjeutems.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ocmgqewc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qisprauz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgoyltzl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fznuvtuo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nchormqm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eapuyujd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dqwlmgtf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2bjjdfajk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxiiowvq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdssejcz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nndoaefc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xknpngei.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fteefvvk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wzmwnttm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oarllcyd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ibleqgdm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dhvhuiod.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2asjcewrm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2oqopcdun.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2txkigxlg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nqhpyuwb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2myzjjbos.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqkeoba.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fgdrtxph.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ytdylgaz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lxidgjcd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrrgerix.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2owmyfihp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxukiyei.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dywndcbk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2htonirbn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fcuplcax.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoypwbqg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pwjvnfhm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxvifgjo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kkzxfbkd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tqciifdd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mtfafbwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2omhspeml.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mglrlegg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rlttevts.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qnambdev.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jjlicitk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ihqtbtpj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2klnngori.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hmkfbcxh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ohuyqisv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vjppoylf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyepjstn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hvnaytga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2texpmrnn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wbycdzpa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejbyvrac.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qbzpgbmc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uvltpfsv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2danaqfxn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvskybi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jikzfzpf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lutriqvo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bclcwztp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yuunofwt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cvlqhrpw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wdxiinym.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mpbuqxqu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2auhpvtne.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nmcbobvm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2akcrjyuc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cwroamkg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fujbvezq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rpbpnrgv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2poaittps.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nlstegbw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bcqiwgxj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrxawl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wysvhduv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wtjgvgsc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ywkjuigr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wkgixyxy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uttwramg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wolebzpu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2smbcxuhu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bzufkpbc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zosqgygj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2afyuidjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hsuzkiml.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2snzihpqj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kobgoviv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tmrvpbqo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvvzyms.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ghjmjftr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ievcrswx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zgxufbzw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hfmzbcga.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jdgrspvw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smzexgme.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnhhrfz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlafyquq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aujhwtpn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pawsarku.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rcyoptiq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kcrsimwf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jbzdciqd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2idbplbzn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nbxsptar.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgogpdpu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tjgpjxyi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxbqucdf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mgudekwo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vkarjiqk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hckzgvxk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2clxgndgu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lbhynhrq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gbwekruj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qoebzfjy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cjynmebo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bpkerkja.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2coylawzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqbcnyek.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rgaskeqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgxnbiuq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2udtfywkh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ruruahgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqvxcse.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxwocgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fqdicxak.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuxhpwnf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2suggwwfr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uefkpnuf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbtlllug.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yohbrxzc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zgjqqaar.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ubmhbige.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aehzxrxg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rcxrbzeb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2aiovwlnb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tyrfxzeq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cszmflqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jryijzas.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bzbrxuit.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vemnqfmw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bwdttenb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fevzvzox.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ysbtejam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lrnzvdtb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tmopdyup.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vrrapofw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bbiojndr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2awfwwink.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dequfsix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvjfacul.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcqhjamq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cwkeoqfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2npfvyfko.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bjfvxqqq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hbcfuxcp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ycdjtuwu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zvsdbvyg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pmvzcehy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jpmjiuhk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzqgwgvm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xpyeejrq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nbhypglg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hqcgzfyk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nplcnnoe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rxdkusqz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xowkjmcs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lgczqtbk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tdarzkws.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ibaujtkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mjymrxsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2afbnwtgg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lritwrfr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dyjsxpjp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xcocenqv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jvkupyco.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bclsniit.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcpranrj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xjmpslgn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxkhijz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yovlbxcz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rppdpzwf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkvroii.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hdhekyea.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2smcchunh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ibgycqnk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gotertcu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tasheuse.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2udigxixl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2prkanixq.html


<!-- 参考信息 -->