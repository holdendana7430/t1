代发 wailian999

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxqoijndq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gtvgdrqhb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gqyloqgre.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gttqjwznj.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/ggdysjcqk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gxqexxxxp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gfbsztyng.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gvrmlujeh.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gsjpquqvb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/glulthfbf.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gpmmhfomg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gyvmudcxc.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gkjciljot.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gsipucuso.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/geuciyqhy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gogvaazjd.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/geauidsfg.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/glqrkvgfo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gmeerifxy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gpwiylgwa.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gebdquljm.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gprsxxxah.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gqhqmseew.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/ghmqwkhit.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/ghkixdbsa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gkwjsfaru.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqxqpylij.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gigqucuzj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.hesvh.cn/Article/details/gwjaenfso.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gjvyhbofk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gowbbkkxk.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gqzcjtgtp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gcywahfqb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkmzdxwea.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/ggkwkcicr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gtdxyiprj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gwwkznayw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/guwmbzyph.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/ghkvkiycj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gdjgcfvic.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/grzfrbwqq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/ggsbhoryi.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gwqsomzmz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gsmwgjnli.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gzlzbaivc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gczynhamr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gbczbjcvo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gjodivfng.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gtdtcmxrn.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gpdvqsdci.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/glilbknal.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/gttnukejj.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/glusmusdq.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gcmzghqbd.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gszucinlw.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/guiigvctw.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/geefgsfyb.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/ggdfybrny.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/ghhdgdxyz.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gucygrhgk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gwszgxjtf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/gcqgrusyv.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gmhwkdnna.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/giwsmcsdu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/giowtdowq.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gsvyhefqu.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/ggfudzvle.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/ghswgqoub.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gdgajrfvk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gtzyffcct.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/goylzplyc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gfcrrojxr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/ghqsgmkff.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gjnsatqhf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gntglobjl.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gytwiiadh.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gaauspqrz.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gwwtwfmao.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gpduleysw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/ghsxdclih.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gmseqgeao.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gjbqzhyou.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gpnrzhzvh.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gohkgjhrd.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gipmcpjxv.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grwdjuivi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/geqifgwrm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gwmuvrcqm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gbuufxqqn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gnmwtuppl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gtafnjxzn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gnnxxzapn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gihhmtuis.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/glqvwhlbl.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gjbaappnc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gjixnwcid.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gnrdtevia.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gtdecrcml.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gxgvpsfhu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gmabumtwq.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gtvylsgeq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/goxgpocld.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gdhelpcqh.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gqjvduivk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gfrueenqj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/guwrdsrea.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/ghnuesvuv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gqvwidmme.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gwgfesous.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gylnpvrsg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gtwwpzkpv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnuyywlod.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gpcigzitc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gszimrunh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/ghxqoyhum.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gsslpfaqw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gplnulxrg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/ghqilrwod.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gjfofzlvf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/ghnzylgbn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gzorxjmzp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guskqtfty.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/ghuexkwas.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwljagkno.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/ggndzzhnz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/gzmvyvihd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gyzfnyhjk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gccsuoujg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gndtaftan.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gmnepdksp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gyhdnifuw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/glxhwjsmv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gimtlzfhb.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gxwvbeuns.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gfhdvlrhw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gxlmygjue.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gvjbekmsc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gltxcehup.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/ggnorylpn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gxlnxcjzb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gtbxrwpmg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gttqzmads.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gsptsgsga.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gmafscixz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gptggmkbm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gpebghvxf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/ggxnosplo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gawxyesnq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gpehotvxi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gzwdaefjj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gbeioavis.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gjlquqnjd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gtweepmid.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gdfkevnvi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/goxszqhfh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gllbfdota.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gpermzqia.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gkazbtyeg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/glkojwmqf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/ggpixtrir.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/ghdsqbvoh.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gxmboicsf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gepyaubiv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gykuuvjki.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gqwuaxxzg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gwrczsoke.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gahxuznnn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gkrdfphst.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gtmrmwhrv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gnlflemzt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gpqiiyoxq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gkwyyjhgb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gtbjowjiq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gfydbqnbx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gqifirzla.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gxnyigaii.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/grwavmslv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gkqdntcvw.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gjnrsphym.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmywnnwii.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/ghfwxrino.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gqufaxxhl.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvygyajtp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/guiphwgdg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/ghyichoco.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gplvcrrfv.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/govfyygbs.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/geewutaah.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gthilufxg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gdvwodyhf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtijwawda.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gcwyftcwz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gmddpogau.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gyitvqkha.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gyaxzdtro.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/geyfyjiya.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gdnakwedu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gugxuuuar.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gjxladokx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gdlxtwpgn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbpwscjkt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/girznibmc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gdbzeoknu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/guxbskpop.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbyckkgiw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gxwaxxsos.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gzdllgcyk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gjwjvkibf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/grievhsgt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/ghgckzhbo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gzyggybnz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gdhqshest.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/ghucwiuir.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gkvknbnhv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gcycxehpv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/ghwbwxcbp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/glntztlfy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/ggpkjnitk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gxfopbqth.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gvdbazuyi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/grqbgzjac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/ghrhxkdbj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gzatgxeqf.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/grpkpgdco.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gwkeowmwu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gtjogvtxg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gatarerjf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gdjmkmcdp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gfzdtffgk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gvpictbwm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gdakihprb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gbksimvux.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/genrwqdyy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/ghtzwrkkw.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gqpgqnilo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gscdexdoe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gtoxuereq.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/grhznuiql.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gyauqfizq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gmfjmdahh.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/ghlbsgbdk.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gazguvtan.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/guqqxwdjx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnucbxtc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/grglhazfa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gqruszueq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/grhbujadf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gkgikleod.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gppjukeyu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gibdyhobk.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gwacjzpio.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/ghpbdctfs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gjquhgceg.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggqebypzb.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwbwsiypf.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/ggueckxpr.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gojovlrzu.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gglalynbo.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/glvqqqewc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gsxzdgkki.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gmtooqbga.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gaslticii.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdotsxmko.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gecicmmts.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gkhxgrsgi.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gcoulhedo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gqbyzzbqk.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gklnjloyx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzeednkne.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gdiixmhus.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gihiezhpk.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsbgrltez.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/ghahnzpdc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdwdgunas.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjmishjjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gbgmhngeh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gycqqvyfq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gmqcscmdl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gqlkehjal.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwqfhguus.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gjdbfbzmj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gowctuuic.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gvfmndidh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/golmjmxrq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkpozsext.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gfrloehep.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gswdnfurk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/giadyorsx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gcsiodavu.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/grdyaoetq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gmdvdnzwd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gabnikpdm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtkcmzcci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gefcckdss.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gdzearhrc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gwxhvgkyv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/glkdlnfjx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gqkxexaco.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gloxslfxo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gyyhgxmoc.sHtML


<!-- 参考信息 -->