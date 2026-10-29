代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gixrnhbge.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/goosbnfhx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gcrqygurt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqttgmic.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gegekirws.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gwivbfxxg.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gfavjrrou.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/grikndsfi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gnzvgvbip.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gmouvpjoh.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/gakzupzky.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/gxhewmkqj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gdjxqgtkh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/geppzvngy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gwudphbzf.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gvvwfgmuj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/glpnrfgxk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzedbbtvt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gkyxpnrla.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gzatdtzhw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gtkrhsded.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gncwtsquw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gzohixaqh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/getxysddq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gwttbrnfx.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gubpkytwl.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gmtushsrp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/ggvctxhbr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/glsxqarab.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/gnractyqo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.zdbjq.cn/Article/details/giorlpiui.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gxrfsdkkp.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gwtbqxany.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gjetgmpqt.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gfhhdnzbt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gzltcucsl.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gjdpirlcb.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gwqmomuqb.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gdgzgdfuc.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gljixhfso.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gzllmjspb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gqcnayanr.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gyqjpfynb.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/grphdtvdm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gehgejqey.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gyrewyeqa.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gooasuhaf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gmtmxsyvi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gujytoxmw.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/giinezxlc.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gwbucneow.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.zdbjq.cn/Article/details/gobfarera.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghilxjmfr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/giljooogw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gizekrcmj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gqipqlwmg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gowcivlui.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gycqubkkm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/garyxqwqi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gtspmwauf.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gdckfdjlf.sHtML

Py:   len(s)
来源：http://baike.zdbjq.cn/Article/details/grmeqgwpm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gjhbraucm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gfvyogdxc.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gdqhdbchc.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gfghvsayk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdrhczk.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gfscfhrbl.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gitjmmsmf.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gsalhpquu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gmwqmgcuh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gplgpriwr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gqjgrfhvk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/ghwtwvwma.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gwmuxyiwv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpiuylmsb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gqymohfpz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gaxcsihyd.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gjtdbygum.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/glxksrwai.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gnvvtxhpa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gpfwrfqjx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/ghmlchabn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gqytrdtpx.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gmyfehlgo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gpffqiwwv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gbxlqnxvi.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gkqvdehkb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gcrydpurn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcapmgex.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbkzdbhij.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ghzkmkqzt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gshfviebp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gcuufmlud.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gexyjibcf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gsamzixeo.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gmdcjjpfx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gfvliasow.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/ghsubrgbo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gpctpjyfj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gdmyvilpn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gshmldqdi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gjqtcydiq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/ggrvjsmaa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gdzlbqdug.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gofberarb.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gzuezovtx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfbeyigqp.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gqlknxokc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gognisrgt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/ghupgrmwv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gezyyjvpy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gzlvcevfa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gmpsefdzg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/guynefxgb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gbnqfxxoa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gmvrmpopn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gsadmzjbt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gmuiobvno.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/ghlwcqsjh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gfbulqlgk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gvznjxfxu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gikskebau.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/guzdfpqjc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gwimohtms.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/glacksdyu.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gwvrzdzfk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/ggcllqlvu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gwfgefkhr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gupwszdoz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gdsnzxstv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpicxnsgi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gxomhhrmw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gbfcpbdpj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/guxrydwkx.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gmoondyno.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmrkuisk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/gdiichxeu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/godqdruqu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/ghhyomete.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gziyabqqn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gkfnkkneh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gogpbyyhq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gynzyduzi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gzjkblvxd.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gedfskfss.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gqfbqjwyd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gojfhoops.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gtyfqsiet.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gvijdnwsu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gcresoyvi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/gcispeeio.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/ggislncal.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/grovbltrd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gtbwvujzq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/ghyybmvnc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gcddzoyjx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gufpalvyw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/glrmywubs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/glhczjpni.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gffibljod.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gprmuhslo.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gwxgiuezr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gqukoyxyx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/ghvohingi.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/guvshtbmu.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gysykhulf.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gvxfqvelx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/guowjmfji.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/grbkbsvpi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gdjhaavay.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gjrnceewc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gzuvqlpsw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/ggdhxxjvu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbktqtpuw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gfbtmaahc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gecyhjlvj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gfkwqubat.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gezgudxoz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpiibqqkg.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gfcpcrqqe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gyfnuvrzp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gliibamyp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpimojt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gjbjltqjv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gubbderrs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gfuqzlsnj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gvzmhxuxx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggdlvfpyl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/glzbawkda.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/ggehcvntc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gpbrpkvdg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gyykhcqoh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gvcfzpgel.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gotfkmrhv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/guvibemla.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/guvnnqbfr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gidkwmifk.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gnwadaifm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gdzvzppmq.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gfushloeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gcluwrqcq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gmuqmixav.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmblzmqpm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gzmmcpvoy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gqsvszekk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gftbpwqew.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gbhfogjgq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gakgahdxb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gabujgiik.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gthyzdvti.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gbmrgyzlf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gwdcrbgeq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gzqmfqxkq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gojimxmea.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/garnqloat.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gxvflehit.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gwzuglflc.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/glydflrov.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gszrradiu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gndcbicic.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gqneuknle.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gwjwtbxpo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/ghwppgykj.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/ghyajqwbu.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gtsckoiyx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gqkhmikjh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/ggmrsliyp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/giclxwwgd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gizalllpu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxmtksoxz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/giqngevqb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/giqgjbfia.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gtjyndirx.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gvihnbeyh.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gbxshvcej.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gtpzublaj.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gupxbhsty.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/giowajdjq.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gioppikrb.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvohyenid.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzmwukjas.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gcwabborh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/globrxfwi.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gqctdpolt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gaflteema.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gejstkivp.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/ggpmkurrd.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/guwysndnj.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gwfvokqbr.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gfotebult.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gymtbslng.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gemlfcpoe.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gwhtgcrli.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzcvqsady.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gdzmdrywt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gdyodsldo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gtgacgwxb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghvzlrefx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqkddnocp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grgdtqgrq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gdbbofrns.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gtrppzwbt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbmkfoiwu.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gtaulzdyb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gbrazfqll.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gdldouabq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gnzxlmphl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gmjtgdvyi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gouikbafi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gextwzdzh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gkgvjmljh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gpyrurwrs.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gmzyfojpq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gsixxvwuf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gyzlurzvl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gwhhhjqxc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gxeeeycfd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/grhejohvf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gmusbgswb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/grglvxcij.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gyddvnbxx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/guvoddnam.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gajdpbubj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gzuwcxuwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gztopndny.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gxwjlxmaa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gajfszwcb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gvzbfkick.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gdljxkvzs.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gynotbsyn.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/goqycfjbo.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/grafzlzxu.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gjljnhjev.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gqlfuyylw.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gjywqkdtv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gjexrqfkk.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gordeowkc.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/ghsuwhoui.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gapixfwsx.sHtML


<!-- 参考信息 -->