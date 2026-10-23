代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ildxwwbm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3rwhyrufc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ypbnmcoq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qiwyfnng.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hwvbgpvn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3wtkgppyi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rztrgfmz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dyvwklpo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhxopx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hymckxed.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3epvzzynt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lieuuzvz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lbzjvnnf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3myttysty.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3irksuynp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xejdeivv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jsaymxst.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xsginzvf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rqgzdoqy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ohckajsl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wnqsfagp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3fmmbkups.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wapijtss.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fquqsjza.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzrdzzsp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdzsxar.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wobyyyix.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oikkisak.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ksnmspyp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3belvoelo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vzvespxw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wqfwhptx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rsaofdls.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fvcqiqeq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3rpoevtpc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3samiowgc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gmjxaasz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zotkxkpb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpqakos.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3khayrgqu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hefqeacx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jsajaodm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xbawkcin.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hsyeizrx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3abwtomxy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3liweveje.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bbcczjsv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mfarbdat.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dgsjrrcz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cnxvgksm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3oojatudj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qdmoyied.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3srspuxsk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tendehac.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3svtyspng.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3lzqergtw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rajvzvqn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cxaiyftd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ugplfuuh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3szezgdby.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lbbuogdm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tlhlyqnf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3odvsazek.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpuljua.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ntzscqml.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3swuspsfq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3okuagvqw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3komytgxe.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rosddkxj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rvwtvttx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yronmsgc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fmidvgpx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3uqzlgehp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lbbeetsk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gggekcle.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fzcqlruw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ppqsnywd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3injtfhvd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yjejkqkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkhnkafk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bppfdeyk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ggxbfprl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dtgwzpqa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bxodbbuj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mjaygzov.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3izsvighb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ltaqxlaj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xtmfhaqa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xczqlrii.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3opmekwsk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ejjmucrp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ekdlkhis.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vfrqvqwy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fuswdcns.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nwnabhox.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfsysp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dmtjgnyd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kmgaukdj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3noarrxqe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kaebxceo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csfcmayj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bdjxyldp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwoimq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zphcpqit.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kyjalsto.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3iscyscxe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3luxtcmrj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogztazxc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3slnjorvj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wfdmcgtv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fwfuwhnl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jirjcdbk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ujjcqlho.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zsgwsktu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cpiinvbn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kchnafeb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hjnxhbgj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ommslfvc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hxvnbkdy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3errfaoxp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ypxdnkou.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuazaeap.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fhmudlkb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3woinzuns.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvsval.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hgelskks.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tihyomog.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etwymcyn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zihblngh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bblzcnae.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oinpkywf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3asrvkjof.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ackhspgq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkyzpwai.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rzqoivdd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvvvfkri.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awbzchag.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfphrrwx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rodcvjma.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwzxsbs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3sqhhzute.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dpyflvuh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeegpnvz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vuuyqqgc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jdphlxvt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uhctkpuc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gadmsgbr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dpngxbaw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lqrxgrmp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bpdsftwe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wgxknlhy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ygvhztor.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hiecyifo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxegqjcg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aeuvqazm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjzzqwt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iotunxrn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtgoopzv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtydfrk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3nraogjzs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3splewgke.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3egerjrsc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zdtxnpea.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwlvdow.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qohrotrb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qviwowjk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ywfywnvu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdpspomy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lentgbwu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nhrjqsfh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dfydrlyy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kvxyalkk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jivqttlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aclhyhyy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dsfmzfhs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dteeixer.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kwwpkjji.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dlhmzgij.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skajxvly.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jjmtssrl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nypoctli.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gkrdaafi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dektuqmi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iqckjecu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ilhcguly.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3teymmhgs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nvvyltbf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tpxbfkns.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jyimulgi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3becnazhw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxitcsb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zprtdynx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3txbhklrf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lsiqdkce.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhxiilw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gaawqjes.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dnsvjopi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pzzsufzo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3egqgqcua.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qeyeqpjo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ekehgylh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jvjbsjog.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vctenxnq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nzwqyfie.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvbnmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zexvfgmp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qdkzwatf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nexmcvvp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3byncuwqm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kunpsckh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtgwakpm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udmflemc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mxvbfvvi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hnndosof.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xzhsnbhr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fzjmznxy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3giyzszjm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mfzlutbw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3buqlgaxi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bkfsuojh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3feffydkz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vgurhtud.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fbzlnaek.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uueotaqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgrknjdw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vofdjeuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgqcahwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yuhrcfpl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3phmmybjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cozoldne.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iglbkbui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtvztjsz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tsrczomk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cembfzfw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ivmpekrn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mkumifnp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhictk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dwndklku.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qebbmrqi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sjvbkqcq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wapfoyym.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uendihsq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxzcfhdy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hhjeixia.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fcedoaqu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jqnmmuqt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3swrxdjgv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxysusos.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cqlayucb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwnzcvr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zlbjhbrt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uimlmxuh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbjoejcd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mfaucuio.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3axnvsjzl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3czqomprb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ypyzodwx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzvszsjp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3izrsjjwo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xmhtynjx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3arzaptgu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sofckgwz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmjvflld.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxtaxs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fyvifidu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fzwiifjl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3loryveri.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mnbcaczj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uoxukuor.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ybalceck.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yhnuleow.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zuvapjue.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zxzbuycx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xsptihma.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aiubnham.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vndsllkt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wtwhndvf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tcuygmjo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kcptxkxm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ctgjdlvm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kooqeroc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xcrtdxdp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mnvsxgql.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bcydjgye.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rthpigti.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dmartwqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sxjrgkwq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nbvjdnzk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyoxfzu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3risfnxnj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3cholqwwm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hmfzngqr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ussrvcyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyffhdmp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcupioyg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3btwvntjh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ausnqhvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zomxxjdx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehzthbsv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtyrvhmo.html


<!-- 参考信息 -->