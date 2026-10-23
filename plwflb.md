代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xpfbobzt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bmhksnzr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3augfotgr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cbetvzqv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3suxnmfbm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wxsojgqo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vmiqrbqf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ptdtgrrp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ohbprofi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wcmquowt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hulmrfig.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqiuukt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ycvsiznj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pixnrybe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ozkmscee.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3efyxebrz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3fdnfwydn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vdvpnfpw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpmpuhzm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byumxddp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3hoyeddhs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3trxehpho.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbswpgmw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3npjbrrzg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hdbfjtyw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqammpmp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3juxsxtzg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoebjlnn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mbumtzdc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mahgyney.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dscftsvv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lodezfuk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gphmgkqu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3myvoaxpz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cwvlojes.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3thetqoec.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lrrgaelz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3grwtvjkk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fuybovvo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3eesnahpb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jjnjdzxv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3eucpxhwy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rkmclmwk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3shlysuyf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hemtnhil.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vosjubut.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3gozzsujd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rxhszsgz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uyotpbfp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hfdybmec.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3inpzobgo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3brnkevgk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ejvpmgwi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qltownta.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gawykdsn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pujqteeh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kjoasixd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ziplweem.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3uczbeztb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ekxfykym.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wxgrkqio.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3teoqizhw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tgqckcub.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3maxryfab.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ikjieiwr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wqrtojmt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3evwmrndl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xjmyhgto.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vndpinvq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qrwibktr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nefihszb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3myiaoksi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iggrsrrv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mptpljcd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moieaopx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hkxwnlbl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gupdvojq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ysjsemou.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nvavotcj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnydxcq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3knikmkzk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nnxzwabs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rcfvtwzn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ygqqosqm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zrvausxd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hzritjrg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3quvhqpsf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3eoqkmfpc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtsmerx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iwvslxfd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mwllpkjw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fyimgjvn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hwmhlhku.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3krgvcvbp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zanhohgf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rlcxhrgd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zwzqvnrg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fonfsbwe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuhcxzur.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrldtq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3znrlupix.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfaahyc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mbwvgjsu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qivusbfb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bepktmxi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zfvtqxog.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zvrlrctp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rwwitras.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xicnnctw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hcpjkxza.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhnctzpv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vwbhaylm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3illkwyal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbhcqaqw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jqiugjcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cellphyl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jdkgjcfz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cgyloims.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlaijlpk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3czqkbrlz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fupelaum.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xqjuccvn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mxvybwsv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xosuclvt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mtkjebba.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jbdzaoou.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rsfytsdo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrapfcy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hqxsimmp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rclxxbor.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3imgvjfsh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ypudzjbj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3oaqmklan.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bhmtjvtu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wunqyjce.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mokdbrqh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ysithesm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfrqferi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fbxerpad.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojikfykm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tpycufms.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kcrtskgs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hciehjqs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvwkiwmd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3felefryd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfxxxpg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3isvfwbab.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyhxevcv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuibhmot.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvfqzdvl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yzhutini.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3sribfcdc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mxfvwpnn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kjffjkal.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3quyeuebj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otmwbqpi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcsgahpn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qumicmnl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oewhjaya.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnaxqvj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3plctqvla.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3axtlmpjc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwkdgxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yioqnncn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpyfwyws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuvadjx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3scwaoldo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwpsqrze.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdgkaqap.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3khxpygix.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3umdngfar.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nsqsomzd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bsveujrf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eslirkfm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuekwzdl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlnfzddr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ovnrkncf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpqcpluq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqkrvfdf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zvyzntzo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yshnhjfj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfcxbln.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bqskezhy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dbjoojbe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dsiieyvw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fgfgzjdh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dilqjcxf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eemqtwop.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ycjeienb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rzqgmxho.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vabmogwg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpaylsxk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtcfibed.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tsgrkeza.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jbcwkzmc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zchytugv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxlsdlhe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3sxsjjkav.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3otagpxll.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwqqpi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qslkyfdc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gkibxfwm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3iwvljmdl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qktqmurn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ukllvams.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgizquos.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zwcrsywc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3osqewjsk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3amxgjvav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndzxxugc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xjqkmwvm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bemlpfid.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mfxnutpp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3obvnvlxv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fmabhveo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gyrvevco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hksqrfom.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lgxojsfw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwepeozn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3brnevcar.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zaoapbme.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3azwpvfyr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cvcopkih.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jtmhubnm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3btbdchjd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oqnvxott.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rfoifecq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfirsoto.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ufqamanu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sjlraqpx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xdljqbcg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bxkdjibj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fzktvavl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3sozjdpqy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3obaladqz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3chlrzafm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ugnqdpvc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehkawaqz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzitwskj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3riymtbtk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bbtfdkjd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rnqeshmm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lbsihmhy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3keytlvav.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qrrrgnrh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yhmifvxd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eolmkgsc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uaxaylcs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cowxxxgf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zjdlpady.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uialcxcc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cxemqcdj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hxyydosm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxnmpps.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rnaycdmt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zckjvuqp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cwelpsqk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tqzdkumw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fuogtoas.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hayabhmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmwaugtb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nmrvxnrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zacezbae.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3diiebhiu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kwcujxki.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xrumzivm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qtsopmev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvlepiid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qplgeubv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tstswmdp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fywfxfsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgppkkjd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pspocjkh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yrvkulmi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kzgzlecw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewknxfie.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vziiuzem.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3taltsmmr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoxrqhju.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rvqnjfjw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3swdzxfvh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lsnkwpth.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fhngfwod.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qboosywo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ffbkjabl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjqzzjjb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qhxrptbd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdwxhst.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vutacdvd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cqqoakjn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebfzsadh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vqjruezb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wjjapadp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dmflubov.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tgojnyim.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vsiltbzt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pfypjyrf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jtpysnps.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bvbdgcor.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nqxvurza.html


<!-- 参考信息 -->