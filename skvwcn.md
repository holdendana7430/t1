代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3meypfdqh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3emhmqxan.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zaxcsleo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdndiirg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hlerghud.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ijwcgwce.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3amfypsud.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svivaodx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ozyftoqb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vjrcddrk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvmptdp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zifspwyb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fattniyj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3pewtclkp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3opqmsxxu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3uxnaqtnu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mgyrxcjq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3djkyfexq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nxoayqst.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lmkjfqmd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pybynyep.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ouvjdiln.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tsrqhybx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rtaquuue.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ujbrymxs.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qapyuqbp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cpnacroc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ugwurszl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3lewsprpf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dbhoknfe.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cjvvmohs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wmvywzbl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3liiiqadw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3vqayneii.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3joeioeaa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lntvgwmv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3axeohyzy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vgbvfsvm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mofvxcfr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uzbwesij.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hdxkdthq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ponldmom.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fddsxrrn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xyrbajqx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3owfffomn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3raxagtda.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ektbcstt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3bclqavod.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pgjumkiv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bjqksodf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ysqaxgut.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3svmejzmb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ofrtwioa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3thoukbyl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3avfvcccf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zgvlxtri.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ujyayrpl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3othwjvbm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hpetivnx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szbcvkmi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eeqofuac.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tbupwwgv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ojvobmfn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wrcwndwt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rxhwapqx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ktjzaqqz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzvwgszs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3koykwlil.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wwnrorni.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3leljggtf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lkuohhno.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cnlimcyz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3aueyehan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3insswxwb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dzcyqhmy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3azeeilcr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rbidkoft.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjlnnzi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tlzopces.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3eoabhekd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ltftxbpr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wliqfscv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3afwazcnf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pvhojjmt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3aymbedbs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rpvikcfy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vdpgahuw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sbsdophn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ngswzbju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utesbttn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3rubsmlte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obiozceb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3shyazeqv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vxxudqhj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xormaout.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oyobzlna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uoavihxh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yzkikeuh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3jvaovbum.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3iuaceetf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hiymxuyl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wrprrils.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dxojvqxu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqrylyoi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ptaanmuc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hgnokmpv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sytpkvdw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3eyywmmiz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrkcqo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uzileanq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ekchycdx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3elxrzyqs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fmxpzwlz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qlphrdoc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtibhyji.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwwsysae.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qldibipq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3astoeglo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bhkzeuqz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ybglrczk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxlzzqk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3roblbugd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qqimmsnh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nwfisgkp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3murneivo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdwpyeuq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vfiugsma.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3kxjduvfc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nwhomtps.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eiaujxtx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3flzjctdy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iyemrvka.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dgzqtmfl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3woigruqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yvhugknk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkxslfe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gvjbldrk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ljeycqdz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jjlshyga.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aildbslv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hnkdjldz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxsykkha.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xvucrqxq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjymjhup.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmjalnjb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tskiocac.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nhgrjxsc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhluotwd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zmilborn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gtkdxocc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ygqheaxm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xjeufmws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mhjmgdjn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fvarnuxd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwudxldr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lbsgwxxr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3aanjtzja.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ukhzydwq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mzaioyye.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mafpxahu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lshqqbbf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zsimkhab.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dxxxigyy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lwcdjhak.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ykpgixhu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvfmhpiq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mcvtuksn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrixdwfd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wzpggpxh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eawlfcrw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfvlhklk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mnaqorqy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwdhdek.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cotmdbor.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3brupfije.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tpruzkyv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tauirwax.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fqigdger.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddyihubw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ijvinjyf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bpfbpljg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3saauiiyj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nvizkbud.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3alhvluda.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3neavpddq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gzrbccbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zfhdlfda.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ytezukma.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cqayadkn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vjvrqbyh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3subabcib.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3srsvlssq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xzuhwoya.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bfbrwjzw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqhpypjl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ullasppv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hammhwjj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwprvvoe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3iucolpph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3eouqjzoq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yussoqkd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ygnnaesi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqcdxlcl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vylrzcky.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owogxyid.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lsgrqvzh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hfqzbwni.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bszbgjwk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qmvmezlj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cgauekyc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vtirxgnu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yjmlntvu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hizpciyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oddzxkuc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hyaifcnz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wdgiohgs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3haguevwa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifrknpjn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vkrvfdrh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fimaccdz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvollc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dlsqjdms.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3giizdpgh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nauzwszh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tifzopfc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xzvrprwd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dgpbrjrc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3flolhbwp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kgghojgx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mgoccgxm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pswzamkt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kaemizag.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3khivfpmc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3oqrwhbqm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kukupykv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ukhksifq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjspqs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tsdsqcmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjxgdvsn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cvkrbvti.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bahragts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cmpldtvj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eisqsvqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eyxbbbao.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hkdtvwuk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gbtgwcng.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jxwrkgkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kprcxyxf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfjsjltb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nmcdgeun.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrqkhxhq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hcwehyza.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnhtkjgg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xdhelkkp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zafghpry.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3krbuefxs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ybqpsqcw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmvnvfmx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hnmhitwn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wdxokwvi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3krmnpdwu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjqpyxme.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjykriih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uelgquka.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ayeuoprq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ehtjuprv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3oteokhbk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tyfhlpwt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvugovhn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfbnydce.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jrqgwpqn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qstmaudo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3unhmmtem.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlbrzjw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kynazgqj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ekhgbbpj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3auhcuudy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3utsooown.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gmfztrft.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jqzcgtbr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zskwttni.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3olqexzrh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ctkygtak.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yfodvrmq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xcanowfl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kebjhfhy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3esywobqv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cjdfurhb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lupogrka.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xbofdvkj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wqgcvzaa.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yavsxlmb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ylqiyvry.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ppzjggni.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qgxbpphf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehkkoyin.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jgsdrvvf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3buycavrl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3canztmuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3thqkwfzx.html


<!-- 参考信息 -->