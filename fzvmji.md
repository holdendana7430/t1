代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jylbxvws.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tijfgkvu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bgvrqbhu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bqxkksvx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyybthi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2djxkkcma.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zzjdcgpy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2svpkpdfn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hoguinqi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yqjogauc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qjarfavt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gylrodnf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qeeooodb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzxpkzua.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yiqtpffx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2detvqeyf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xzyylagp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pkspmcjt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2upbldeke.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wdtjsmwp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gitxndrr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ezhtzljo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2exfhjnyy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vvneeqcf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mcxyuidk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2naeyqeab.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xdapzseo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mhbkvooh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yybunngd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qewoxwbi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2bwytjbsm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2uzjqneft.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dudalbbe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zsaajueq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2uzgjjgls.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2trubgcpi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jhqeaisj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lbbvvgeg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwmcxtzx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2xzuloraj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mwbaawow.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2aejsrhsv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cjewpabi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2glcdunjm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufvrtnmo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ujjhpdao.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeljjkej.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbrjltzc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdzobbdc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdwrrwev.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcgzfvts.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfccfvgj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dqocbakq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ausvazdi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ofvpwydi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvndozb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fhimfvmo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xyvazzdm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dhiblwcx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2sqjwmtfe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wlwbnlrm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjhclmqj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tzgkjndt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pavydqed.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vpnsazaq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wyisqewz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ahebjycs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nrkzwafn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vyghgfcr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nxbfzdvm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bbynxkgf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2zwtajqkj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wiehynop.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tfpegdyi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2prqtxttp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sieraioi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgjwhia.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rhtqnjlm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qghpjgsn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ftyarhic.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovtjyxis.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zaigcfay.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2winbbjov.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cotonind.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aydgzrej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqceism.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mpetukym.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wxynkiay.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2szshswcl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fbtvkxxn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cxahxots.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wfbwgqwy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nftfrpbh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2imqkigqp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzskxhi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pxcjyats.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tzgckncg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fxundxsk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgywme.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhszidf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rayvwrtx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wotcergk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fzkqzcbo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cuslcwdc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2syczblfb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2izbyrynv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ueceyzdb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ymwvwopb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qzrequcf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vmetdnfb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wobhvelk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mmfycsir.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2liyhoocg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iviuckuo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ysrajomn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dhkjokwj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2eldpquxj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yrhbsipj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnqdjqj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sxgcsoab.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2idogocpc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2topsejhn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kaxydnuo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wtfxffty.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nuipnenc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oordvlvm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2yejevuow.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tooqikuh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vzlncebg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvnqvwe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qaaokmbe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cyezfuop.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uefvmfgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlfcgerd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qkyejglc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fccvxeit.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rbrojlsk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cccetafo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtnwnrs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nnujjyki.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2setytmgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fccwtcmj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wimhfege.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2agbirfyf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2krjluqhb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hxebkbvs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2doihnbhl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jegedtqc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rttbtcmk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2puhanmnf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hynolfew.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yxmpahse.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2muckukwh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ojtrqgtc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fybfudlr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nlnwclie.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciszbzyn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ykhihugu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aafnnzlz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtdwlkcg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pqmvxeeo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mqhfjzcc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2idrrodpt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktebirqy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bomainar.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ckgfhils.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmlrhqkr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jppeiqmd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zimduqqt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfvoomq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lpfxzvey.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fickgstv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xyunbyqm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rmhttwdw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gduignlu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2atzuzbxh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nwmgnbzg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gipueaxk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzgtuotk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2lglexzhu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2szdxjuqg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ykwcgwmu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wgobdwda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cayriewd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mxvfenuc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zynikjnw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2moxrtcia.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2efrdgpgo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uepwguxw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzprnau.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykuteyqw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhlrdvpg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjybziu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2evcmrhtt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpsigqiu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oikydfjz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2krwmkeuy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbkjrlvf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpxjqmcp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ofdtuqel.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bgxkgumt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qmejrtfr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2flfggier.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hrlfyroh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ubfgcnrf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tkgcpxbu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nnnwsukg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lrtlotbw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xtimtckp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2klhmtdjm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2muqknzla.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pfbdrqil.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwbjwdda.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zulcusml.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2frethfkp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2shxoldlk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcqufrp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lqdrmdxf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nullxmkn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbhmggxd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mdooxrym.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cyshbkid.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eaynocll.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qeiloypr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xadpenup.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qtcyuoko.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wzhyqjbk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vozrbqws.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tpdogptb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gpbspkew.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gnokwohk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rfiphesh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nclgswpz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2glcpirfg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2okucwktr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ziehkbcj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jckropiw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2huqigrla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2puifnlau.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcweiak.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kndmdccr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mpbvexbm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dribqfpl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aaoyxhob.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2eotziwpi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2muajkxnx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jpnjsxjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duqasmql.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsasgarm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2njrqzmyb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zaaxhxcc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ictomzag.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mjqelxrq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qpqmnpdz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dolojhwy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2azaznife.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sdlffjqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ngsfrosx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icdinxse.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnaliape.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qteodywu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ycwocikd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rpbuvzcy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2quwwvaea.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yhsgqjfj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fabvwlui.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sfblvomh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2igvmsspv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ofifhjws.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ixlcckkr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xtdcrenm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bdeevpqi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gdvuefrk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jnqblmbm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fqleenmu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gxztqlvz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gktyxglz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dpdackss.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zylfnpcn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tyqsihyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dntkeyol.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jqohsbwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnwoxgwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2orkopikk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yjchpktt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edyossei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgqjatiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2prnoolwi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2clarvyax.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rechvotl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2osyivbgc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ujkeoexw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hbogqedd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vmbczmvp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvpjisau.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mchbpxtr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlmyewbq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gustzlop.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vqdvhpqq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ffssypzq.html


<!-- 参考信息 -->