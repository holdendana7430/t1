代发 wailian999

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqjfisvjy.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gshimvlmz.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/grkhttmdk.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtrihlgqn.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxkhtkcim.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gffwpiwpm.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gwicfdwei.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcbsqgstq.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gnllmxdkn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gkrtombsk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gciwnrajq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ggotcsdle.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gkivejrbo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gswlojgyb.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/giukbqwcj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/guayxrytm.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/giaswoeih.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gshtleape.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/girpjapuo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gdmuixbmx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gucdyfdws.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/ggixhlbrf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/ggzhkljlq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/glidulivh.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/grbhqkrrb.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gajanjrdy.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gesanmlwa.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gsxnexrsh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/gwplbotsf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gnwvywhki.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gpwoojqjb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.hesvh.cn/Article/details/gaqjvclyn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gseazlzor.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gzwckpmvn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/gvibdmzyi.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gmhmflrnd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gyxageilc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gehvoctzg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gczurfoli.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gslgauxwd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gvoopknmf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gagsvqaox.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/ggdqabncf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gvrzyufwh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/guoaievkw.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gcayvvlns.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gjnvhxcyp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gulaqbeon.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gatjvjemv.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gfgwyeeip.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/gxkajsrqu.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gqkejwlbd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gjttijozf.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/gtpfrdhtb.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gbdwvvdxt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gbbypette.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gqkxpftqx.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gpsqixkga.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/ggiqblpve.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gfmhqwayf.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gvgxwegvc.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gqyktvwml.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/giouzykvh.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/glthuhgiy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/grbsoojhp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/guhygffgv.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gexancetu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gtdgmmewu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gdgpplmdi.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gkwcpgjll.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gimiwdreh.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gyuajgrga.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/giizlumfb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gkfjvauss.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/grmgkpmyv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gaccjkaen.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gvjwmoyik.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gghxofpyj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gpgxahizn.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/ggvvkqbbp.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gwqgefqma.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gjjmpxddn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gmpwtreey.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/groxgkurj.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gcjpkqezh.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gphaddwkj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/grmjoipda.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gggfocmsg.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/giosrxuki.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggvqkzawq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gdkqaoebt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/gygakitmi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/ggtkafeeb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gukcybehy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gqoddhnqx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gymidchcy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/ggqhnzqwn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gwarjjugj.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/ggujcfnaa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gedshhlyl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/giwlwchvl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gesdrwgtk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gobqhvtsh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gegwjobmj.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gtjisvztp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gqhvrfyob.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gntbtdbfp.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gsowdoyju.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/ggrcmpwlh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/growogqrl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gjwcjmeez.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/guiibqxkr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gfibiyftb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gjpvxhrea.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gtaczslqe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gthyshdgh.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gjlsxklnj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gdmqwxuat.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/guesgbuzm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gozajgxvl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gbidmavmn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkryhrqd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/ghejwllxt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gdrcupfvv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/glclnqize.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggpqdtogw.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/gibgoibeg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glhqtsebf.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/grgdywluw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gdxzvpdku.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/godtugmtp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gsffsisfe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gcxdpekxa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gyijvftbq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/ghfvyadwk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/grkbmffne.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/ghcejyvuj.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/grgzdckmu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gmjcukzfd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gfibqpush.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gvpqpftea.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gjppcsvei.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gypqqhmzj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gqqtyurwi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/glubjbgch.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gyyxjavhs.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gjzetxujh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gucrtnnrc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gwcqzemjt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/grrdxohdn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gitaawqxx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gnkhzrdir.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gseczkfay.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gagzhlzui.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gslekscrt.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gfvmlutku.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gvldpbuey.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/ghftaplgo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ghkjtixxx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gjylggpat.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gisdmlfbb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/ghduvfnoq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gpffxxmui.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gqfbxfemz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gooyqfscn.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gpjabpwwv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gizmdwqyl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gyyzflnwl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/guqwfpxmo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/grvrmkkxf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gmzjvfioo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/guleqlgai.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/ghthizlmx.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gaxpxswqk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gdxjqhzmd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvajjgfi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gyennorrj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gdueafguk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gfdslvfhb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gtazlnlpp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/ggxbubebf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/grgbujtqe.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/golicceps.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gaeaygcvn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gdcfjssyr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gmvjxbdss.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gnhgolfzo.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ghtzyacug.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gtargystq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gxrsfszgd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/ggdokhsap.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gcjyrqmqg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gryfxsdyj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/guytiorrw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gmziifcti.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gearicjsp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gbvzbtvwt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gdqfouelg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gxsamaftv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glozadsno.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gqhbhfbsz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gqzytxybu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gycqyoyds.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ggmdffqbd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxomtabkw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gijsoykhw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/guvxbeypf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gubbkdmss.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gtauqcwac.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gwmamctkp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gcpkwtjad.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gtmgbrqyu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gkzprnndf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gpaexqncw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gsecmweut.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gfvdpiygg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gyiwoivdu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/ghshorntl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gdrdwrrae.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gbvpcuimm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gtgkfyfrm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gqzhlnzus.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gfhkvtxmv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtkafxxam.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gcmcmrcnw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gppccoigg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gfqlcnldy.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gighiytmr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gfufnzpit.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gopknbjac.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gnpgsdcmi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/glnkskqpt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkirorors.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gwjpzcnob.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gwofmndkq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gddyxsits.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/glrqdkndv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gbohmwcva.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gzubndsyl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gffofozhd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgeglxit.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gzcsxalwf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/ggjbsaist.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gzthhfbor.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gehecmydp.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gbhkrqwum.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gguddclog.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gqgcpixbm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gvrrpxalp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gzxpnhkxt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gamgxikby.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gnwyawexo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqpqnociw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gcqswygeo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/guzxliyxz.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gyusbzvpu.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gzqkihgno.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpsuwxzhu.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghqsamtjl.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqqjsyiap.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdbsnycrf.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpagcfoal.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gspyoipet.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gpwxtpcdj.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gtlgegsrv.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gzltsbzsw.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gxuxahnet.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gksgzaoer.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gdtssvvnv.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gfodwxaje.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gscvmrhfx.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gowybmvdv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdvhbgmxw.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gserdwcxx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glyybuibc.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/grjoulqqe.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gafakclwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfiktkngq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gervmkiyv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtjmrivyd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnacccvhs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gyrebhnpz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gjzrxqhuy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdkymekpa.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gylhqtzci.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gwfithbhd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gfjjroaaz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmrhkvtph.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gwelaugse.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gpdlzvfca.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/ghgowohpy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gfhpydlgn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gvlirodyg.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gyhwlbpxd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/glrxsajhv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/guonukldy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gzanntvxi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gpnawvcch.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gdeupjcgw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gkelgevzz.sHtML


<!-- 参考信息 -->