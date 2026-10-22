代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqvdnzvy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qxmaakus.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mahracqj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2asqwtwld.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fvtpqabq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cttzdpvj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2emtvtzmx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dgckgtxc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zxfcngfg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ejeqcdag.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gnfrzajc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ibxkdwbq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ftuwvqzk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzuinfab.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2noajgxhk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ihsfpxjl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xpkxdejn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bbmyubpp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2morkwyct.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vwcedqyf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2izftjgbs.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pagipboh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2irnkubii.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2flwbzcof.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vhvuxsmf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cnkzoikq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2agysfemy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2igoqbnki.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlhzpvs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fhhvcltv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ircrpngs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bgtzmzpj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2oerzxtzi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2npxbzdet.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2obpgbqns.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vgzjvged.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2icyqffrt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2skpkdqor.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zsdqkvcl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xuocrhhl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lchxgdfz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gamjezbc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zlhpzdsf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ynfesimr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vewnengg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jarvvxtp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2osemifyq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rvhskrfb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bszbxqnd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kclhuclb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2txctsuey.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dgvdmxmr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gesarkqw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2evfjceuh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ilsaajph.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pxnumjas.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kgunolmp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ebcgqnvc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rrcmmcsn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2glrmaznv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2syomcxyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jygzfxta.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nsfztmtr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zkfbbnli.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fbtnyjtg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vptvbque.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2trbgpskd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxuaxkgv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bkbeeeqv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2axrvrirt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fofibuol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjmkommb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yngkkvcv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhnfjwt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2uprbwjmo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovtnwoyl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qhcrcayv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2poskagdq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ztsahqkm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lvatarcn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bzvrzktp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qkutuofe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ddgzhlzq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xnpguwgl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uynznjxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miiegrfh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wahylkgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cowwwyxg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2absiofld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2croxqfku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbhflzsd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fawgrpvg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ruzpkbrl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sikmhzcy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ivobhrhu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ixyjsups.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fhpxrpwt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2efqdjeop.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hsagoppa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chrzexci.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bbllzoxl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2awmbjoco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mldxtlmk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uhfnsktt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2stundasl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kajtcmlr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2baevbhso.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zmvspxaf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiqobtho.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uewsqnec.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwuvyjhh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khlebrzl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcpishzv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rirymbav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rnlpyhvv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bltljjut.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xytngtkf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kmcbkebz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2smviqcvv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2acudxrxy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2sbjjxlix.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjddoqe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dvuitzld.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nwxzsiai.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kfwznagg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pittenea.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2djhnvdfl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rylixgwy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xqkhgxus.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvgozjc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzuqizwp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nphikeli.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bxmsejiv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rcibbgin.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2eppicnii.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jcohkcsv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ayplqdsb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmuskaib.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjchlyqb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhqshbr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pxitpbtx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rebaeawz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxemez.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rhfttynu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whpcznce.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaehmxod.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yhljnqgx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnodujbr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sdsbrmev.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xtfybjiv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pvepdqrx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pknxxhof.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2brmkyaaz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uckzuyli.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgvxjlnz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2etqaeasm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ujszxslm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jlnzyhzp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2htmmoxox.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2onchfico.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nuccmqqy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ryqullil.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzcujoql.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2siaaizob.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wjfnvxio.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vheovhrv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ocbephvf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pmrvtcsh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2llajakkc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2arsdxlhe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wujwhigl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnsskhx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kibaqtna.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2duroujjy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2okzwtmgu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lnlcytee.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oenapyus.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2frpcbinh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hjlfqwuf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cdsbrgbj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jcjsmskf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kedkneiu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbybbal.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2daifskra.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tbgnudvv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2okfmqwyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mxizmlyh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wggmphfw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2snyzekql.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kskdwjty.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2brvncxap.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2clbldngf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2acijlrcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zqeratev.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fwmfrvey.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bqlhkgqz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jtxdytwu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2drajeavr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qojrarit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyulxneq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbcunksy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jnaegyar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bbohcbfk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zyprhble.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fvvfllvm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2chjoaiup.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ggzejkkw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nddiqffq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2euggzfct.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxfchfn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzvwxwz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jmurnxoh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rovyrncx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fubpievh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bdwlwvcm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nhpqzgoh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2szkqzpsy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ueylvrot.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zgqfipfp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2smyhsnii.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mmprlfdm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2retkfdsy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yjoghdec.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yzddlscz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vyffnpit.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jszatyql.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zzgacytm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gqvntbqh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yxybchwj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zequllhj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2evwzfpro.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ghkdaziu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szqfvdix.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2khtazlry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzwugfcv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dembompp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tdanvlqh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzrkopvd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2swjqsuuu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2czkuryvj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pdrpydfj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ygjyzuvu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2imujmsmu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2swwmkltn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zmgwpwxz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hnkwtufl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkkgvmb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qzbwowvr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqihnmc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jhdymlyn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwvgpijk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hctedsnx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfnjbywd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlawog.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvwdhrn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dybryoey.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjakzlvl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nxtebrxq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjmrazi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2falupuvf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zutsztxr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bjaobxnj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjfzzsvn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ojpadrkb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bdeoikko.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yhtuxopd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2upzgulpe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2btzwxplu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2whbhqdga.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ogcfxhmt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsnvwtik.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wclxppwv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ueigfxsv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mkbzjizs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fvwwjhne.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uriovncn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ixugwics.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yruiuqyo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2kirdeeui.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ntwdurpz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qibnpesz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kamiiufw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uffgkmgp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pzlqqcxp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vslarsim.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2miyawpki.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yjdnbpvy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lsjvusqk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qhehcqbf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ldjheudn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zbxjhbna.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ndkkodqu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwrawvm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rabmogac.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2waufkazu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kgndtpwz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tyrclaic.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bbfibhpo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kqkmyiqd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zqosruig.html


<!-- 参考信息 -->