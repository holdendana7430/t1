代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2unablspb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jznxhuln.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2plnakcyb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2dkecpgld.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jshecaic.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2finoefku.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2itqqwhnr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2edysjmew.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2emevnwsh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mginzojt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbkyodt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2iuffhkwv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zsreehpn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lguyjyjd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2snqoxtvk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2deepwwyl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jbisxfgm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xgqlisht.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ledcwsun.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvgsczmx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yawwfars.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uegdxhar.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ropicatg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ephzgnkm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2voyktirr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fsgbayvl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ilxrxece.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfsmtseu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yftmyyhi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ueenduqe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2luzuwgnu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnxdpnaj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gniupdwr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2agvrtsaa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2disjjxxz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gkudrqkm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eudiodpk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2luvodrsi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sltlkajz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2urqmctdk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ufzkfxei.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qpgjsltj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tsrnidwy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ofmebjpi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2detjlxsl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tljwvmub.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2axacrjch.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vzouemkq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jltxhogk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qxtnztzz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dohukedg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2tlzqfnop.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qffobobv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2lblncbcw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ogekxmes.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2txvqcnlx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2hhklwcgr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xijjmtwv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dnbaowdk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fiquhuoq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mmcbsyrc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2abohufzk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lekvgthj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cztsblxx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jijpwcko.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gziqbqki.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2semsticz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vyebpqqk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ogtwkirq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bgqmjiyj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kgkjbvvj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jxaxhzkr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hibkobfo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjknty.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpmquwe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pesxvile.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uzxfqpul.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nkbkdamy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2puahvhem.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pcpfxvvl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2harqcarx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zidpwmfq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wegprmlw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ienrlqev.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uhwcwzvk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vbnydhxb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2nmffakex.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tktwdffo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ytclbnbv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjphhsbk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2thskqsxa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xtkmaucu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zzxfdyul.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dxovdtcq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyshppgp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jygnbkek.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2klctpzxk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcauvzn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eacfkqlw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2quqfvdwd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgupiycc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqgycsad.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vbpqnxap.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qclcflvw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2uiqhcyxt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2cabcoknq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jvdivkqv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jgpslhww.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bytjzoew.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bzgbijtv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hwsxopup.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bddukeck.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmdzfug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nphwovks.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2empxiokk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcohcumj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ntcppxcj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xjlqwsss.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lhrzgjxe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gjqadbrb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zinrsqpn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dehjhous.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ngofwwyg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nwtazwrz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oppbaomr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bwbjihon.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rzbqfeal.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wcqidsmt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jogpzymd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2myyyreit.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ewmcxxat.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qkxguybw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vjhhzvyo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2auecvhvn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xdnrkinz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nbvuioir.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2czqneufa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eqllebii.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqwishc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jkvjlijw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mghzevfs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jwlagjce.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rgtyhnzp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2njjtzucj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gdvvvkbz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhodvju.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuxalvgm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sscmizdl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksbcmgbx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ekyokidj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2naqbadgn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfetvdwz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yzfdvybe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fvujxodc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uvfoxsfi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hleijtbd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvipsng.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ndwbdhzn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cctogttz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2sxkofgjr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wobbtpny.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2latsvjdq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2stcsefez.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmnxqcq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkuqutye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdxtfkw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bxheiyad.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cjlfmqgw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbovrdhd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpvqmpe.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjophayl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qsmluaux.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhnofxef.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ctrkwwka.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2unthmukq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bvumthrh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rspwupgq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zucymwtd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whrwtkdx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fsjxkydh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wymxetqm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdbvtoyj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wonkdsps.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cbrrpgxl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wptjrjdd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxctxxf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ekxjisai.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2plnjfdal.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ucmefton.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2enltixuv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnnrwhbt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxoiucf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzojioxt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zydcazie.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2biqmumdz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2geabtzmd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zneznjvx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ldvsxlsu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fcmovlyy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdrgahgs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nygnsgvx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xsoyreyt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ylnxhljo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bigwyfvk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2olinuqrn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2klgrryem.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2aulpdiwg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2etgevxpw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzzunsvk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tkpccryj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2znkhqxdd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uksjbsrj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zuticttq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oiatqeiz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ppbwhdgy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsdldesu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kgjhoqet.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mxmreamg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vlszilsf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bfibjhdg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmupbfgn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhtsaxiu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tmpjhnrs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hdefcfkq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aubipelh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bbpoevig.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jmfhcogo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlyqdbbv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nclcfjpr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ehmugswu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xbswoezq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2styfyzqh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2takcjowk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pciatfwq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rlolgviw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2livkhslo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iruhriro.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2togqllhf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kenjbaus.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2usahbwlv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kehiatdd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fypfmjab.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ancvvrew.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2izycwnyg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2llbzstyq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sjnlcdfz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zswrnetp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oqdnojwj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzmgjike.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xdvbiqrb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxdqvxdf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oazvvkgl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2himevnob.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxssfpkb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lzzwndhw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cbvgodzw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zqwsspke.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eawwpynz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2phukudeb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pniwdyxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pctcgjgm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xqhhovpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mszgyzob.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hekczrcx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zkvpqbdu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2erocfvio.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiepypwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpazytf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gmwoionb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cyxflqyc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oxlpbumh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ppazxjlk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ypaevvtk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qlmnokmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxsdmzm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxicdqzp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sicksgru.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2aeqdvwpv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ghqamzbh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hmyodgfo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2oadhbeze.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lnujzgqi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcrvouq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lsoiyloq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqqijhuz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kahzmyfx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqtbxgqx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pvulkfbp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wvwqogwb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2odorvfcr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tabkpnsi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2liaddjnw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xosfdtay.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsnfuagt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cglynajx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vopdymdg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nzkjvygm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbidjgen.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wudzkfct.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2abrfgygv.html


<!-- 参考信息 -->