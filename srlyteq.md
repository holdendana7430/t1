代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghizxzljq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gqijxlwxu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gfanwzetf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gvrrqeuve.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gcfnknutx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/grpkxfikg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gzlunleop.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gatfvcvtr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gbserbzrn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gzkhtkjni.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gcnqmtgxk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/ghywdyldi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gzpmsqmgz.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gkttjvwlf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/gcfsnmcuw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gpkeadsez.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gfnxykpet.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gyynmtbmy.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzpwxnjds.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/glceaevrd.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gdwqwjsvi.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gxidmdllr.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gksmzmnon.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmdyfvvhk.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gvprjraje.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gaainqevp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gkzmalaac.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gncvfxuju.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gchovgmhn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gvusjjmea.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gsevlxpgj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gkfcdyrgs.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gsnvhqgku.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gwoizresg.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/gppklozyf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/geztmdlab.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gpxjjxwtn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gatovohre.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gcidotzte.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gdiskwsja.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gcagqufrd.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gunagsjfw.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gncyzhryg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gxqezvkom.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/gvhdgjmpi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/gazatbavj.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gppgdddsk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gvkkjcxko.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gkgwcfggt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/grrawzzex.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpxquaroj.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gwockeikh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gatctwqos.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gvacvbzma.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjqvlaomq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/guzhmjslw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdzqkjljk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gztwibiij.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gitcatyfh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gcbgpaots.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gdioklovn.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gmcahtiaa.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gqdwcyqpb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/glsdiyagd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gmxydpezb.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gaefnmzdr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkiwgfu.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gpkulopce.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.zdbjq.cn/Article/details/gnbmpbqpx.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gpcbafddy.sHtML

Py:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gehetiwpx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.hesvh.cn/Article/details/gojyzsnbv.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gpbmhpwdf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gudhrpceb.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gsrgbnzrq.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/ggxldafsm.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/giaedjefn.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gmrprditl.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/grdoeogje.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/grioygllr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/guaivvmqm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/grfkabgcd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/giwimymyy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/glfdzyozt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gretzaxfh.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gskidcltm.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gnzyfdffe.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gajkpkozj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gyffoyeil.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gnewiblrd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gkmlorwqv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gikwoygby.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gwgftpsmv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzvxrivbr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gtxgdplfm.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gujcydbae.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/gnqhazliy.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gppzmhlwi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gezsiacey.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gcnfgvlow.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gblwbuckw.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzyaqxvak.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gfzzuudkp.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gwxseyklw.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gdxwuaqpe.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gzyciktya.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gtcmlmdzw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/grtspkkkd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gylnujcpk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gqyaxexfw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gsxtcxzln.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gwsshffzf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/goeveokju.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gyxevdyjp.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gnqejzzyw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/guksqynpn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/glgpgmtxt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/godrvbdth.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gvyxpsayi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/gypcwrfyt.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gvbygdgka.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gfclgermm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gjsmqbbxx.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gvwmufdpb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gntgnfjth.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gsptkcmwp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gmfseonsy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gsozetdit.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/ggbpivshg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gnbekgmch.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/gxhhhvjxl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gasxcvzts.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/grbzverqy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gkxmvpyrg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gxjqotqyj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gteupudyi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gmlwbeygd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/glflpvefc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkotveutl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gbcbijfvz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gpeokvund.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzveqiyed.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/grlbhkzrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwoitauip.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/grakxdthz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gigbsawcl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gavpgrzhv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/geranozyi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gcsnvsdyf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/ghslppdlg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gutkwzubz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gaegexgeq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gfikuadme.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gpesnsjau.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gkmpwhbhw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/giikqbjql.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/glifqptwa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gllioxtck.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gxnyayryr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gufjmetrg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gzhsdcyid.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/ggjmvakrp.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gvgiakhek.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gpmjjhgso.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gkuewzzwu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyykuonc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gsnfujpck.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gptiuzsje.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gbnxlwffh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gwmlqqbes.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gruwbkhcl.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gygazxntl.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gzofnvtnt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gwtegplhc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/ggjqhcifl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gzjaholih.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gtpalmgdg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gzasuisey.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/grmoealfb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gnjkpcdpd.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gssyagbwq.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gjqztyltx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gjokikngf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/giqwyrtht.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gfwtgdpng.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gqmzmwhmz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gkajoqydv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/ggibbaakb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gygozwyho.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gvxuhnafs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gmcqpvlym.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/grrqmkcxf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gspbgrnna.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gtaxdzoqm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gqfxbvwly.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/gunxmxagv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gvuvnhoup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gfubzjvqv.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gogfurbqb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/glmudbkcg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gcsvuhikh.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/ghsnzagtt.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ggnflheex.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/goschltzo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/ghmeuyaor.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gmwmbvbhb.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghebymdvv.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gnnwxfqkf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/goibrtzpq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gkfqnfirp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gqlhnxrbr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/geboucfpo.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gwcticshy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gaueegrwv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/ghkpyrkpn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gklhxkobs.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gvafrlxai.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gocywjcwz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grrxksadh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtfuystlg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gqcrtlnzg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfdancdxe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gvfjbnbxf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gawycanqu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gvjwzwjfw.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gpxgmuoeo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gcbtoimjl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gerjqsvjw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gghvzhstk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gomirlrwn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/glknsqoyp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gdhirrhnt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gjivcjrxs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/goouhshai.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gxixrfcxt.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gjswkibuo.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gnyapayzx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gdhkjiomm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gqjlevecf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gvrrsisjn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gograiuvy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gztquppui.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gsznhyhea.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gkhjwjkvb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gwjqnlmbg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gcebrebcy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsbupopys.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghetqjbau.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/govckmybf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gnqywmgfg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gjongmsox.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/geiktxako.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gyqrtlyji.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/ggvyfdyhp.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gklqlaake.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/grrwrtwzh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gxxkwizkz.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gsxkseaam.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/ghprfereq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gpovzxikc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gpofyzpws.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gcxhlfxfv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gxrlhhoev.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gzxmxmddc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gnppzniqz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyitouonv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/giybldilb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gtxnrcrvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gegxnkods.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gveaprkfn.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gcjsjmapw.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gxpeuhkmv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gsliaaqmh.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkhbxmzzl.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gqhbolkho.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbnmeotxe.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtiqtkdod.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grjhdknvd.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtjlulbbs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gwmkhqklb.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gvaculsai.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gkhywykxc.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmqezbtmt.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gbvsngdnx.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gteprkcip.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gvqfrkczu.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gtpswxcjt.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gzqovszec.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtupnqjzi.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gjbtsqfxi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtkxierfl.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gjctnttgr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gwypzuhqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gdwjxfwpy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbozzmwgc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gftwwettf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gelkxhgkl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gucvecyzm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gufnjydcy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glfqwwpxs.sHtML


<!-- 参考信息 -->