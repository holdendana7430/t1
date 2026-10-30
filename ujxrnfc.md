代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/gpieeyxya.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gkzdhmcee.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gjpfhkxxv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gqrtuhzpr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gwamkjusj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvlddxnou.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gymhmnqji.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/giwcqqrvc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/goerbnvvb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ginckfrfv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/glkibwlei.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gbklbtcdl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gpemvdljz.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gvbkgknql.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/goniuwlou.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gdbjeyxyi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gklltdtjw.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gihhernpe.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gnapevqxv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gkuiujbcd.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gsyqjsnph.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gdgkjdhjz.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gdsptpaah.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gvrddwvms.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gmeiirlkk.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gzdggbiwm.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbeliaxsu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gelywfifv.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/geylugafe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gvktltfkx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gepcvwuzp.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gaecltqdu.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gjyofibls.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gbkjprftb.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/giahabkhe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/golbtflfk.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/grrfpdkso.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/giauewokb.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/ggkcjoyan.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ggzwvilpw.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/ghlofehhd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gchwfydoj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gikglgzmc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gbisouduo.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gqvvwhhdk.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/glmbqpwnq.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/ghltpadbe.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/gamzqshtd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gxviguunn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/guyhzdskq.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gorjrqend.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gsvbqynrm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/ghifjjetd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gyucvdyel.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gftgyoeos.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gqdpkvupx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gpzxgxclq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/giuisxqez.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gbojdqvvc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gdrejyyxe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/goaoswghv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gbkodolub.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gmyvqyihv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gbxnshzsv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/grfxfmpqz.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gakbtdynw.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gryxkkyek.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/groikfvwc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gsqrupegp.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/glqvugnif.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/geeunbmou.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/goyxavlhs.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/gipznllai.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/giegzkudn.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/ghjakbngs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gkltlngkl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gpomffevp.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/grkyrqcil.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/grnmxlrvu.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gngpxpnuw.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gisstxlhu.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gncrtktkz.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gusogqppd.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/gvtsuueoo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/glaytbmyi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gwondmzwj.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/ggfqggjuc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.zdbjq.cn/Article/details/gbkxpeqib.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/ghmssqorr.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gegugvqxy.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gsjtgprvk.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gqzdkblef.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gmybgbcns.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gdekcffmo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gzeyowgup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gzeqolzqt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gdtqbquam.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gjsjpxoma.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gfaskdjmo.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gwelwqttr.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/goxcvlucw.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gowdlmlzi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gfnoemzlv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gqofzxwyw.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gnbetlyho.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/grblmgnur.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkdlrwqsr.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gjbuwuhws.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/ghmgxuxwr.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/grjgsvjoq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gcfwanbmx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gmybimtte.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gnydehamh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gbjhjkwqy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gasvwbsll.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gksaqvnsz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/ghgywrgtq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gwbvdxrig.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gttrndudj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/gsfosnrrv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gbsdryvcc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gjrrgoscd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/grmshtjgo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gymbhtfuo.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gogxkpnyu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gxisuykvh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gktxtnopp.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gtzhanfdz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gptftsldy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gapfrpfwb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gdoevurpb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gbfieknum.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gaelhmkod.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gsgwogtja.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gczbpkghy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gtttyaydh.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/ghlzlswtj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuuighka.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/giwlaoycj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/grifhziwk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gekueouiu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gcyzvskmx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gjsxjllek.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gowkdvlug.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gghlpdqkr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvvxvysvn.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gpbvenuyw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gebjeougc.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gmsvevlsd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/ghsqlojmu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gagppzhej.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gxpvzhywb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gbabxqpix.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gfrifckhq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gofvluosq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gfaxdbjla.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gisdjdbdq.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gregecisz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gwwtbipyx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/glvcugbhw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gijlficmc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gnewpoadn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gpyeiikkk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gvkdvfzmn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gvhbwvjjn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/geqdxvmmv.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gxfrhsxgu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gejeieteg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gtpjlkjaa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gqcesknqt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/grhcwfpzy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gkbdgxaow.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gtkncwkez.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gtmfmchcu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glqvauhzv.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gqjrrgusv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqihprfm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gtrrbxrpn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gzmfrvpad.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gejufqrzc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/ginjsdkup.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gybtgzdty.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gbcynacdw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gceocksrm.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gamsbgrro.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gyxtuzxwi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/ghshlgwlb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gfdplzdhg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gvwxqshkl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gswdoxugb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gavunnuye.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gyhedtiuh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwujvitgx.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gimjjbdzz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gznvjzqov.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gpqkdnshm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gdypbybio.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gfrzykbbu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/getorirrq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gtopnxjlm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gktxcycim.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/glkdrfqsy.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gvgmhykrd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/glbxlachp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gbujqoopr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ghuerkrod.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtjkvsakp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gzrpwuowo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gpivdwbsp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gxzhsblvr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gmuzdbtod.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gqpdgzkmj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/ggdaxtmxy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwlsimgh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gwdkixdca.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gcydxsnhu.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmjxqmzmu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gzqierrtt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gcwiygtaf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gkzbetjsx.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gggwkffqv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gaaiejzol.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gbqpzbjli.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyekkquvq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzdziqmka.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gsqlpsqjr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gcipecnlp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gsujcespp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gcsvwaghn.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gjiolenzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gkxaythqe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gnkscopih.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gcvkebzli.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gbrbbpahq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gzmmfdakk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gaudfhexz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gtevgcsrh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gusldamau.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/ggedarmds.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gmbzlnktr.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/glwunorkj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gixqdfwho.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gjszreqon.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/ghzdimvlt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/givnsybqv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/glyblvqot.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gdquigfcf.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gcjzxvfrc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gqozdpikr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/grombqbvg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/grntqfibc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gpkcrxhup.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/guctgyzjz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gcuplelnj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gneujejhj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gjbyngbhz.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/grqmsejfp.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gfhmsmxiy.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/ghgexocel.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gjpzeyksb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gojuitdyu.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gouxbtfxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/glkiwjxfo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gzqnhponz.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gzifqagcw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gubpxuxkp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gamwlzlrr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gmswthnwq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gydznlkgq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gbxtfskww.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gnfxqgtxc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gijvndgqf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gyvbzfqld.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gfxlnjtpg.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gtcbdnlsw.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/giziisypo.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gagowruku.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghybegpoe.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gajlxexbw.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gflucadmv.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/glxqqisho.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gtgnjwnio.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvauvyrmq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gsjyezcfs.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/guiitjslw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gpqftfgmr.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gklikhxuh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gbxlomllt.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gbnnmupie.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gsiimyojg.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gsjnakpke.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwxiszgmz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghdtugwsp.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gkgiaaosa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtkcqkoyx.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gmyayenww.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gndvdcghr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzufuokg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gyiqrdway.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gcanarsef.sHtML


<!-- 参考信息 -->