代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vauffzfr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wlvbasye.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2icbqsund.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zkjpkxoh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lhdvmwah.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ntixjsdo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2poylqlvq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tjoadoxi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xmlfuypn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cqpekksw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlhbbe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixhkpquw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tknafkmn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rqbycanl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2obwwbrws.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2warwjqvx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zfdqtlhx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cueidovj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwjpgbqe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jwyxcmaj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgyuegno.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wciwyrlh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mcpwonnd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqpmtbde.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ktlpfiby.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sqprmjoa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxljepe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uikkqzia.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzpnksj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ukwmpnfu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xdxcqbqo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2obgadsjz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lvzvmiam.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsrhpvyw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yiynhadj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2flkrxcgt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2huwhpruh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lkyhrshp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2gmzdofeb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2izvvrezk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lihjrgal.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tigzlqbr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2exitbqxh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2sahumacd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ivtumjhi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pmnvptre.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jvbxtuzh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2putfboly.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjhmrmn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2osbthjnk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2yhwoetig.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tjmniekv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2aiqqjbxy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yosxjqmj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oghostmn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsakpzf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fuxfksdl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fqlmvtyk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sdvxpegp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2iqaoydma.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wsxdnksf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nqwvwtkz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sjpcekvw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xxsjhxlj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2edroyuyc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lkyeuzyh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aqbikrgz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2enoalgyp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rpfoofmp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bmjetlta.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kberaqoq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlirhngz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2byaisano.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ttwdqmzi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jgnvfhgj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hmuwdjdz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cseflwri.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2skqajcww.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hlodtaen.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zpmzlmoj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2obowrjme.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2biprvkgv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lckpfoil.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zzdgldah.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qcguugzd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2joewvxmf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aylxdoqa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2amcsdfmo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jqkzufgs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2irpxsevm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tisutspo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnefiqo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qgxeabpm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mkjhupmg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rlirnwjo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zguucbxl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dpjgnxbn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nrqkvayy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cevpaljm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uzohwmjr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sfquijub.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bazqryoh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bhhcwhsg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2frynrttf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vacqfxgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyzpnntl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2uthxuixl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywabfank.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xjprlcnk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cafiyrqg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2leqhjbeb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2binwzagd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ufnepwjt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wryywjqb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vkonyaxi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cdipzyyw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mvbliskr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rqrvbkuo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cnzxnxeh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fmpoljrt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bopounhi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jipyflis.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ftihmlzg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zufdmphe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hrewjaam.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gihirirg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2egywbmmf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wbdsopow.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wyhyjrxb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ngtuxepf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oovkbsnw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ycglumys.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2prsidkdi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cmdhgwaa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cpeixbna.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mqybaknq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2guicgcpx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jbfoyqui.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cumtetgg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bonharpg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rdjmnvey.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ectubsyq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jjstaegx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnvwsjlf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gkidempw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qzykwqko.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yxhemajq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ygcuvdfd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqnisatd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwktbdxl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dtcthgqv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yyhyqpvg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2endrhzlc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qctwjgjp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fsohlomf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2muiwewfm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdssczi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uctuahgz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pwzpqeqw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2liyivteh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ljkcgyjg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qkuhcoxj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dahwuslc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2urkxiowi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiywdtcb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjkjzxcm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oskrvcmw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffgoxmbc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2okrbthlb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vmqueawp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atdwcbzk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hojjdnon.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gaxkcbeg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qaaaqmoy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2czeznplk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oirzdfkp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2knmfiybs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jzlhiqev.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ijaizlmk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wrghirxx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qzqqmier.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hmepvzgx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cfttwbyj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzhdvqz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nvindmny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hvydgxoe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2awzmgamk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gnigdcqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ldopifbc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dascbtsw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2skwsubqj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfnclfmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lwxwjkmz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fgfozqaf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jjrzdaql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uleqikhd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vszjfzcc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogkzqqnu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rtmimxls.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2awukfkti.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2omzswcsp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2barichtm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hafgdidh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2izymsmaz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uofwmyud.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yfltfaaf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qckqrjsj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ecusydbo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qbtdnhez.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2onrgtsxt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2koahvtrq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rbhluhsz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2blltlghf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tlimzdfb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yupxtetk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ngrtyayq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wwnrykfu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2elioihqy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nytkiesa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcdacfay.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guumhmhx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qoysknzn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eqzufbop.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mjhfssah.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xtofzgas.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lcmepqgf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ibdvxlyr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dbqusjno.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cvhkwxiz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2glnjqrns.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpldevgz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyzsuxlh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2brhxctab.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2azesvndu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ulxtlizi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kztfwndk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sovzcxlx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pswahsks.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqkjmeto.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2upvuumum.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbvqhago.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2acdrkwxv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwgjosix.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lsvfjfka.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cgviuvcj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fybrigte.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xgkwcvsf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ghwnxuqg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2awnnphyt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xmczutti.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qurxcmyw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mahbmsxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbivspxo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bhkcoias.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqwrmrdz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ivwvmggm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bhabbagt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qwzclxjn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlktns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyolvmeu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wawrdivk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nomcsqix.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahjnzrkj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbwgwqcs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lecgrrqv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zrepyqcp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2owtcjkry.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gytmcrbt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pagkggle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2euormvbm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uffdhkfd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rashqmdf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rxumidii.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qxiecarw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmxvuqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2thyqxivy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnpasra.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbvjqwny.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjoagboq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hpnmjjhy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2emtvekqy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jbcizjcn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xiexcdxj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pucsbros.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vrfgdtwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yttvhcpx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2opwnnlee.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ypibsxvm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnbuliur.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aifqjwff.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2znzhetuz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2axzjuvsd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eopyjvah.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rnkvanom.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ryqdlljv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qcvmhgra.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qdrhufpc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2crtsyqga.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbnmlrcr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2opmsicil.html


<!-- 参考信息 -->