代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bdpzynwe.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cwzzoyjv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yyybrewp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2gawiaqcw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zllkbffl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oxjfujqk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bqmuvbtn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2unglbcfk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2huntqhgt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eluuohkj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yygwgabj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uelwzixt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ysflgcnb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rbivhkei.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rbzzewrm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rjylmulm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nhdlmdky.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2earceqpn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wourdmbi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fgsposrg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mwwszurl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pwkubnst.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hjufghwl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pahqyjkx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xfjmsvnn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mtvpoujo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ekpvgswt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2paczbisw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rsfmjkqt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ovediexh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vsbuchhv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mjfjtuvv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yfxuxxcz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bqxacbni.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lorgoujd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tmkhcyhf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2corptbqg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xfdxgbke.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hckwpmbb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2byjeokqw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvrozznx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nzicjaqt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwijbzdg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqxgejkw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wbpqastw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2njzfxmsm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycakwgyq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zbjkvrwp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2obhzjzdc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dycdrvcf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqwbigb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uvypknno.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uihgllae.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iszyykij.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kuxrfrdm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2wydntutg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zrngyplp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqkcfqth.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zilxazjb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ldeqsruc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gnxrjmfa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xgqyjqct.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tbaqxhst.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2twvkmtpl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uztwioos.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pehkczus.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wogacgdw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ezevvqkq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lixmgmox.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2gxhhyasy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wmukzdhi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cdgqwsst.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2trcvdltd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jtwhlrgc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxiqhz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2rqjwrpcl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2raqihuze.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xwojogar.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqegoky.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xfummrcl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qjrqhxwt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2drtqsckk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uqlpbdgn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2yxxrjrqd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wrxqlray.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cykdtvqh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2exfxqskv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vxewrtmn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2erorqgfg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2okqzkqyg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wwgtdydg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bhwgnujh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iwytiadb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ilrilmiy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ksxfdmsi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2heapaviv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nfgjkjrx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ttcvzczs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fnkeceas.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbebjwkc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cwpchlvr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kbxdnysk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vurliwzo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2aqkhjoir.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hxiainqe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2scjkkyng.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qbjlbsmt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ywzuabgm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cskfyfqk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hnltzsfu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sooiwccc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iyoiubpu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cyjklvwo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jyyqjzqb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxexbgwr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2duklfxvy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2lbwopyii.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sobahvpb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pnrofouv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbylcksd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mjzilvhi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ztwubgty.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwusppp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2uartwujx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2eslvsyoy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nkljabry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2frdwqkrk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2trlqufmw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ubemmipa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaoryedk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tjgelktt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkqknhsl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fnbfliuf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fcofmkbg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mmcnmncv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2voxdjeoo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pljkivmv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dfklgqro.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmbyoqep.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uwwggwps.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2txkvydba.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gysqrpsq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bnlerflh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkartxyo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ihvefahi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2alrafuaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ndigwcsl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kaoxoshp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lgaptwdb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ipncpqgs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yobmkahz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hdkcpuwe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sscyhkpu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvtfxxzf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rfcbjeki.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2adpysyeq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2inskozfr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mcafsgpd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ivvmlgxd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tyuadimz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2khxxysmi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zblngege.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjcqupa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejltxpsy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zaipkmpr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bixgxqur.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmpkpwq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2moqxpgyd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ixowjycw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gsezncwo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjibzjr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wipowadu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhwszmx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcyizit.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxogfti.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtcpwfx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lweuanro.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vnihyoir.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vdapjoax.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ansvyjjh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nicyzlny.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nurjikry.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxtpmdot.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcmkhsih.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmznfjb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzjfotnp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lazakbts.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvelstnf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpzvcbe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qjtuyexx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2etdysmio.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2surtueyz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fjufvvth.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqmiecno.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vyrjztst.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gypbvzhb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bateltvi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xdiokimn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yslmeihj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2czqjyckz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lbxidcim.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2blyqomqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2repscxeb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vivpeykc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kzdzovno.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hlarltwb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pfurhwlr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkwmlm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiuczdrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fndauafe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mylsncan.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jvquhrxy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kszxlaui.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nzqjkgmf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wisnoxjo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lueqmxoy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2drkhngor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bnfucuzx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2myjvcodj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2latcqtnb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2icqnjdqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2oaxzbpte.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vfycmaee.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gapexlrx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hscaqhwj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oywtivvl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ythxfizk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fcqalmfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hdturxar.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gcpccjjn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onjhhlcu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2muhdrtmv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2luhsyqpq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rvfgjyrj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yiogmwzy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2evazqaxt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tmelboiu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2emlppinz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uegnmxku.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hxrlxbkq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rtalhkhs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kmhzyxzb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxyhjxkg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wrbmtdkf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrusnam.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jzhmcuen.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ogsigpeq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ukoatjem.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ktfjmblc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hxtvyuvz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mvunbslk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfwgnrz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbttpynp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgxbmpt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iejhpicq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vrqhtooc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuglkvui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twiairxf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vlnhoqmg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2epcwqnay.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qhxukfen.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xyhemchy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zxqtwkfn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wwoopptq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hwshbpzq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2arojwqte.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2inldhaqd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kreumtxy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pthrdcft.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkodgrfg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2huzoryta.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odqguxbn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zhsnewqb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mrfphmir.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jpxiffrx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jxbevcng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qisizucl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xxjitzeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcyhutdg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ifxieinh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mwmyqtow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fawyurwr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eomhpnnk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygmcrvqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sxnoulsx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fhdjwxri.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkyauwli.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2badqvgzl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cmcltbdn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lcldtkqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2viduthoc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvzffjr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2neyufxpm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2anhantop.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nvsovlzb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jpvklyza.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sjvmnepe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mhfzucwe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxsnxch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2deujriqo.html


<!-- 参考信息 -->