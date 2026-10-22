代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2joikjlwm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2razpjbgz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcrmvgnp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2easblrpg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2blialidt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vcrxvlzh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2inszqnsn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ibbalzin.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lrpjwtkf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2aypinfkm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qmsqhjva.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lprjjnvr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ikzayenx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ztiynxwt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xqqjlcfb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2yparcmss.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mirsuolf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2exxrhwyz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hpybzlvg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hkvzlwzs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rsfnqozy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bimzjbmp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rushtnxr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fnjgnrzo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2grntwoux.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vvdjfntd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2eeiejfvq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ufxyvpbd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tgpzcafw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2edhopfqy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2zsunrytl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kcewrhfu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2odvooeqw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cpxzdoal.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihocfudk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiynmtka.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfbuadt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sdsizpru.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wyjtocwz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rncpxqja.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hgwshmof.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2pnlfyixv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2twhcedhw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jguvmmqo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qpxxmmnh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bzyqrwti.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kphcgduf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xjkrjdex.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ryfhppgn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ikiozusw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qxukjhbx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vtsqudxd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aqpksrru.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nyvrqtfi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qprmynjc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjknnpoa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wqtoewmh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pktnyijd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2prdhsenq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fofdxruy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlxehvg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jpmsexfj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dlaoayqa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ztqcjphv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bvbohbsv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zekjerhq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ammguznc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tqbskljo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jllzidvn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbffxrhc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqngffl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpfywch.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jorvagqr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2powkohsl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pnvtgnbv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkgngid.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2myazjstk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qfsffznt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2teiggfhx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2zdagdpfd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2egfyqqpw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jmmowsea.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dobtjttk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnmpnk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oakggwce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbccmlto.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xzekvwfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjmkhy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mcxutnnm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sxfmlhaf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2quuvmnif.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uqjzltvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2migavmno.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qzaegggw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2sovdzvvs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qcznbbix.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2plyfnztq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ccaarkfx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ocedohbf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2pmhhtdzc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zaucxcbv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2covnoeqt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wnsraorj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rojrstmy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2esmicrvy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aqgkruoo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2thwmjzwo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tuzaivyc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdftvmu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foodyngb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upgybpfi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtrhttd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qzqswbak.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2okpawaxe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sdidtips.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2utvgtyhr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2srrqrehj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksxqpowx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhatmxvx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcsrbcs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxoeehtl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkvhhjg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fdznqfnl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ijkjskwr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mfgdrveh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vradmaqs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qekwivoh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2asnyfcre.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pdodjrbq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hdrwwuml.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbfbbkfd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vdmtmywj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2psoewvtt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fbewmhph.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pebcjgni.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljaswsaa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2recgkuyr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xthcgyvb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xnqoapgu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2eoanegsh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2znuywnix.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ypbfpxpj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nzvqxnid.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oublmits.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qtscqnkh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ptfnztkn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2beemotau.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcggctgy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rdcmxlaz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dzlwxocx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdhyap.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2betnjdgd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2btofxdlr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zptdqyqv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rwbzyprw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2naddbezw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pzxjphzu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eoozfwxa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mixcdmoy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pysbszfs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2umbexnhy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fnrvisuq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ciylwkxp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtckwtg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hriwoatp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndzdhsae.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uopleujt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbiovho.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbxuwzxi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bbwnmjqf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ygtswqdf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whgxzqxu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rrbtvxxc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2snwrpfml.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwagpn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2esvjcosa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzhmvell.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2bsoffizg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hmefbkjm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mydyeuvb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zydmrpww.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hxpvxeln.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hweyekir.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cfsrfhlg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zwbqxues.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxwvri.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odtztwgx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qkumwslf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cqexjlea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nbxbhaeq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmduzkgx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2beonuhiy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wlwejgwg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ggekuwqs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yqplbtso.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mbggylor.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2eyzloxpl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hmygwywt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cblrrtdv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ialaqkmr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xdwynlxi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wflthlhc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lnwkzhlv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vtqceawj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kxyebhkp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zfidvqbh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tpgvcmxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kevnfkfd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rmvithom.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trbtktnw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zmsslucd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2myxokxka.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pqyijfrh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fxqpuwub.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sgrxovjx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xnbekipb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fztcoyum.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pyllzmiv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2syewfwfa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2udcbsair.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nipgzban.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rhztmiwm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2frkcowdq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hgkhwdzi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2knqtzdsk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaznftuc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cguhgyzi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxvzdio.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rciywbvb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jhwibhgw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pjkokczu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hrskqeux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hazimlnh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rtfhzxkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehvgpyjl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dvgltbpr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rencnfmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yaerbffz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpfquch.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rnpcgjsc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jhiwtjlq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2diwwoxpt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vahspuih.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vyajzeow.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpsyoklm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ghmngdmv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyedndva.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wgwcrsef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ctsgbicd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fubssedy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfmmtqit.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uoxbalgf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rgifigif.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cslgdpdj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2omfwflxc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rtlsvqvy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cyxmdkrn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hvqdnhpk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqqdilcm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jbindqou.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zpjhwepl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2heanfotu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zkaxsend.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zrrfadwv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2goalngfm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpbsiail.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uyyfjwaj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mcxgvtvp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2oftpauuf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ifstyweu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bmvztzsq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2unzgoeev.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oggbyfpy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jvtetnjb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qjobrvgi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tlueavif.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtbntu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dqtlbymv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxltnv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dgziswqy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mzpbgjnk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jrmgxzxm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvsoofsz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2docyynlt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxpekdqw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnriyyiz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uaupardo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aahylbli.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eqwhyiiy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hrnylkgo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfwwlgj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xgufkmhz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cvejpdtz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwxsdnz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bxjxquqd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vmzlsvxj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dcemoesa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ndyerjip.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mmatuayn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lznxpton.html


<!-- 参考信息 -->