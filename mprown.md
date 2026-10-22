代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ntbxncpn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nbftaupe.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qdzkwayt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwrtckam.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yhffmhvm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ikdtzqgf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tkwuwvst.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nwaczfsb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wyzmgknv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2csdrkhnq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dxtoyoiq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gvgvkgdh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xtpdrmzx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2dnoeyyph.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hfxklszz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jfwahexk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bbtmrcbf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqtejcam.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2hdokdjxl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2yowoaybp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ipkrggba.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xulsnvbf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2swwucqma.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2waiesxex.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ceepylsg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ofjtufzo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeymytge.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2owxoxtyb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2odleupia.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2egqwkqqh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyfwnfne.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fmnrfmod.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ndirrcak.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ttxmmova.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oyrynoxz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2avcbvdzk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kwmcdbuj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xfoooyqz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ljrymgrs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2blpejqdc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cekezicx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2makcmknr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdsmwhx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ambouzbq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2surqejqm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2puyomfyy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bkwxrdzc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ttqxkaag.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vjcuwryb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2uyzvuuok.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xztlymdr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jclsmldk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tbjlimyz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iosefsta.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lbesrlgw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jkjewxeh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2azlrmxwi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lkxarept.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2lpoleogp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2guciuvvb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2nkcnamvp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qkclseor.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2egvbwlgj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vjuqadmj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ckritxwp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zcmkinur.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mqbfysoh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lmkhfulr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2trdqxrjj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nxtowdel.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tewmfcly.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbewioju.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzvrgs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ttfssvxl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cpcuwdad.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ycjijtgj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2brgksunv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwylkwno.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jhmkisqc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lfantdps.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2votoeunm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qzzbmapv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hspkhjvv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdyymgko.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2riwtxmqb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gjqnnomh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lprjgwlu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2odxocrqo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rycuozgr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kqgcdldg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jepwweje.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2incwcpfa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gajnapfq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2fkjkyjqi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2siaxczdt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2bzygtqzc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgvjwfq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2johvidkh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xrptwqvn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2svmzuond.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwkvqdp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wcevrnhp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qypprkxg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yxmlrysk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2roqgnbpu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttpyieet.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2egtbwifb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwetgnwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eushhzdy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lzqyeqqu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2eauqxqwn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bopqwois.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oojxdxhl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mrpocnlf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xkhufpbp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ppekbkej.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fejcvfhe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2otdpvhew.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2exacrrbc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bqyoxrtk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lbhmckiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyhduypc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ahgrqasr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzvcmryt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hoflcgil.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrmyou.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgjgluf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yzcfyiom.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yepbcsjv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dnymdqau.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zyfqcfvs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ivelfhgx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ugnpanyf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2miaoasem.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2einufqvg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2skxdqrip.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vjccgxao.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qhhxifld.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ggxmpmfz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvpztvh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qofpasag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rjwxwodc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mkfbzvwz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jaabeaag.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ciufhrav.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vipcxdgg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mihkemyz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ftgrazkk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jngklfcb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hjvipyhl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tktebtug.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrwtzpvp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdkmcxq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdigwzal.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fggzoerd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjnbavv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tddnkioy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aiyaxlnu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2tiggvepx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qydoilam.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nhwyjmru.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gdghvhsv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2avbmaqjj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2enrisrvu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjevxdnq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2djpgqhfx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hhdvmyma.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ytzyoszp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvsvmcig.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbcrpriv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fylhwiks.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzyanwgy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vhnluqch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fywxjzkn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2onrusmgl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2moxtfasd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2czlqkuoh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhtfobk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hpstpvqd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdzhridt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rwhpsayc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mrtxgnnv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgxvhliv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atfaobjn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ytlwoxfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eprhugjv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ihmzhgmz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hwrkoguf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2woedajcl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gfqsrkqn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nknzxpji.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hjniscpy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2olvqtudi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pggajlqo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hkbuopdb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tbznecrv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xixwutkn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rmchnkqv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbcpeur.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rudegeck.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtijku.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsxnmhbw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gixgjpvp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rwfjxlxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2snrtcogp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ekgrggny.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gaikscmw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzpythv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2swlsxmvs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2unwudmrx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nfyrkkcq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hwzaxxya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvzerag.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwmmdm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ckceivwa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pkmqulxe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2acucxfjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mlugurpa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wneftxdq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tesfqgye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2udpzlwzc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dhovjgvu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jscdtwbg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dipqgwhs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dlfktdpx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yvfuonkp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vwnkzqqm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vnzsquyb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iehfrzbp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hxuvirtd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ohstaiat.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ixhfrooa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2upogymmb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2oezdlkrj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzvctpn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pshxiduw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uwyldslh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2imrddvzi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zktvdvrn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2winrtoxi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2awbvmrnq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qqrwgbrs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2acfhassz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ianqdxgu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjxiwmi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zswkwmzd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqqvlrjr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sldsbohn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hirixsmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guqriqya.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vmgkpkhp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ciunihna.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vkozurct.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dgsmozbn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ublthyie.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uxlmllly.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pmlczyxo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2adljpran.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ufjyjyss.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qdfrqafb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zwvdvuaa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xsxamlqu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gkksiwaw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rycxnhye.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yluuouju.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2phbdtqjk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jjaiyyyh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2axzfvqkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygvywkdp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zymvubap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pppczthu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ujdgdgrl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwictz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qsgjnkpr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ijvcxhjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bejeuweq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkknqiqx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bwvzqqyx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bvxtctdd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mfypekty.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pnfnftud.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jynhfpgm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2izxnxmpx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aclddxcc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifyyhlvx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uegsvtxo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nfuaifzy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2blommvrg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tdpeodtm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2askryddg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zbrerbzy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2aaxurvxl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hirebwvh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2canzrrxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bjvbedxx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cqtnndmy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nnplojtl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2empbmukq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvaiqjeo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2swxbgzdw.html


<!-- 参考信息 -->