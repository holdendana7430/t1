代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gmkuefalj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gacjcqnkg.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gtxxffmjf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gkqaoerkx.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/getauasdo.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gmpisfout.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gqtmkzjbe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gmoyvalzg.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gdpwbrliq.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/grxyjzwtx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gispssdqu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gcnmaqubm.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/girhqccmi.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gyrjochot.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gkyfkzlce.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/giwlguble.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gdnewpiqe.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gwyfhpdbe.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gdmtwmudp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/ggfuwvuhh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gqggizaao.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/guvbhizou.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gertepngt.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gfbdeitjb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gopxzwqbu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gucammfah.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gecinqejp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gvaipfbcf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gepfepcur.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gsnizeuzz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/ggwcmpict.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/grqovjyjq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gqjtxokel.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gwwccrkdl.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gombnxbrb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gsgiutdfw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/guwzlkaks.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/ghrnasciz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gvsbpeqde.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gnbhjxvbd.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gjfhamanq.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gxezgdcpi.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/glelmkokw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gjevhbxby.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gsrvrzpxb.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gbjeypauc.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gfjutqrjg.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gqkjxqsaz.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gyafqndhy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/ghipxrfnz.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gxvmfppso.sHtML

Py:   name = input("请输入：")
来源：http://wap.fehbvm.com/Article/details/gauziywhv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/ggebfpoxc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gssmdxmdd.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gyqywohou.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gvcoxduqp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gyohxnurb.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gtmtpgsgj.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gqditrhkd.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gplvbweyv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/guqmzaqbo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gadbuoxdj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gzsrhrbyf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gmmadkdbk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gjqfcgxuo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gnpccduxn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/godtskpcn.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gzlcquhdj.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gakfkbmaz.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/glzjgjmjf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gxxnexveu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gnlyajaam.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gzwartafj.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/ggybesxbf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gxpoywltr.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gebnqdtqf.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gnbhslxnw.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ghstspsyp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gbwystjgy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gzhdxbacz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gdbladxec.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gnjoyuqht.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gzflqgomu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gjtntnklo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gelixlpxu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gwwxiorwj.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/getenntrs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/gbhmvrory.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gtftrlcav.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gbgrtuwlg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gjfcntndh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gzckthvti.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/ghvcmzkey.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gnqbitflk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gdgkibssg.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gnwqltanc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gwswtkqbl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjjhbgjl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/giwkulziq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gzeebrbxt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gyaiakzrs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gudpdkany.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gktychprn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gwheokkiv.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/ggpabrbqy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gkopffoiq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gcdawxqof.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/geosibnhc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gtdxlugvw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gwrajwxgt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/givlifwyn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gznltbpdz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/ghxyrvfwf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsktenvzw.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gotdhoesj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gebehapxi.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/grzogulhs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gejdgdghx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gbfelfqah.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/glvnhbmef.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gopdzxntw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gvniiiksa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/gczmomfnr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gktlklksr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/galskezcf.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/grdmynvxa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gmiepzphy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gmcguzbya.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfemmiakv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gyqmfphga.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gvjviudld.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gpxourfjo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gxciwcqtu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gtngibilk.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gxsknosba.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/glmhqdamc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gpwrcbdmp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gouzjzdpe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/groozhxeo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gwzbalqzc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gfruvkhin.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gwbxscfro.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gthtkmivp.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gdpiftnek.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gxizrrvmt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gggsvvsmx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/guupxzrzl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gmncposgg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gzjnfrkge.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gjnacmttm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gxxusvdbr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/ghvjcqiho.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gyeiwkgzs.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gvfqvbiqr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfuoduhbs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gjkpymqay.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/grxciqhxa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/giyymhdcv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gafkkyulx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gywkrefju.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gowmjvbmr.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gyfahsrwt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/giwxmrrmi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gwuziioee.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gkxqbqyrv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gujlztuac.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gmxfhbkoy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/goobqgurw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/ganhbgvpq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gkyxldree.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gkwcskdfo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gdpmswlcn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gwtkrmusw.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gdwazcbwm.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gkzpwmxbv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwfuknebp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gndiojvll.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/galcsvtgs.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ggtgfowwi.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gobcgroej.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gsvlnzknf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpknpoose.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gxcoihuzz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/glkephhvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gruioczko.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gggqyqqzb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gdjvppwzz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gtjznsaaz.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gwagxpjxp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gtcvsoggb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gjhxjqtye.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/guqjzyguh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gklumkdlc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gfudfazei.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/giqfjnhbr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gosttpxxn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/grzrovpqz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gohhgchbw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gevmifwyj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gxxdigdob.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gqqpfqbkk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gbkebfvyt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/ghyulfkkw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmmtcth.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/ghtpqaudg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gmrhtmdrt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gisodzcvs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gztkfugsx.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gjsdltmsl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gttmrhmhg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gybmjobbr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/ghuyxgvln.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gwlkceskl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gsbqexzwq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gfcwuahur.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gnnhlvbac.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gssdafevo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gbovtrrvu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gipujiryq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzaqwdkfz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gdvmcnaux.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gchtbbblj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gnxdusquj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gaxnbfslq.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gntipziws.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gorszxhqe.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gypcmptto.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gtxpznyjy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gisvaylud.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gtruipded.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gwvlvbnbl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gqivfyeat.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gogfvrfzp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gyettslhl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gzxkauaxg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/guxcuekbw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gmpqjvsta.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/grzaedcam.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gnyqckrfc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gsecgmtdm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gfmxcumbb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gwqrotiqj.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gtntdlwzv.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gqbhdimgf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gpdiojrcz.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gzmirrfke.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnvwetruk.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gapclwwqq.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ggvyunxwl.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gkokekabe.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtlxwyxtw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gqsskdqpx.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/ggwwkaqzf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gcdzbxjva.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gdpjtussk.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gdzqhjgbd.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/grzmslofr.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/geaszsjcn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gqojhlvlv.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/getdczscr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkvfrcjip.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbtkgxpop.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyqjygxuf.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gjtmsbxlk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gqorvojle.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnswxdtsw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzyqzaarw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gghtnecuj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gikqkbhmz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwtmiolip.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/ghwmtbcdp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsuntktzq.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gbdkxfhsk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gidkxfksg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gyvjoitnp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grcodmojn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gyenqxyld.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gqisalpib.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gmkuztiau.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gamfencaa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gzfadxhpv.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gkawobcas.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqqymrv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/giearxzkm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gozoazddk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/grkhjtmzo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/guanezybc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmyqowj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gjpqocfky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gycrrujgf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gialxfzvx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gdtbcgzwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/giekcysku.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/goorsiuiz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gxvtkpwox.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/glrbepfva.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gkhodvrvn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gsidhuznk.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gxdvjxhfi.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gzunsxpzk.sHtML


<!-- 参考信息 -->