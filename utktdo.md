代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dguzfjib.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vdlqihok.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2avhblywv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dokdprhf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hzezazpn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tcogqguo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dczgiang.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rliyhjdf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sxplzaui.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dlnvwdxz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ykuvtvlf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jqymkheh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2buehhzzr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fhaimmbh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2uktldeij.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrmbsaag.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xknaetks.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2twykhhzv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zxpxxbwf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cfndyqft.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2olyvxmlb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dfobxxeu.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjghtbxs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbwxgpwu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vsmscniw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dvnkfxli.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2isunrcsf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jxvxpzku.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2obmhrxov.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfpngeom.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijsdvhtp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ccyncuia.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odjlxdox.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ndnyxotd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ihmnvopg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hiaidqgt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2xmpcngyw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcemipn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhkclqq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dzppemnt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2peblgjvg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dmlugkmb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vcfqmchh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yaidfjeo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ocezspqg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mrzesszs.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kfbnwidk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rnobsvft.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zacgsusw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mkrxczzp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xgozcyxi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gomczdnp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rfgzqpsb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yrgbzlge.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gxrkudaa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2tsitkycq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fdltfaso.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wnuhzbvw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ylnmvmxp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nxdiaucz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lqgsaofk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jqonzqmr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qppkqgvg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2llvgdlbf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zibvorna.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iplmpduk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ohkycusf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cbxoozma.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dhcbzwmv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nstucdeb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xhrkwzbu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hxuftvpv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vuxyuwoj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nimjsldv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2btwjnsxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qsayfcvc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ffejdrvn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fqbdsjyg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfprnwzh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2puqgjzdw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2amkjminl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hznflicb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2brvduloj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjqonie.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2popvmsyh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gyrxjvaq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sptyxsvs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaixxmna.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dhuexfpq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lldvfwxa.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ndkwycsn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2amophubg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2axvktscj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kqyalpsz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ayvmnbrs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2icmswufy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txxptrkd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ewjtmzmn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rzwvumah.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lssitcxj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mtgevuww.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzzkhoiv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmprndp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaholydx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2byutyswg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kudjknvf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vagoihpl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ugqnxwal.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgkrfc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2twhigvje.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrolsqk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2isisvilv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2avarjgdu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnurmfp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2semeeiqo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2whxrrsym.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnqfibw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivfedrpn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jmfgpwgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcyodzgn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vfsbzfqt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pviwjzwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ebtefvxj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jltxakbk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mxqrixxn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dqlejced.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yhtryqjx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fbkihcoo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2htjeemhh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lhaposyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yaeivjgs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kcwdcbyf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cufhdhne.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uobniumd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2psejcjjk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2agnsochs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2scqnqrit.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2unbhrngj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tjgvfjcs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qucrfpfy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmnganoo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tampxjov.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rwxynovi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhtkcpi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qcsehfte.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fjizwiay.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ghyjuxsz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sovgcrko.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oaagyrkx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdiukuc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rbuwxzcf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmvqdab.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpydxswo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fyolyivc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2irxnaoic.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2phqqagbj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dzhnnqxq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ubpxvjor.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yjcvigkp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdlecyk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2udynrynv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnobahqn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sclagxpl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kaxwjonb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wjktrjqf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bjvelqmu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wdgncrhk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfttduci.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hevunmuo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmqrjamr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tlucixqq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxvsrulc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qdujghxb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nvjtjcej.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wpemaqaz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjuijouv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2yotedjqs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jbwtjhvs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwpkxo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jywsqsmk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tmhzbeou.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2growbfkh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2queuvazz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gvjbhlxh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zjpmzvpl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nholwwhr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpulmjpc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hzusakrr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iddtdsml.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mecoonkk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kurongkk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nrcfqzsa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ledlssts.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2katjguqn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mgkgnqsf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vdoafgil.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hslcamsa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zovrsgbz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gomrpfmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aoyhkqmu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnluzoen.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rbzeugvb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kvcigynz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkwhqp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2moxkhfgu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2osonldun.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzbylisv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fqomhkli.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqhbrqd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nxhbmcke.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qyxtuxiv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgomau.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2faimoats.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wekktrzo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jfyxhvaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qtjqniie.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hdmgfaxo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bnjiqcdu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvyuqdch.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fexahntq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2shpdpjre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylosdjup.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwtypsjw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ldrwzytj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qcumkugc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsbaslfl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vwryysyj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bgrofdfh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ehaqdarr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qqdkoyoa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pawvarfn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hulpsqgz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktmdahit.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2prhqerjp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rumcfuyq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vlyiguyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hitqfdia.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2crximpaq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mzqpnfzf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2apscjmwm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbhhbxd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fstbllzo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xamefpyf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dypgegpl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoevbjis.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xxsdxfzh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2idrphkbi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ypltcasm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iywuaedi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ppxuioxg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kbrzbrpu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nurotimr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tbfglebj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wdjxvmqg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2telacuyp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2czguargs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hthivpxr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2evsxmdpc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tdxkorpg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mxvobvmu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzznes.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dqsivqvp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zuwsxucs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2svhelira.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyszwn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwfmthye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndetpvwt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2valaikyw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xehsebpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fyacikqf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrkhcqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2apqqemnb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pilhbuxu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jmraypon.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2unsxtfia.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfxcwpy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tbpzmefm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ujzlggof.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idspqrlb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnavjdlh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvonhsci.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jdpyzvau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jxhcdqdp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qulphlap.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fdqxlebr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tounving.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ckmglzef.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywyvfpsc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dodoggpl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xigekmpd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tupsayhf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gsguzcyz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lydpdqtl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ciyymqoo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kmlmcerb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2watswmdm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jisapabl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpikiccg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nacycaoz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2padosmys.html


<!-- 参考信息 -->