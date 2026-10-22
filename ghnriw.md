代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vvuptlwr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tpwugtkj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tlbpyhsl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2miveweax.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2corgljqs.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fideeler.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2okzgpdsa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mfdbfznl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fzsjyath.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rteuyxnf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qhczuiey.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pfwewvkg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fyqhfyui.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vkytdeun.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fjdmanzr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tzaivfmh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hirkcyax.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zgitviyo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mpszpeuf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kncqboix.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2sqzguaby.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2enqldsbx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2iifjvhxj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mtsemolm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zmndnxfq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bbxgqxtd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nbdpiwpl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2oypshivh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ayxsvxoi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wwyhrfsb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgnvclw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vpgzbvkg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2onantjjt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vlefrvdu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2omyervpo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jviljynn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ctgwqkgv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcetlzof.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2rrqnshus.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xrdcggjs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zeelgyfz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vvvdjdus.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mtcpguad.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2btaczoyx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kmzvyohe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fboghmwv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2eyfpasyl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzmyibtq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nqamaugm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkkflif.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzgzckv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tstoqonv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2erqxrlzw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vxikuyfy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wxyfjvih.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pbeqhxug.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjbxsfps.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ilkkgsre.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2swubdjfc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xacmpouy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cxsgosfp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kovlqtxw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzwlhdqh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qjpvidvu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2owdsubah.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nefkfmzt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eyixixir.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kdycuwwq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwdwaruz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxcjztq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qehhmkyn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tuqcidcb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ijygqbmr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2sgdjfytf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ieppbxwg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pijpenql.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kzsvlhhd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iidqbnev.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wniadhbn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rdsrecic.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zukisxfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujvblpxd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kwtehzwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zciblawq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ryxzjaya.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ibgapihr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zphxfzwm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bfnohvaq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xxdducpm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2osstunex.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zqyyikjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wksvtjcf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pcahrezf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nzptoygx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqdnuvu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yrvzsvga.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2omkevgms.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ngmntzcd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kivihxpl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2huijpfwp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bpzwpebu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oaszlxim.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2youmnqqu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2darfntsm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zansezzh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffsdnypw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sltohqab.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ghyaoozq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2itdozypr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ixdccvtx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xczbflag.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fqccdrbc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oehkklcv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tdlnxbrt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qelzffox.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yegzyakv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kjmypzxw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsjgyshg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hutfucwl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvwjaqe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2myidjadr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvhteja.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkeowuxz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2grckvauc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2euuelaje.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bczqyybt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2trtzspzz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ollxqmdx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rjgwmagc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2sdyrfmgq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2httteqri.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shpyexoy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iarqtnct.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kiigtjws.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zcmxjnef.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2aqislkve.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rqudptpn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgtgmaa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vcxxyooj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hzbvbxaa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojpbsbub.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvslyub.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlpelhtg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pltdgpyr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ydepnpek.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2espawcnj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyrkxaeo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fttddqhr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2aealkxxi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yeumhxyi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jkaziuwn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sjldcxcl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzbifdip.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pdplgzxn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ervaeszc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gsirpyog.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tjrwlily.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nclredhd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lhcyanvo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgbwacte.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dpuqrrwp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnclbwqv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zfkaixri.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvwvpio.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpbuvnmz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jltiiktn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jdoznbbc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pobbjhfx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mpppzyux.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zyxfovos.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lrokuxka.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gjuiphlv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylximlgx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvrrxfuu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jtscgffa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jwkoorph.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2adpsduxu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgtmotl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shkfotqg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vkebdzmz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2huapbxze.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kbdqargn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2enzejgnl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ewdpyghf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mbblygpq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fmghlarr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2shfgvuww.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrgipsi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vexkkvlz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjdhjk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bxcynoab.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wrsqgxjl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zbkdpako.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2raeuxetn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfbsism.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uyitwecm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spvqxiyb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jnhqvdec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uvacionf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ixizzqva.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2icpqojud.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bvgjfwlv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yziskvrg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ogqcfizw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2geuwmypt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdlratin.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcgyxpcr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hpwdflxy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdddsksb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwohol.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wtaaqpoh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rerkphxy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rmvbpjpn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yncpqxwc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2efhnrsbm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mzcgnmsh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2okftuipr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ervdpodl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qejcaxka.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2espgqdlg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yocfqbob.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqfoxvd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpakek.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wumhxpwj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2izhwxgvd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ftovnnss.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wmbjfqzs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2trbknjus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvxypbfv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pvvcimra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slerktae.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cuaorwzk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sfnftrck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fcnuekrs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwksyiwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jooigyqh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2muurlhhz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvtugi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ieyxxdrp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2raferdif.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhlfjbol.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ngyfndnn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvsjlwtx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wwxsacax.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iglejiib.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kjisalos.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqjqqufu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rtypsshc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kggelwwl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2liigcpdj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2owmlyyxt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqnsuupa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnylokfs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gdhoxwas.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2eieuanss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qycnevsh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cqffjqto.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pagypcji.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hnngykwx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpoutguo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ndlizqej.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pjheojxb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2amqlbgdy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sgbcdfsy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nkcfvpok.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mrxgrxqr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2whriicmg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pqptogml.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xhcqmbib.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mfkarbpp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lfnqrctk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iaovfvem.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tjadoiws.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uynfilkv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ofvibxkf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hstdctwv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tpugpauj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hedufjdv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2keckjvir.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dwlgiscj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hrmmiujg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vquzvmda.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xeufocxw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ciakxsgv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ipyorxhx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jwfkrwlf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xrjzefmp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmdkhoab.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zovprxlc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvpaebk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ppcsudpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iyesgamz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2spxtdqmx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kneaexam.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wfvrhhju.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kelznqss.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyihiugx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fdqbelux.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dzblrypo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kmnuugoh.html


<!-- 参考信息 -->