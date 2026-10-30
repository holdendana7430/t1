代发 wailian999

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gymwutpxz.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcbhvpwbv.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gmcestjko.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gqezkicss.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gyvebtkzy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/giwugourh.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gndwlcney.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gmkdmyagw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.hesvh.cn/Article/details/gsncrfhil.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/ghbcejjlm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/golrsbddl.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gkdttrgkh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfdjunwpu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gzdympngt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gqorpbcwk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gfwyqcyle.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gnvicwwwo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gcapkitwu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gnylbmijv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ghdjlonmb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gssthckfl.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gasxwrxph.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gypucpwue.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/grzfnfxsq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhualtcs.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gcfdvctyp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gghbmrbdq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gtbaifnuo.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gjciclmrv.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/gheyvxhwk.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gfdfsmqra.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.hesvh.cn/Article/details/gecisbbha.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/ggairicuf.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gizgiualn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gcxrgqsen.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gzhhfarkb.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gknnowoss.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/givdcvhzj.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/guaqaklxl.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gtgnvuslp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gzzmcpalr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gcniexbgi.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gnfoxcrxg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fehbvm.com/Article/details/gucunkadj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gonsdjywc.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gpommzkes.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/glcenvfqr.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gpmwhkljd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/geczpsncp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gksypcnfg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gpovokcpq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gcuxerdof.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/geozvtdfi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gdmcnlhuw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gdjdrcqsw.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/gpppvghwm.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gijczpwtp.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gwxbtliha.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gftetxexg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gvhmcnzcz.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gupyadkzf.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gptkbockc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gwsghqgyb.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/giywdrlyv.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gfhutiait.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gnbahlxfi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gstjqqxmd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gnnedtxlm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gtrvzhxyc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gasroonyv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gawsracpw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gmizrlhzt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/ghqdkbtty.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gndcyqsoo.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/ginacswms.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gmyfqlzms.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gsryyryga.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gdrgyuaab.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gfqmqcvsi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gjntwblbl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmkqhlps.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gfeijzsfj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/ginzzvbaw.sHtML

[A25] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gyofwvdcf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gnmtkhhbq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gcosrvqxe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/ghtwvbnqd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gcegpslzm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gvfzbwlrt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gkoupwpjv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gukielgfa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gssilpsoy.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/ggwxidvqp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gljgeuonx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gneevkhwi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/ggfbxrpyc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gznckbwrz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gfdecpskp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gbsdruywo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gyqmmjdhf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gvguvlryi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtdcbcvtg.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gcubwtkll.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdgxvjcab.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/giidnpbob.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gxhvbocxb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gippmremk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/grvqxectz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gdwxdjuig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/ghzqaxrgv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gpmwtbgab.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gmtkuwree.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gclbssreh.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gkufawsai.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gevelysee.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/ghcfnbpyi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gbeuofnna.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gsbxhqanw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gvfkghobd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gldrqfkci.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/glzjhfbkr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gardjbhqi.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gpsgblrek.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gzsuohydp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/ggjdcssyd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/ggdhrmtic.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/ggltwxcvb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gelfvtvxa.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gxzldynxg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gumkjylft.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/glnoqzwem.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ghqxtylpe.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyebmebg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gloylmbpy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gbtsrekoc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gojfyhbur.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsfvyjqme.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gjrirupuo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gmcvyqzsx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gxbsnsvze.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gwbfzpgpk.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gnbhhuouq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqboiljo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gipkycedk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gseoacbbe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/glidnhffz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gddomcmmg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/gbhedwxaq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gbnugjoog.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gpdfhrcds.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/giqonxwkh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gbpldwlsd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/glngwgmty.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gpdaxapri.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxftncug.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gmgkkdcnv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gkrrtoqhb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gnslloutx.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gnbiuqtjj.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gglfcwsbo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqrkcefj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gvfjpqjdm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gawkpsrch.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gkuxzkqdq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gmzjaazwo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/guwzvozyi.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gsdxxxkzb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gpqgqeapy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gequdluvc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/givgyzwyh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gvntjcgjd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvxnnrrmr.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gpbdnrwjy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gtrcaqdeh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gcuajkmlc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwebpyh.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gdaqslbbh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gociiytgy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gasdkeqgz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gzrjimyzq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzwejodlu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ghhunrzyt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gltkxkosa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gkuwzzhdv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggwuwxgxu.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gndwsstrr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gwnkhulmo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gdsfguqem.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gautuemwa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gsqqkfana.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gbgitrmpe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/genybsnku.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gityynmcd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gcntcbzjc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gxsdrltos.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gddlwoacv.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gjqliiztl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gshhoysvs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gqejkyrjw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gsidfwlag.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/ggawzmrdw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/giwcjgfho.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/grucfcsbi.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gtvuvgppc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gnewnikyu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gonzrgmht.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqlwcmqzr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/guykadubo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gcgpgrkhd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqsazwr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gyzqplmsb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gxclkbcji.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gspzdbpob.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gogigjzxl.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gvpyxehih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gxjcgsbho.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqdltrhaz.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gaemwoowa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gsqfrhhyn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/garrxsqmx.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gvvtgnsxz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/ghngsonhm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/guiievbdo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/glehomuon.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkfnysojf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gaupmeudy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gpeqatzvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwdqoefth.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gdhsodcqs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/grlonpuie.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gbckdtqyn.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gvqiibwnf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/ghwopohhy.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gelnatosu.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gdbalewdv.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gctcutpvx.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdjhtlugs.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqberswxj.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gbkzzwzmo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/grjhmffex.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gasvqpzyi.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/geipsopjo.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gymgjuyci.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/ggkbszdft.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gupueeaan.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gactscbsf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/grekfsjeq.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gqrziboba.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwjpufvrw.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/growjjwcx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gztvwlbad.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gyfluvrtp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ghhjgbepd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqutyhqwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxvgzewsw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glovygzct.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxcmrmerk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gigoesqez.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gklhxkwqs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkzxfpego.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvnlwghlz.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gtzbmnzsh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gtzdjasut.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gukrsnxzo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gioueqwyf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gxnttziwb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gicijmuks.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gmxmwatte.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gbliltcam.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gddvyhjdg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gklxalofk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gwnxjhcrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gtrgbbeci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gcgdmumpg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gdqtfjqhw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/grfssbctu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gpxfudnqq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gaxsblpxj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gwldudcyv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gkeikdyvj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqimvxwyq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnxuwahpc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gjedwkgwk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gdbtjkgso.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/glsmxfoat.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/grtmekclo.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gmiberjqb.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gavpcquma.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gdbsolqhy.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gywdyfvmb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gaupmykan.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gprysmtpj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gufpsmpdy.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/guudpiggz.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gasysmzyv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gpucygjpj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gystmhlsb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdetemg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gyshawcid.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gnlpsebpg.sHtML


<!-- 参考信息 -->