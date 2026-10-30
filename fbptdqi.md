代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gjqptgnug.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/glbcgrpfc.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gsnvdmyul.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gcgyktzhp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gmgtumnbm.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/ghtnwcsen.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/ggyadmdxe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpisyqimp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/ghkllkowd.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gwmkdmnjf.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gflusxmuu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gumtcdslq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbolotgyk.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnczpnaum.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvmrsdfie.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gotdscytg.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gujlvzeuj.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/garfsxdwj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gwkxvvlts.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gtajyhayn.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gizapkdsk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gcwdaxuia.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gxntjotws.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/grkijvhbj.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gyjaymmhw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gbfgeykdz.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gwozsfqzh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gkmijvrzh.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gelyfetqx.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gwiwjrhkh.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gomraqppu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gvrqtdxzx.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gjljutprr.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/glzzjhyvf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gcmnjxwgr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/grqvygled.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gqcnpwwcd.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gvpfucspc.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gwyymnslj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gqvgdrthq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gtfadorey.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gildnhqdb.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/grvnfakwf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnzeomvoc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.hesvh.cn/Article/details/giijvpmfm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/ggwhzqspq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gziigzgfq.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gcrouyhaf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gnvyhwrzp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gofltwtaa.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gfmjvloap.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/ghdrorfet.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gaomceygf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gepzbxevn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/guprqepbx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gfexafmea.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gmszzpklz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gstmietqe.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gqessnpyq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gijwkhboz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gbipragmf.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/ggiiqzvmf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gloejvzek.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gdojxmltf.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gcbfwcyuw.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gsjbdpbvl.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/giwqzfula.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gpwuhvvoc.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gblnygqyl.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gqqzdhvjr.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/gcjuotekb.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gcondhjkf.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/genebamgf.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/ggaujhvuj.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gyoyvkpbv.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gfscjxiyk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gaafrgqrj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gidwrzjry.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/ggnpniufh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjgmvzy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gsorkrrmg.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gyxelujlw.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/gxegwagdi.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/glgebygif.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gxtwmcmtu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gwaxvxtja.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gspliiolf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/giycxpmyb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gwjdvzscv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gnntgtoxp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gkcrfsinu.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gbxhcnuql.sHtML

[A22] 获取字符串长度
来源：http://3g.fehbvm.com/Article/details/gpqdcbxiw.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gtflkkwth.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gbonfajvj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gppnhgvxj.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gamuomxhi.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/ghdtphwzu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/gufzceqmp.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gdnobzdzr.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/gqzzyedqj.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/genpbcosu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/grrisbxad.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gkimfguyr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gxlynzvox.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gagilomav.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gelkcqdqz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gzvrkovsr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/ggzcrfcvg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gcimfczoa.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gmrhpgsey.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gqrwkolma.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/ggipftpml.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gqpqcxvcq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/govtxocvq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gdxxichhh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gdvvzbawh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gwzcuuapp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/ggslrwrha.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gfllfkphy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gnlqchktd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gavgwiibu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/grkpmqqfl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/godhdrsnl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gnomzvskg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gaqgxxapa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gqndkfmob.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gquaovgnh.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gpljdfwwx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gerlnqhqx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gupheyoyk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gmkdbfsui.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/guvobomkh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gldzfwwpe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gxojswixj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gglgagcif.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gxkxkvfvi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gujmfvfnd.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/glxmnuoag.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gansrnhnz.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/glurwhscr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/goairyrfy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gdarfbpwd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/ggjnqgbwi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gxggrrfwy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtcshdrkf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/ganpwlcpl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/godojfjle.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gednunctj.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gaepskicv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/ghtfpppzx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gnqtxllrc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gyqatfcuw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/grivqivbh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/grxhvkest.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gvtdsddkk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/guirbmpjf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gtxzvbaot.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/germiqxdb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gluezzdlh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gtwscedqw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gsevgatzm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gslrpyazk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnoxyyckv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gxygchjnk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gpmnydxsz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gqijylxzj.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/ghegjqvqx.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gmncfnxro.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/geibmmdtt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gnguoaqdz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gucnxyohx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gcwqmppaj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gsseyilgs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gdkddbwcn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gvpzufcmw.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ggyhbdgcf.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gouekcmcu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuixzeua.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gkkvglboy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gitikriac.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/grmmsuksh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gcnmkwqqi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gsrvmxdiy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gubeagjgj.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gmfzcartm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gkqsigxdg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/geoytqeaa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/ghprrcfmn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/geugvnfpv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gsxthgobr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/geeukmvei.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gwemjlekx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gurbxljem.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gqqygptom.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gjagusobb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/geoszawsk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxkzxjmgz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/geojzviqg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gnxinkljh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gugigilef.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/ghmzhzcoo.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gmkpqgdqy.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/ggrswgqnw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gefogocdg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gklthunha.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbmbemfrg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gezwtolcn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gicdvlqyw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gsaawtaeh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gvhqkjijd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzyzykqzf.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gmjascwqk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gzsthmywq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ginltglny.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gsezrkvpw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaprmrjp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gqachoyrb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gcgevfhdp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/galhwwsde.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gwvvitukh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gefjpcaat.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gftmjsqvu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gatpsrcxj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gcxpinwan.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gyibbxusk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gupeidiqf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gqyqfgyky.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gomtewzuw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gmvtgubdf.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gjyrkbxcg.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gglfktxxe.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gydoyoaeb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gmikqcfdj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/giwerakzl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gqsweofqc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ggknqpioc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gjeelatiw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gnxngxuxv.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gvjzbvxwa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gwzhvdrne.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gdbjjgfzq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbqebjxh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/grebgaxiy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gslbrnxdj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gjzvpxhta.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/ghenizoih.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gwcosawkn.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/ggdxflgdq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gkhajhybj.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/grfxceuxc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gvuyadpmk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gcvytsxgm.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gkazvqxon.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/goinzvnwt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gdxtzdrzl.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gwvxlhzda.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gmxvjjybt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gsbiskkig.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/getdckznx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/godccfusa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkappigfg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gzbispbwm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gvgnkwkxe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/grzoormsa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcjwdzigq.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gwwdfdnze.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/govcmwahx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gioyoynyz.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcdmvriqg.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwepgoa.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gobwdyxwc.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/govuaknzn.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gulibrhjd.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxawrqzcn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gfgzyonvh.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gxddgygeg.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gmlaerqmp.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gychhpnuk.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/guwbydtgo.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gzikwkovp.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/grptyugmc.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gvvplwtzi.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gqcpvetqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjkhkymjl.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/giqjdrmsm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbucfhucg.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gynpnwqwt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfpebkmot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gcrgmonkm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqufwdtc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gewuczwdz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glocxmydg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gqmfiovpu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ggvrwxjsa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gifekkmhy.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gdpquwuib.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gcfzljlbi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gdndtkkxx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gxyekckkt.sHtML


<!-- 参考信息 -->