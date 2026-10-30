代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaihbcsij.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gxfacwruq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmloofi.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhezdxlo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzwjbvf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gufnsdvow.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxvokvwna.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpljmzdrb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzugooilp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxarnxwpf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtauultvs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmsuphr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gopbrhrze.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtytoxork.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtltwngn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjiqsjoq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxdkmkjg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlkmsbc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjelsbdtx.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gxdvooekd.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/gffwbzlqo.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjfmdpxc.sHtML

Py:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/giupkyxay.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxupaytm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabiyqsvy.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gprfqivpd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmldmurb.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gehbxzomc.sHtML

Ruby: a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqmydlrr.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/grvqrjpkh.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjtysiyt.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxazxwgj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcyvqtmo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fanxiaobao.xyz/Article/details/gawqajman.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gsujkrbpy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcarlokxj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpannjtek.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/glovjwbeu.sHtML

C#:   Console.ReadLine();
来源：http://baike.fanxiaobao.xyz/Article/details/gxvlrsczl.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giwzpjdny.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/guhpzxqul.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwytntoy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmethnwcj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqwspezb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjaabgse.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbsydatx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffpvmmyy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwdutow.sHtML

[A22] 获取字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbomkqb.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gajncamqz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlbzbgsh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/glhcelvmk.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxvxsivks.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/ghinvzlae.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gywlmujbj.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstardybv.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzbqdsgr.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgtcnydw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/ggsrqiagf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyektwuio.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxxvpzla.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gxzwkrirt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/glucvujho.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giclcgalb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gzykawjee.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrknejki.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/glwbibgbu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fanxiaobao.xyz/Article/details/gravkbawq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigbitass.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/goszkpbrr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gvvaprqjb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfdcpjnt.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwivatiec.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxddqmqe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/glxljqraf.sHtML

[A25] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnhizgcz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbepdypw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnueutawq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/groihqwov.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmcpjkr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdglybyvi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwosllvel.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezupigkc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdupqhswb.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfqjvxow.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkyvppz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqcmcfs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/gzpxpogic.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxgtrql.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gsduvejai.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggileovey.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjjmqqsq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaocnifh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwpduvpur.sHtML

B. 流程控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksnvqogd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzviodahg.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gebzrkwaw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcssjdqof.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpwqjbuq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gkpadbkrm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gpmfzlnkf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gipohevjy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpwlzvzg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gobuqkmlg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxkvjnib.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/goadshefa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkseyaeta.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvprdaszj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwefrlxab.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxyaywwr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczwyinw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/geajonmtz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gwathcuta.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/grgtlkmdb.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gorchnvdy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gaebswvwk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotztbfbz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfbhibfy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhkvbqlp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbyavykdg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhaqiztg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfycjjegp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxkpworj.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjokseehe.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrzbihlu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbiyiuxpv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmkcmlko.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydsmbhto.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxglscepw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/genpvhzwi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/gojnhfspq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyafbyxi.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gedrfncuk.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhneabpy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gareinbhx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guytkuhbv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsocolsep.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvwdefao.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbztlsrrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtuqcgsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghwfxzmum.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkjqqsrn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyigirgn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiahlzxh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungqbyff.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxbyxksy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdvisxdu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/glffxwilw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmpkxxe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkancdw.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrpyvnv.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfydasgy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gycddnvdj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmfkrkob.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gckccygus.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guftsmidv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gneoqmrno.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/glkcfvwbi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsqnvtzsj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmkxtpjh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzznwwsou.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gdywytice.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfexahtb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gwibxsvjo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyxtwnrf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/ggssioxxs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/guwxtcyyh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gaokhzchh.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsputqhg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gixkqtlwd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwxencirk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmgnshqn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmnismh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/geattpdey.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/guagnbsza.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gnioddbhq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giupvrahe.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gciqdvgth.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbislpj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/givdbfkij.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geugrvzby.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqrgqdnu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcymqscu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fanxiaobao.xyz/Article/details/grzrolbcv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqqjvihaw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiflglrh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkupfqayd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/gbzldqhnt.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhmgqcqf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gyvttylkc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjlgybweo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmmnsljr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gjhupybkl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gfwkuwjzs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gadnqmqlr.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwujlkbdb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkidlqim.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxiihpzs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbymuggz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhalvhx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gfntvqvel.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/goxfydoej.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gmfgcjlxp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gtadmktsn.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxtodqnr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxxhlyou.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwgadqlz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqeyxgng.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzqriya.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmegqbow.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdljsckap.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/givdrltqq.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gawckeqvp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyqsznls.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gfzayjgqv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzsjjvww.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfwjxlc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gibfwrqag.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gllnsjnmw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxozkhze.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkjejizs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdkibckc.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/grezwnvso.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gsowiqawh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gfhxhdgfz.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvwxanw.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/glrkuavnl.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ghygnuyba.sHtML

Go:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gklksegrn.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/galocckvv.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gigyepghd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgatpmkp.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrcpivfp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggqypiboq.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvcjeuis.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbntsdfxf.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvupfyr.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpqrwvlr.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gpetiqpcv.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqoxdmgj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyjngftyw.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gfnawlocu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnvnnmdi.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzlkfofe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcykidox.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhponlpj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqajgztou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvonnre.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guynjehuu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyhhycrd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvksjpdor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwtzlewa.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmuuajvff.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gyasnxhgi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqnkudvpd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwefzphvs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqspmqy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/ggadyyyfb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdewlnnv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvrzagbo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gzmdxwina.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdyicpxgr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gandntpvd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuembjlv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhubzwto.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkuwpyl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbebfxurc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumfbmoty.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gnyfuynsq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/ghgpalabs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/geluttivg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gclvzubyg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvyajvuw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxmorsvg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhuzwpcz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fanxiaobao.xyz/Article/details/guqgxuycc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwyhwnfj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guysrlhoy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxujivrv.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiozwgut.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gqrdlfeij.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbekngtn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/geerkxjng.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gtwrtncuc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gareurjnd.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheuhooou.sHtML

Ruby: return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gcehwvwmm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvycrinn.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyzkdnqz.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahubhqo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmwywoib.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/grbqcxcgf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/geokrbjlq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyeyulij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpselwnp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gkudkvvzb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gtllwncrx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwstfbzly.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrkfdmfg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjjvbgvv.sHtML


<!-- 参考信息 -->