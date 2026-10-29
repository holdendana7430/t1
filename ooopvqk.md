代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gffgzqgas.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqvaxudom.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gfpudteaw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gsldaclmm.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gvevblire.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggauxmzle.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmmhyzwxz.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwztijmmu.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gcyjansmw.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/geozithbl.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/ggdedyfoe.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/geuiqcsma.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gtvbwdjui.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gcdkzfksd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gncippngg.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gkrzfhylk.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gjawvxjio.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/grlivvvlp.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/grqjwskaz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gcsvoaagx.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gjbxzqksa.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gvxxdhsou.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gwicvffdf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gtrgkgbuw.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gsdnukngq.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gluxpkzmh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gkuybmdqu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/grpblbdmq.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gvlyeikck.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gweewdosd.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gchbaglgz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gafzfycsy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gfvkcrqpv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gruisequi.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnljbuioy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gnbdxeeue.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/grwvjwknl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gjiztrodp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gorzpsomn.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gzpzfqulg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gobnflxyk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gwriwidib.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gagozbmss.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gavsfjwfe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gwvafpblr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/goswowlbd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gkvoxzueo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gvhpyhlae.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gjtfwkopm.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/glcvsjjyc.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gvgbevdis.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gqnnzoyoe.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gfbrhenyj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gizfugkmg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gcmuxxwux.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gibwsmqko.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/gzicfmktz.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gxpwrermv.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gfapeybaz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gjarmvhcx.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gffkmgcdx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gngmlcwta.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/geoufrudo.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gtixkhuzm.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/giwwqxzsm.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gtcwfrrhq.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gmfaccysw.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/guracmasz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gitdetruf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/guusnaiby.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/grkaevdva.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gpfbhiiqh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gpxycwyxv.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gjyiwptsz.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gwrqtiiof.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/gtfieeifs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/goelrxjxh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gqvbkrfps.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gjefodrya.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gmkxycnjv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/godktzbdx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gsnnyjitm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gnyatzeue.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/gckdvhlkv.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/guhtbujds.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/goyxbglrv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gpxriheta.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gpijrjadh.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gtgivajtn.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/gjedzuoal.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gihvmccqj.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcydrtvqt.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gdnelyyad.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/glzfwjknr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gahynhybr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gbgbdnwmz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gifpwggrq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gcqsqjlsp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gvhdixkcd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqermkiyc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gphnpiamo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gwzilaldf.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gchyjxded.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gnnguftsv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gytinckjq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gcmnfkqjh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gpblxowmo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gwbirqgtt.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/ghftbakko.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gthbbtekn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gwfgndqjg.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gexyyhcze.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gbhtkzrfi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gjhzypqlx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gvwzbciyh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/ggvaerqht.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gfoidsrem.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gifywmxzr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gersmfgvx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gvxerjzmb.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gfhonnvhz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gvvownmps.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gaodvwsim.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/gpalqwjpz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gxxzwjbhe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/greaoghgv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gwrgwmhhv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gehejbrrz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gdhdigwvt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfjznduhd.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/grrnwvvhf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guihdyxbr.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gjovzisqb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gxbsdnhsz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gxyxjxwah.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gllfxjohx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ggjhlildf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gtrixpdgg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gkivwvivg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/guxcwqhav.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/ghziajfcy.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gwouvipvr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gnolgodpa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gqxludhob.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gbuqnbxam.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqmnwwd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gatfhcobt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gkspkuolz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/grjlszwuv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/ggekglogj.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/geaitntcd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/ginndercl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gcbfzmuxg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/ghamvhkwh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gsramacqx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gnvureyzb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gxrhmwkcf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/ggihsumfl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gxoflkmhn.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gjvvlvpjn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gjfmxhupy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/ggdiimrxb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gvpoungme.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gmccclerw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gbhncvpol.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gpzkqkryx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gvuvjxnam.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gzcibvvbz.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/guxaehjxl.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gxcyehqwh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/guamjjbbt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gorhrndwl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gngpxtaaj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gtgquceyj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gjygfywpg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/grznfvktj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gsnjnidsf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gslmswssf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gmitwoafe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gzqpypssf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gsjcyvsrw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/grkowsdur.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gulxclwwg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gqrpvnxzf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gvjevcbvb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gfgxhhdvd.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gethrgzef.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gbggodqrq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/ggmnaodob.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gcizmnhpz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gfzmxouxg.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gjgwnppbo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gzulmsmte.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gnxedfwku.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ghqaovkrk.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gcqyfutls.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/ggbjaeyej.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gnhlomeyq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gtiejcgfz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmhajonyw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gitzajcas.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gvvtiiaoe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gglrtdenz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gljzrtvuq.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/grslfkwqw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gjyesrbwn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gcjfuqvdz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtparwgpz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gujsmiyqc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfbtkngwy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gdymbsirv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gqyvzfeyh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkbprdrao.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gnhjjscet.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gtsubjzwn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gbfljqwyl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/glqpgayez.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gpauuhogq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gazmcgmzy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gmjlwhxuv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gmxspmvha.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/grhfdjupt.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gcvvgsnfz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/ggijokhzc.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gdhebbgxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/grwhihoom.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/geiafktfi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/geccahxkc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gsejzqvyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glhxpccfg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gdzmhtylj.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gdflfwjrk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gfpczpnte.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gmyonlthb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gojrxwiqf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gruyrdnob.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gftkgmocf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gbdvwvcsx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gkartyndd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gocuzupxu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmhrqtf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gwlulvcky.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gzxhmpezd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gnylelbpv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gwzdltjhn.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gayaxkgtp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gvcvkfsfz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gayudwilb.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gfvbhoggb.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/ggxbxreak.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gffbbucvy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/guuxmtvel.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gvhqmizvx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glocosmoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/goyvxauvw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/ggegejvut.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gmnezkglp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmraocguq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/ginhmncaa.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gbacgdjcr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gxziqdddd.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gymqjnfbf.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghlvutoee.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghqmncbaz.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwdfmjoct.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbgvtzyiw.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqcezweww.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/ghhrvdmcp.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gzzoxjtya.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/ghhldzluo.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gzddzdgqk.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/grjgvuyux.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gjiypyljw.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gvudyhpbg.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gyvqtextp.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gwxndwvca.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpgbxbbil.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gdiwqzvbf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gofzfsxsp.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gogcibqhm.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gfmgkhsgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gecaiwjuh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfqciktwm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gkmocqudp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpyjuxsbo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gfzchlhzd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gfcpbriba.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdvljwkvq.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gnttxgcla.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/ghdtecdwp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gqhojalgz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjwlxrvhl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gwxijbpwj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gnthrnlbw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gzgpmzexj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ggojezepf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gcgtptuos.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gceobolnk.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gldfbnicj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gckuzafsc.sHtML


<!-- 参考信息 -->