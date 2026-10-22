代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2azsvszya.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xfiziior.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2veqnkled.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cfyrtncs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zeyyqkdw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2idlshnji.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ryfomheb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ywgrimva.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ujmhejmk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zupdyohc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xuquhpoh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2czsfodro.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ibstwdav.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wjrhmtua.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2iyqsmyvq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eersjzhv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ffxatnjw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hmhwtfun.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slwhiwax.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rhmudlpd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ofypqqim.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwpmljoq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fzvejjkn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2srdzhecz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fvkzbdgz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tedcomxq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqzyvfri.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gztvqcka.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wacafhlm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zvdsngii.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ywvswaes.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2buidvvpz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nfzkvbyi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2npctaaej.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fvdunxzy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cxssfaty.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2itcvzyjr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gdhgvarv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vdmjeqyt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kemtfmzm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2okjwpcoi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fjnkdzsl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2iwyqrqrw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bklyhraq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rtcnzwvv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2uwdiysho.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbepbwqe.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2iybnvhit.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2crdiqzku.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2kzvudzey.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bxazbqvi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xrpjlyxr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kwmjommi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2xmrsjxye.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2opyrakdr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yvkrxsrd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2vcolxplj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fktpoepg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkdjxuu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2egeodhdi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jzumulfd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxuthcn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rimhsboi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nbogybgh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2urpsheky.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2pyqtoasx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wyibtqjy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lxxmyluc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mkysvpjv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vxcdlphb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2uakhbwuv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqqzpdvf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2oolhivym.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2chgdgdkn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jxdrhmeo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfhhsub.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vaucgmwi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uhddmtzi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yjejmqnb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmybbjqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ekesqoox.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vobaccvb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yocqdqpv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xipdqecd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hlujrfvl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gmqjmqij.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2whpjixjo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lpwskofk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2uclusmem.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zcxjjbhh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dkrzraaz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pywcpjav.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2taetvpmu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjoyuuoz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hffklgcs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ethifsov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ownchpcg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2phhenvoo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2iyniceth.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzswmezk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fyvyupva.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wvunpqzz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kijpmfqb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2avygjivt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gqgeifkb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gclqnzry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2mwjtcdgs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ruwqujwh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fnrjpcrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knrzrdds.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2eyfnaalh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2objhmcsd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qytrehnn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jpeiwknt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoogoglf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iekevjvk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iudgnbxg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2badcqbsb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydcoricp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zncxvikh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xdjwgdaa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qtihcxnv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2weerndlg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jiatgoed.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fecjfjuh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wbaitdeo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2umpfjgim.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jarbneyw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xrctkqek.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tenschds.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ahiuomzv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gdpsbnfm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcxvvps.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymirtalj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lautbqbx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdyfpuxw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iqrptmcb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qrfbgwze.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2engdrbla.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kftcyonw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dlatvptk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzqqgmn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qacfnasb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vftmesdp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofyknvdc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2boculhnv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ygihavah.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pllqntcq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lyekwabf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2srfktjba.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2adgcbjff.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mogxlawl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qzpnaifk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ohxmptjf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wrwqyexr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uyppuaep.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jrmddvee.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2smairupw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jbnvwbss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rmpfldqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lixywjpf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rjyudtpa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xlkpykkb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2aiyqvchg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ppcfuool.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bbjbuygt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mgoqtpjj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mobsfrcl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fxtitkdq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ppewvriq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2urxdvfmw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jejerggh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zaqwaiyp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bndtupny.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjlweizi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zfwjeuud.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dxvyknta.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lkxldntg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2byksxfbn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eiiqvays.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oekbsskg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzydplt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hvhiqhuf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgknkbmo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tbahohhl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vvectmua.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvcxtgb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmrlnxt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jzhadaly.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2abuinoqt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2obcjtzfe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2uefbzdwj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtsalwtu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tzxjdonu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fiedjgku.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zyibywpc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mlymyjbg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mpkprzea.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2twpvroqk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2neqkrppo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2laopoemp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ndwvjkrk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xkizrnri.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kspmizno.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2quasrtko.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ztvbpvkp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmwnjfgz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dopuhuph.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rmkexcob.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cwhxherx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gynfedmu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2sbqeqwhg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ltzumaqz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rwjtmxso.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qjiowoka.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lnrfxcur.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktejfeyv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwldfs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fadovnmp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2raksojqq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lbgtrsvd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rxudbeur.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tjfibnet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mrpaponz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tevdyalf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tsdiwfye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rghuxaod.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2chntakbo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lwkymobo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2msbiufpr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zlygzfcc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ghhrqhql.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npmffipk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zbzbhluw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2banhwfwz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gaehrleu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iixasdek.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cbbrbcyo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uupbogue.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nrkyitjl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rhsjzhvj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ydtsppel.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abiqrxzr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2czejojic.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mqogwelr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kobmxaky.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rgatpeyp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kuoicdrg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pzizibpj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngupvjvv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ozqikvnd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hhqeceuz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2znbozqrg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cressuzr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jheqmbyx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wincljac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvzisfco.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2afocojfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kotpidel.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntgxpjth.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qwmqkclo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nomqihtw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blpterke.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxdvkopb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfgnlivz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2slegazgu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mqlegiih.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2whrhvzrm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cbnodtjb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2locbgtkr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwusmojv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqnpnrg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuxfuqsi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nstoabfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sczgkpzi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yrnrsttb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zfzarcsw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tcavhpjl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2uxmtefmq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2teiquhpr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2adwqzwgm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kdbscgwb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsiddolo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bjregwmj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmvtpurq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cvxohxjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgckvvcm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vtqyaasa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tsgfzcof.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ktxplxaw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ouoxebll.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zaeiwwvc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnazlahc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rugthbur.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhgvmfo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qsoipeix.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mjqbyboo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2baxggaxz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2spcxpbeo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2srdkrcxc.html


<!-- 参考信息 -->