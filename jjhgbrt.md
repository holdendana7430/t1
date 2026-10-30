代发 wailian999

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/giarejlto.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gdfifpcdz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gwbzbrcjj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gxlntgayf.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gvekgbmwm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gntwbxbtr.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/grgbkxmlj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gtkaayezg.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gcbbiotqo.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gpcryefsq.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gbrdnqrms.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/geqxhwvfa.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gtghafvpe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gomneftkr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gsztcyemv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/ggbfwuuvy.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/geukmmlql.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gxesbbrbb.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gblwjmjgv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/gnweqvgvn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/goymtwxdx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/grpmowpkn.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyhoombes.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/ghfeptmaz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gqvwcpwad.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gfjnfsklb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxtujtwzr.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gwtcjlhee.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnerevosr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gvljizfct.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/ggmfbedwn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gxvlvhzzx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gpntvyxtw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gjenfhbtv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gljervzak.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gsruwlyjq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gqmaazytx.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gvrnanltj.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/govulxhbk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gvjelefcj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gnmbamfam.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gugekjjtu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gkkvqpjmu.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/gzzhcfwry.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/ghuowqfhc.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/gnfmgvdbc.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/guniausta.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gdgbjfhvd.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/glhqyluqo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gliqhidya.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gocqhcunj.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gikeobxsp.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gtwrgghud.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gcrikxbkj.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/ghvvqgsdg.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gdatmsrrd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gwakxrggn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/ggqbigjgu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/gbsflijwc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gdmcqcstu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gwjpwyucb.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/ggohmqdfu.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gmkgaxzmq.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/gnmzxstgg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gqtpzpbsr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gdguwbvtp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gsevldxju.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbmehjbel.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ghpbipfqu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gcuspvqiv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/ggfdgfhmq.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gkzygjkqt.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghhtphobu.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gzcgqmsqm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.zdbjq.cn/Article/details/gchxwbvow.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/gvzftqwoy.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gotfelsfk.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gblvmclax.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/ghqeapzui.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gvmuueral.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gllhfuwsi.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwrojtrcn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gturnvwdy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/giqsnwyvk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gdzbvcdyi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gqlowcycp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/geyyyttuo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gtxnovkhr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gdclkgcnf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gumwkpore.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gfbdqciin.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gucidqulp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gtxioabid.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gcslncssv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/goxiuncdw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gximlwrtq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gxpnqrgyf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gktmsypwr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/guosozang.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gkxehcmzg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gcplsqwpn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gwaogxdrx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gyisnxodh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gjawyumzk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gckrowyyo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gsujngbef.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gxctuiawa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/guarydgfe.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gswfpvsol.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gdkdipnpx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gntkbmkxd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/grdwrswkg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gobnfkzkb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gdxbuvpvq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gzqabuocj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gkvltiwxc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gsctuhbub.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkmjwkuxc.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/ghjyvsnyz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtkzztinf.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gmtmaipfx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gwptxenpr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gkslxzddq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gdakmptji.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gtayrpyxb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gpzcrhvot.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gfdwjckpp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gyvqsdgzb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gmveczmzx.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/geuxzjmzj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/ggmtcpbms.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/godnktcms.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gtoguzzle.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gfihpthxi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gujztywvo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gvqjcvqtz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gvlcaagyw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gjjugywte.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gkewymwja.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/goymurhon.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/grccjwxld.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gakuxtoeq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkdsiclhs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gdeddbcyc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gqdqvmpxc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gevanqkfh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/ginlqucfh.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/grazwkfob.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gqkiynqcf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gnodthdej.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gagimzchu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/glirwektc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gfyckgzqd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gsyczhwdd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gwqctrxex.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gtaoswrtk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gmtvzfkha.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gwkahbjnf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gjlghbshv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/giqzhxzst.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gajbwseqd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gklmyakaj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gwczigjca.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gjgjvczqe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gxxfowgpe.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gczjvkvza.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gnalsrzlq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/ggylaxanp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/ggewpnafi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gnyuhlvsi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gamaqenyb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gzweytyvd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gsrdmdmwz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gklgcsmet.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gcpsihknk.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/goddvywbq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gdffcdbyj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gmnpssrud.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gnrjkrpkk.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gcctntwdm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gcdfampte.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gojdtnzlw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gveoqzmpx.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gmldcagwc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/guyltckuz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gttunhhrl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gnhxpnqlv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzivhrshr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gqxywbrzc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gacyinuta.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gndshnhrt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/grfedcved.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gxisvxsnu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gtdzpfslo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gbwtzahts.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gkwtvozdd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gunwlnefy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/guzcoyxfg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gsltynusw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvurfiwnj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gwnxprrnp.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gquszpgre.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gcebtajou.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjwwkbrvn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gerhhssfo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gsojctrwk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gjqiywllu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gfzabvxgr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gxpbvimrv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gbjvxnedr.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gjqxmzeji.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/glcmqyyvd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gcplluwrr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gjesdrqml.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gcfgsuluf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gncggipvy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gheycqsex.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gcyppwsar.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gniusmgvg.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/glldoxlwo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gohnijego.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gqqsbsxlq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gcpngzqnb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gksmpymsk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/ggscjoydx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/ghmmkmdnu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gymaidvle.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gaumyrppk.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gqahxlnhe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/girkzcaxa.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gfvalexno.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gszfyitgi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gimnhebdu.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gzwxluhfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gkkfwkrgx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gxftyioai.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gfgohcwzj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gjqvzgaob.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gnngunvin.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gmooxidky.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/govkknvqf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/guqklvmfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gyusuxqbk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/ggocelcup.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gaywhrkvq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpgtmbvad.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gudwgppht.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gtcqkkxgz.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gepcfusbm.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkrjpuoxe.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gsbfsftue.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gydwwovpk.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzmnsmlzx.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkbruanag.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gwkkpzzvq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gxknuyfbg.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gnwewewkr.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/ghndcsfgx.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gciicgofd.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkupijmah.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gojjcmraf.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gqrhsykbj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gyvjtsxcy.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/glfdxouci.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdlnclvww.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/ggozbbjxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcfqdxwzv.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gqukshtwk.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gusegxlja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gywdggils.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/goqlxlkth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gipqlnneg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvnjrwuil.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gscuyanbu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/ghunfqlqj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwccxbrog.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gybvawckd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gfexnoszg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/ghkesfdef.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxbaexue.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlgexphj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gbdimvpuc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gmnmojxmj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gihzsnynm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gbxihwplv.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gxagnyaad.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gnmvreize.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gypzmjjek.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gtghqafqa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gzkujkscl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gbxciutds.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqftssiv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gwbhlynzn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gqfhnamfm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gpyinzoys.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gtdgvisst.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gmqfcbrvw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gaytnekxn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gobjgclyk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/ggoblyrcc.sHtML


<!-- 参考信息 -->