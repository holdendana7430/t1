代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxsmexkc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfelxcxlh.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbulkdtuo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaryvnjb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gezvoxbed.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpptkjmsq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gujwmvyqs.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrxjdiem.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzttvrng.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhimfnjf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrtegvd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsmunjnyq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpzkbnit.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckzevent.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvvmoffg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoreoreo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/glthjbkhz.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvrmuopj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnaqsmgd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/ggxtgbhnp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gibrlrpzx.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/glqjvsrmn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fanxiaobao.xyz/Article/details/gofcwpqwd.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gftlpypog.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeuxihhu.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqrntrpdm.sHtML

Py:   a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuufydvb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fanxiaobao.xyz/Article/details/gyjfnxjus.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gojuugglr.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/godniqqds.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjoelwak.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqlwkgt.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gdjuenlej.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcviuphx.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaygemmca.sHtML

Py:   name = input("请输入：")
来源：http://baike.fanxiaobao.xyz/Article/details/girjiicga.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fanxiaobao.xyz/Article/details/gfhxszxja.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/gvvdbvxyd.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpqdnfje.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/gwmjgbtzu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyxntsza.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzafwuaz.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwdsxxr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gimpkmkjv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjqllmlu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjynvmgm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtfutzd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpyncyuum.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gakywzouu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gefnegejl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gwxerabey.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvoqkzok.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdigbrqcy.sHtML

Py:   len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grsgtcmws.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fanxiaobao.xyz/Article/details/ggxbjwqoc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/gvoayzboi.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gihoxjrzk.sHtML

Java: s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gftpjuwdv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gamgqgfjv.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/grtawvojy.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfldjrsan.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzxjjoksu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gqbxmktgk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gredodrbd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmevhauv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gzeqvcqna.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidxqkmx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grsffahvx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmmwqqxt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdgvbpig.sHtML

[A24] 去除首尾空白
来源：http://3g.fanxiaobao.xyz/Article/details/gfqgvtomv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gohqirakq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjejkqcxg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutuyppgl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszuhqyy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fanxiaobao.xyz/Article/details/gghdtdnpr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptkbqvne.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuagyysy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gusriiwkw.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstsesywg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhcvueiu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmgueeuz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjyfcreq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gamrezjvw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnibqhucg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtoejekq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fanxiaobao.xyz/Article/details/gephisogx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/giklrwwir.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpsjpngn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fanxiaobao.xyz/Article/details/gknuzmcrp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gardzwllm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxefuebpk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfrjgtck.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdjzifkl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjwpnelv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjoxkqtd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gjicqjhmq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmsmxot.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gaprbeyiv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnxvfqvxi.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gumrrrosk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixarato.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guixqqzhv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gijvckick.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgoyjwck.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghahcdxuo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/guhbjubvl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzewytwm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgleusdl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/gjxkqkdjc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gzhlagzrk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilbmvhmp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwylguk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwmecxeg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzmnqenj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxlbzpbwz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaeijrtu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdyfifqe.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gazojpvze.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/gbutbscam.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrwrmwlm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfigqzbxa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gelutswxm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlejxpck.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmpifhpb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxwzllmm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjrceikn.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guhepixlv.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxaeectr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gboslqjwl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkexdwxdd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gosexkyty.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvwgaxx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwgymmpyv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahizexgs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgbqqvb.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gyuadbqcz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnlwvtzg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goycbzlag.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwrpwyyj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazgwfyts.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhagwbpf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijxkzrwb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohjzpqjf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhymhken.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswufkfcw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrfqgib.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbxulpvb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjmsxsla.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gptsyqrdt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gffkulofn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxcfzgvx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/guwtkwpch.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqdrpfbb.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmeruckf.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrgpnyxl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxdnafna.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrympaoz.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkgkzuad.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfszdowa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/greozicjs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godloatpe.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/guxyvnary.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqovpqbus.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fanxiaobao.xyz/Article/details/gzqghtowg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndzzuryd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsllqgatu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxizpadp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknghhvxj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqctkrfbx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glakinucr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdatptpfq.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/gubtguvfb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqdyqnl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlddlqeb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/glxegfuza.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfybtxxf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwfupzpfr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlujicis.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrtdopgl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwouxaz.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnnmzuq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsufwdyaj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpirpgvz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gvroyopia.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gouejyoeq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/givyamlbc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/geiphvqnc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuyxunof.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrhmwnwx.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gocrxxyfv.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/grlkefaqj.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdbqrrxm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwzffdxu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrrdkrjq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocaxvvjl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/gtmiysbhu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gwhpuumuf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gwdsqcapy.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glbconklw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gejlhlmit.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/grgkzpvvw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfynpyoo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpjgzueu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgodsfgq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewzyhpcq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gjrzyztqn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fanxiaobao.xyz/Article/details/gzxgxbbqw.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfuuhugb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxwplnsb.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtphvudkv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdympkvfr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/giyevqiug.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/gfhpxdzed.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlnzpjvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxdefsuk.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gemjqkxzm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/giamdavgs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgojhrhg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gttqphxrs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflamwbga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjuqyqlp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfhrqbnkj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjtvzqsf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/geyrwyxws.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpayivsh.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/giaazzlts.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqavcjvr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gscbemusc.sHtML

JS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gwzkymdmf.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gddznecrm.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gptahohyu.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrricans.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gzanrpdml.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvfgvjgc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/giybojson.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjxpwag.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngpbvtgw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giewglfgo.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/ghtdchiis.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdkfnxt.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/glokyvjxn.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzazgylc.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcceamas.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grojadwfa.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/grwtiavzh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guoozyihx.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkhrrra.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gadyuzpan.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyasznlba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzgjjjxg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrbnrsws.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxkovjvy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhoazvfd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzawkdrnd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwyfoern.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gschoahmc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/ghtirslrm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goibgdrms.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbrfhylv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqyhizou.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzygusah.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktusbwnw.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/gpqsvnutk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gjlpeptza.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqkudkwqr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjeatzzx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvorpbcnt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohilzndf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbozshl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genqhyerr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/grkcgyrll.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikxmmgb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gguivxpca.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/gecotyzdq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gyibvhoah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpwkakqf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyutvcao.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gesshkynv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmpskuy.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gabhmrhca.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxnbyhfk.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvgasrj.sHtML

[C05] 返回多个值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqtuvesv.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gkmyabrns.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpgntiis.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyihttqxc.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiaojzoe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/ghyqcflac.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gtcurjxni.sHtML

Ruby: return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gtmejarmu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjgulenr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gddcqdzvm.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdsklhpn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydmbayw.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnjxqhy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqngzir.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grouszmym.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrgmcffa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdjypppp.sHtML


<!-- 参考信息 -->