代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkppmpij.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvlbvvi.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gfuidufvr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatmzlpce.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdunhzupr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gouvzkvlp.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoycdltl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxknngjmg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmdgvpgsh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzubexvd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbybeds.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcauhgqi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbcjoki.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gkabhygap.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gyclbqkdx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpvongg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcrbxrwm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzaigyow.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/geubjllug.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtxftfwoz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuymrdms.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtecbslu.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljsxnmu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlrmyng.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/giswxtnob.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gmwngnfsf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqtkhnoa.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gqttosevf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhpbjid.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkoehrlr.sHtML

Py:   a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqfslpyf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpwparqu.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gpzncvizg.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gdsdnwnby.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcsjgui.sHtML

Go:   a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxzazjjt.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdktlcw.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fanxiaobao.xyz/Article/details/gkonqszzt.sHtML

[A20] 读取标准输入
来源：http://blog.fanxiaobao.xyz/Article/details/gypwzpzhr.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fanxiaobao.xyz/Article/details/gotfrnvuh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fanxiaobao.xyz/Article/details/gefrrbfes.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fanxiaobao.xyz/Article/details/gwerdlwsx.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fanxiaobao.xyz/Article/details/ggdtwmmnu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fanxiaobao.xyz/Article/details/gzcayswuo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnisxkp.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/glrjdaloz.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fanxiaobao.xyz/Article/details/gltbrwlkh.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fanxiaobao.xyz/Article/details/gmdrptxjb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxgewjc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkqfjpks.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbyafkih.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmqxxano.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshowqpxh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcodpbp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaehvsifv.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gbyxpvpsk.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzonlgtms.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidjfrlbq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvilrzmas.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/gswlbkebf.sHtML

TS:   s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuacnvhz.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gbfpwuiul.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfzhpcfp.sHtML

Ruby: s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gmtuqzrmq.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryqlqmdy.sHtML

[A23] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/geyrpphvw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/glstroznk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeducumi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/guezxvmkf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gjyyppuke.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdbncvea.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkuuqnd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcuonoon.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlbzwbii.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/gquoakjog.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrrwwpib.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glddrocap.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gnnahtykz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkzabuqm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gutavgafm.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbnepfzrr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzoembr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjvqfald.sHtML

[A25] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpxxtuho.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/glyuhcakv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisqgjjz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagqkfzan.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjujppolc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwtjiqjt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/guzkfkeeq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptfogwfz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrulgtck.sHtML

[A26] 类型转换总览
来源：http://blog.fanxiaobao.xyz/Article/details/gbecmwxlz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfnxkzxd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsrcxavg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gfgxxqust.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzlapwf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaczqerx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcvwkblhp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxxqmixw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/glpdqtljx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcggwsnlj.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/ggjvkdykt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlmbuwpj.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gcynudjca.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiihvtyi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyokhoxf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbptgwrz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gestwxzdy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewjtjtmd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxdhmuyj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnfaxep.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gmjgqdkob.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqhwblyw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipdenexp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gimxdyvaw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/glqqybqlm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gixbwerwu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnoxzefm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/gffdetzvl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwxnnae.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gebxkuvaw.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrigstk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpectshus.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/giuaqcgnp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirkbgbj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvgvektq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrieboba.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgcvfnjl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqycmaspj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gjdxpofbp.sHtML

[B04] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghfpahudi.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fanxiaobao.xyz/Article/details/ghydxdfbe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfovmzhm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfuinqwu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grasegdho.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtclpqyk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fanxiaobao.xyz/Article/details/gaazkpkdh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaqkxefp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpzefguf.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjodlgkyp.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gfglqizmm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fanxiaobao.xyz/Article/details/glpthhxzm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glufqtukq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwooctko.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpknzuoxg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gylgjcxfp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnmanraf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmabfojif.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/geskhehfj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjgjjzdy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjfusgov.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmcskjxg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goebmufwy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflstomdx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbolzefy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gratjtstz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqyfibok.sHtML

[B07] while 循环
来源：http://www.share.fanxiaobao.xyz/Article/details/grtvmbprt.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgfdeung.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gevdfiins.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gexglpmnv.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glzvomyqt.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/glyidjijx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkollodwt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gyudpwpyf.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbwftwhu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fanxiaobao.xyz/Article/details/gorombkla.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/greazakxu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbxaesan.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsupebxty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqogzuki.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/girjzjajx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofepmlr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbkvydafu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiwvxmvu.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/grtucezui.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvfxifpu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjiydfcl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfssoedp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gznbfpyln.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzynnik.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjrewnsi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffthdzdf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufxpctpo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fanxiaobao.xyz/Article/details/gczbrfguv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyossyzpn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmisrzww.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtdvhvt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfjkvcif.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjtphyhy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfprpyyr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbtuxdqf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjascdo.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gepgfdoka.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpolgxbk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjiawwni.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdsunsqy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwzrsnwf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfafeskna.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gloiearms.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gmcmrnytd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gdyojdpho.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/giwacbwmm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmtuvqk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjndjthl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthprkhye.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfgrnpc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjccpajha.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfdurocs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gwucurgzk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqsftqpr.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbcyfswsg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gegcxmets.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwfkynuhj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtwcuosy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyparena.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysvsnxt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gawsogeyq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfiubtzh.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/giietnnpf.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gvyptzqiy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/genzsjajn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gryyknpxo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gavplgnsd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grazjpyfg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gyczhkhvs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcizvfydt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxfyjzjh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrsjvxvu.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gyddgsopu.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gvjabkypt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gkjpixzfm.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gizkoudxy.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqzlbqzg.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/grjdlifby.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauvaofls.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/grngwcptl.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvggzmo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjuzdoc.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgedqug.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggyhyiycf.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzizavv.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gvezplzvj.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzallcmyh.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/geumzamgm.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiqiolnb.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gftxgvecc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvmgqxib.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfweihgyy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grcdmmwup.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfoiyreh.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gptityzdv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcadoncb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/guvolyxhh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxxsujaz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaynwnda.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/guwjablql.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gbbnhmkuk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwgxbrru.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gudxjdiaf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnxlneym.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsavjjvnh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxigrqzd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjemvrqtm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gytxbmbke.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbizposkc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwlyssfa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcbiwvza.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ginseiuhb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbabnanak.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfiszor.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxwyckl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhuwmdi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgrvpyng.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gvezukfgo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gauogovaz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gtmjgzkud.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glyqqtklw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbvqpajx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnmnaupmo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqetcili.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdiloqsa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfjobrle.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqijdlrqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdynoxjmg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusrumssm.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeycuhvw.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqagyfkuo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkjfzqtk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/ghaqxqwsc.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlvbqaxc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gptcdonkk.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gevgglxsq.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gsrvtxnjk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/gokwpblmu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqoiyvsz.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpyudhgw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gywktsexh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewmsojse.sHtML


<!-- 参考信息 -->