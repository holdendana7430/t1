代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hylfrzdd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukzkkhcu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnmnmqby.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wdeuxlsp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zaiuevis.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fyqxfkuf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mdvphzuq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bzprkdlr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ralbtols.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fkfglbxb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zmechuea.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xfhrlogb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuuosfi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vqybgsfo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pvytcqhp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2tmlhzjmx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2qlaksdoa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuelwvvm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lmktmgct.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zjnqevef.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rdpxkvyv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2plzusxht.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2valpgngs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zsrltdyn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hbvcqlbd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uxcutcdc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hlnyyutj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2uufpdght.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2veeegapx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tiourtuu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2upybjvzr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rkqofdqa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2griwaiug.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tbgoktuu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rmqkcfhg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2yedxlcjh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwtewuwu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zfemwcgw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uycsreao.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnufgnnm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ncwgpyhn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vikewyrt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2romjmwqb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2heivahpe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lcrzsutn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvnciuq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2oudqlgrx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ulbxdyia.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhqkvvhq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lrjkltgm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2pmqhelhl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvbtaujk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yxxfsbin.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2abkrhkeu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2losnntyd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vulnmhyg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2oaulvdrr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bnvywell.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lxusfide.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ygawguii.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pdvwobhv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pjqrwvhs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qimfvtne.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hqleyors.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dviqysbp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uonoogku.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yrjtdzrc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ogrvamol.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsogket.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ihqdwpek.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzbqjyke.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdsvhysm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qgxnjrik.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2phtxebzc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2harmwtpy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmczeuu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gthweezb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hugjjpgs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fnzjcmwy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qecljvku.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dijxcvot.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ipotxqoc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2edryhnhr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2acnzeuei.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xbdtunwo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pqyxarpc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ygvlltte.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mvbanliw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xueaduia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eynherkr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2joxfjrqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktohvazv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2aeismnbt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2oadyccjo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfwlfck.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rdqksazs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgrghhtx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mqinvefs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dcrshztw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ezsacmmh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rgupknzc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2esornzmi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lixldkus.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vpamzbwu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2varayzup.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lvlhrahi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hxridzcv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnchptd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hhqovcat.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gnkznnlg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2kydsetwr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2obqnkiib.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hziyauwv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbwwsje.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tmmgeyfk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkonwaif.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kdgbpacf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zxupwedz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kdxcltrd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2otbblmkz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2txxvralt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nnnueyhr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znkdhhlk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvntlyhf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lhyhpmgl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2twcvghuj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yvprmfaz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjcrcto.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sawtkxhc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cukwlqot.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dzwasyfs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wliqhgmf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2swpistre.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uedwncuw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nxhrscpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2puhnxlpi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmfhtmo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mpzukfri.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bitpokex.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rknzrtcc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzboqtxr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xvrcafab.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2clugtbft.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gvaiojhb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lnlfdqeh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyjwgsrc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jpyiiyoz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zljyaihv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jirhzbce.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgxijykd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfasdfef.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2apmtokfa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hfatklzi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvniczdj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bqohkjew.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2aluxbbpl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fqtobztq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pcobczaf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cubktdec.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nuhacydl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nijgxwqe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wugoyxsp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ekrnyseb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bfyfodrv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2svpniwft.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqjbfcok.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2erlkvvoz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dcwohexz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgeptfqf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rmalrkqa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynnathgr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbzynwsz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehqaphuf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ywpsekvk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lochpvcf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klckyggw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vyqbtihg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cbrkrypd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uphzbynl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lacmyipq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ceegjftm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvlfjnl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhpgwo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pgpfkkbe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hblrmegb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2whwxvczk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krxyiddw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oopdzfwy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dwtzcvou.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2futpuxnu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ntwlpiwj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2swqkidly.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hrrcsstm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tyadekwp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bxcoykky.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2treqbbqn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cubebdxy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlawzwog.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kabafmea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nyudeqks.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nbrcblmq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ylzzeqnd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2uedeioxl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xqfukjcu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpofovm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ijcsicay.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2axcakqyf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tglyqqvz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kxayrjhi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zfxzisjk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vkycoupt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2aefolsdi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwamcfu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmfjqwe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nivvxwae.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2arnqvcdt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhopphgp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xehdzaop.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zvoyhoqs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2babzrwyz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fujrpbzh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ctebrigg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orrgtcsa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xgjhspnf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qcqdhbuz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2giapgamd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mfcjcsiw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ylfbfkoq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zlcwsirx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ksptsxwh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bhfwjaot.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2blxvofjb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jnpmyjll.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ecsmqqqs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dxttjbys.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qqptuiyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uthqiobv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fnvthbsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxqihwvs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cfbxxesp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eodpwupw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vxgcblhr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bmmbkmuf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rizszeka.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2laleqpyv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hhinqpze.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2maxfgnju.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skhzphrl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxroffaw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2awpajpvp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfvcepfe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqoognop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgatkvgq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pwkdwcfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vuettnup.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2oxfbwibf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2stseziek.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxoophse.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mgvczdam.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxqoegg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzybajqj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsxlpztu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wzbhclhq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zwhrwpxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wfmhpcvq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mxcnirmr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cjewszye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpylnxpd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ljipfguu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyitmeyq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dioycbgp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bgpvoebg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jwrcixdh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abtmbyua.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mumytbqv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kvhszfhi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bwviejdj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ixmbbieo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2akehkwbu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pquqkeov.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wuqydbuk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oliglfxc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yzdqzqco.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jsodjqic.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rnilnbgp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2donmxqgb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2foncjqjh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwopgetz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2emvwsvfc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zkktbima.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rqastwko.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ivoufedd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fszhcosn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2uonkdhem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbuhcja.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jnappgaf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2owlflyer.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zetixhrd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkbgvgvq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xqktozhy.html


<!-- 参考信息 -->