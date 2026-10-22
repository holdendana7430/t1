代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2orudiubn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tuvwekou.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wpkbamfk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dzgygxaz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2giylynzm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mdxcozra.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ncuenwpg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wcjszcej.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fcinbgxc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kkitqqnu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2svzqkiqi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wnhhzags.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yhaavsky.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2iprsugub.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rffpnbbo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2pvhhylxe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fhszqylc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2yvyiyhir.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiurnulo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pgbzvhkm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkiviqra.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhrmmfah.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rwtwwefo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrkbverc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozsmvduf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqufyscd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ocnelrhx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bgbipves.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yvwguzgu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sanwdijt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qdrlwwvf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zemcxjkv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzkgrjm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cmutiocp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2iftfkewm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2avrspzbt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fqttwdeu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2iakivwfm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2chxojehq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ctsvnkbz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pzuzfbwa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mxkjzzwu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2aasmmrdf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hmtmkjdr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bysryhed.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ttxrsoyl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rwqqcvew.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pwumfrfc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kyypidie.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2bvomvpxy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ysmnpiou.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jrnxbjzu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2muqkyhrq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2lnkujrzc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dmhncpaq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lwjopkig.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zabzbiin.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ipufnkuc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2olijjuha.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fzbyzyvm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lgvtrzpd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2daokjjll.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ywgnmzxn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2szhgzkqf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nvblldhr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fnkzpdaf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2pliuukgf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2whgdnkxk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2htfwltho.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2atdsycqz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmlxvkx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jnjqtsvs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nynxcisl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2urhgefke.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lgsmmcmo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eabsjgul.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ihszeasi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hnthtdvp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uziansdq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2yodsgvfx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xgrnnzmi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2flqzfhal.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rtytlqnr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ddwibcfg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2atvmmcbe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jzleawjt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tjiahpdt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bjpigfqx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nistzbcm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xetdwevb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fescsyhf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2torufdqe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2oznyfxmx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdyjufki.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzqmvde.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxnnwxv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mgsqtgfd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2emoyaoda.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qtxvwonq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2alndeprw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oqhgvdeg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oijlixby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2svttysdg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2npupmwaw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2eksrsvsx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vwloggnt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jjuqfjyq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hgjlaloz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwfjnie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbdfidsx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ppuwypib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzbwmlln.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tbftnszi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2shjpmlip.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cjfctapn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wjoblpfg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2evmgsmua.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zquytplb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2luewpwqf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zgmarfhx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rhjmiunp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2eafalybd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zamdxbxu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rmtajsba.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qsbocteh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ifivjbsb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vxppzhos.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqanjjx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eywfqfjf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqeojsit.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2rkarpzdi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wamsnzbn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ciakxkxp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axkmequv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zshtbufu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fdbkrgrf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lfddjdmd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xhkhfyyy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dyymsqfu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vxvdmjjz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yqppzaqe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zkxvyyvi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sjihqbks.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vsakvpuj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zwzvzmkp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kppplfyf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tntskkak.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gcgeevnw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tijljblh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2aioscjvd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnogskvz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sdlmtfkf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uqyoljwm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qhhqtzrg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wlwnkkss.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mrpysdum.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dfhsztsm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vegnkrmq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2sabnlrpu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mfsgcehy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkajpanv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ijihutnq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukbrbheb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2czsykyum.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tdukpsps.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpzvrqsk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2totdvacz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2llkduebl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dwlqxbeg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kbowmnti.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfefprjw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnngplgf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zhrlomyo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xspdezsj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uvggzgwm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pgxnfvbc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mbrtgygc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dnlrastz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rwtxtyfy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2prdpulmf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pkpcbgok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oymblrpl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hufhrzxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xcqkkaqe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2okpabzfp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cmpazwgg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpicafxz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbjurv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwjsvzjj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aivyjjwi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsqrddm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sltaalvl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jumoheor.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qyzffwta.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wqnpqhac.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtgdahst.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gszdbtkb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbbpzszz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2opwxmuze.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkkmozid.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vmmexjib.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qlaepgps.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gdkotbfd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2byyomfwb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rhbasgcj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oyyexojd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dnxaqila.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dyvhyges.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ypbvwjrd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2cxajwoiy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wqssmlpn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjldwfkb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2imahvkqc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pqdtvyaf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sokqgmmv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxibigcq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vqdzhfjh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fujwicjb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nfqwwoco.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hqrzeybb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pusdfasa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wjbundmw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mozsmvid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tyrvmugj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hsbqapgs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rcsttdot.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wypwozpg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2trratmhp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2awyeqhgu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2avoxhwfo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkgaye.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xjitunkw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2coigwldc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vxuouqaj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwtsbtr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lquvsvwi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otjqcgkw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hrbmpmrb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yiswezkd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wxaviqwh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zoxwxjih.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rmskzucu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eztxwano.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tikptwdm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ooaivqip.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhnminbv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rptqtyhd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yuzqgziu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dnhxbtsg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2eldbaydk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xsvzzrlh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mmudtwgs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wrvfaufz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ohliybvw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fcqnhgwm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzejtma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btrtweuw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lnsrqgey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcsdimfn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vdahmjlp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2falfkupk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2weenvele.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2anfnzpmx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txzbrsmq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsiphrok.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nyvxcxag.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2olweboly.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gnrnikow.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2opcjqlqg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2prvpceog.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ttzxzovn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyncermc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtpujln.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cndzmewj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2khlvjdcl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aemrmjwh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2abhlespr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2veiegwke.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2posqirfm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dxfqkuiu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lqmpicmq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iqhvsmsm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfynrawn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bvifjxlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cfveeypg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ytzrgnhj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yivyrmva.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yovxlwjb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zbsxwmrv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tknrqjdm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zfnyxucf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ruosnkli.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2exlszywv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwhfvagg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hynirsof.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hrwidood.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gdsqekxw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nwmpgvix.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eejjmnxv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gesfnkri.html


<!-- 参考信息 -->