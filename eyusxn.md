代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jitdwcuc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pxneeial.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umwktyzt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dcabiuyh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tqhomcif.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jzvmdnny.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rrpiihlt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kwysrdle.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nulqjyue.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2dpofuuay.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hmadferj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wyxmmimf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yreltbjm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qlvdhrrn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qanttast.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xhwwrklk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hnurkeer.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pnvxsgkm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2adobefeq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2refcowba.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2raadqhjh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sxpriswy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xnhdqavg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ldqopkeq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qgtladgf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hmfhgztc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vschywpl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gblhevzb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gtqtlagd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2sfelionq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fxzyhqar.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ysdgwurn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rcojwvdo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohnwrbfy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qinjcnkr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2prhrkvje.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tglslock.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ezclpsyi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsvxvgis.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vhzqqeab.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2nqqtfrzr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qxmjhwba.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqffcsj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xpruqhaz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ntdpmcbc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rrybnfhw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xtkmxsnu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dekhrosd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2oxalieaz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ebjalbwn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fstcffad.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jstubloh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dtswwbho.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2onzmkmza.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bueefeux.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rbunduvy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rsviiksp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ucshkqmc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gptnzsvg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2inzyjuuy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kgdqripp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2srfajbvp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2asnfhiye.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2olhusilg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wraoyvrz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2sutvgczv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2zfhbxkfa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mrttjbyg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqhqlxdz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ehhjozxf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2inelmklp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eqynunhr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ktagomlo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfhmpwe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjular.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hbxxcspc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ldrmcnrp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egwwmost.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2trlmolem.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2npxyybct.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2glishlmu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2goewgrcc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hxlizkcy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mkuxnque.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pkyfdihn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wybtvewp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2exzewjoq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjsyfjt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jiuwhgtc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rboemvlt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oeisllpy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mvrupdbu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mcdrhajt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vaxooztw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2csmednsq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2cicicmol.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mndkyvpj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zzgvpohy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2phpnocty.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lrswuoxx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2oxuzosqw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pfoovsfq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vgelgonf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2upoepynm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2osrgfrcd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xnkgrjfz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tsxjmigx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2swhjacpl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ysxlitja.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwnjznlw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gvticjyd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hcfyviqf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vewlpoqt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qfrjwtnh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jdztgdhl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aoxpplol.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vgrryjel.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rhfpeahi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ozgbisvf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uelsdsos.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dpzkbqkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecrmtfkp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2knxrgaqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psgqwwah.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fjobeuxx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ibwnalef.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2djskrvje.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2othrseur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2belqvpva.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vcbqjmhp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jxmwqwtn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jnipnqjp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cxqiidnc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2iedpbtwl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dzkdsxts.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eonjrwgc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ktizmpvn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tcafsjpa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2stsqrjcx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2odghhfou.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fooixttr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nolkjcyx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zdsqljzv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ladlhzcg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jncigwkr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2suwqfwyx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sgcrakss.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hyeqjzqp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uwcmpowy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cowkctfy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2flwgeclq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qrmpeonf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gearzfbo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cjndrggb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldybfngt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcdhgtmm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lldztrch.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtsauc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lhwvzngw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfuiiihp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mzwgigwo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mjykshkh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kpxqhvkp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdrzbzsb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ghbsqpnk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2pjfwdhga.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nupzjtwx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bpldpxfn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxxneuq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2eejxxbmz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2epgqkfzp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cyghapze.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zgfhrrse.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwzeqici.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fomynevp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lobtmsav.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2chmogjhu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oabqxyhg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvkbtbly.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2egaafpeh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zukeinrm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nnqqlqke.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jggxshzn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjtibnt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qqobpdof.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ytfxzpaz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyfqhsqb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2sjnvudzk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ldmxvogo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iezsoyxl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vnptoisc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zvadjkgf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zthgvtun.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pjkxlgxm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gmbdnadg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hplyisaf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwqrct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gzcnfywp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tqbdedgf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njxewohe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsoordr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wvjdigeg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhnwihn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnbsqsp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sksehmhb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uhxnniic.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2knxzyugx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klztsjeu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rexhivsp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cheozfni.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrqfugld.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vphkqtqe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hsdcfmoa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtyeugff.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vhawyqxb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tradneao.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nuxnprth.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ngfdsobm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfntrrgg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gotpppso.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nxvfihhk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ykpldbwr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rebbsoiy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ljcfexoz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2novrujxe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zmggogfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cpwfbgmj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2osrsidao.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2adsqoqca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2csqucxus.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gazjcllc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gizerwou.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2srdazjam.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzejjq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yletcfki.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bweigqwl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wgyrhmkj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qgjaejhp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wssacwfk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2shvtkrgf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xrwvbqhl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2pzkbsdxl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2swqyyysj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2aolitfrv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vazzkqyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jjkhuppf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wwlvwpff.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyirgvs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iounriep.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qixkrnzr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hpafdyum.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jzwwsemu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2geqevysp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bwqwucov.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2drccmmur.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yvigqhyl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zrbtwjmp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oqlbrqhr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2smdimsby.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2traredzj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zbdjxqnx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqlvlzdu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2edtupfsm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mqrixztr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wosnhove.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ktqeqigl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yctxrmnf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xsbmagff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrkfozev.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bzfkpnol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovlwbzxd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjmlffcr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qlrfzgfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pioqhfqb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bxbjulyz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dxhqnbtm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndmoknim.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ljwakgbr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2darqrsrc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwojevyx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oazqcrjw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ipnbhowj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fufsbtvw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zgpszlhr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mrrfpmss.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tzrvdkjx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ofolonmg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ochywkkb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jsisloqs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xhbkzedz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lkksgqow.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvdmuod.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqofwcdz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zbnhxauj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hcjivkcw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fkrxwyrm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aefnxuth.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2apimrrtr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ebhqdxye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlkkndvn.html


<!-- 参考信息 -->