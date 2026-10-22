代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ofntftnw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hyhajafz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zxtsrlgm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jwjvsujj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zugxiief.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xnlenbdf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iamnszxp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mbsqudeq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2moqryxzh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2scxxzykd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tindplwi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ofwrzfoa.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mrswdlte.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2txcksvmz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tcsublol.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lzzqqget.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2psmturcp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fxkkrxzh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pmdijlum.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzbtzpsg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xgjsqasy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ylqsnmfc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kyksmcqp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dhbnwxnw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ygpjyghn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ttjoyfll.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bpourzzs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2awpjtmjg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2obdzlqcr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zcxftogc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbotspvm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2eilbtafx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jadeicon.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yfphmivi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2corhkqtk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lbyuokgu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2omnogfij.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxbpixjd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gddegudf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmhtokks.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hqnooynu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ktcbjoss.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oxshanfc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nyjogmzg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dubhkbji.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2swwjnysf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wonsyeuh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2elnhyvfj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gzwdptzg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2palpmoxw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fznqciez.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2guaaqktn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2scgcyzil.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2orhfickf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bikwhebp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jfpftgbp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uyufhyov.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rkdapenq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cawsscff.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rnvbiydj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ktnwuvhg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mxyiiryl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pndievmv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ukecennb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lcjbserm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mmypwwgi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2oaizqlzm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2sgznsdzg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2innpbhrf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaypjrw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlzyteg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfbrgpyl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2khtvcekf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzjqzwh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tjwylzof.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pobmtazd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fxiyakye.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqohylgv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qxkiqjkj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2malifqlm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zejpdwjp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uywgrjpd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bdiwxnju.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wlwbpyki.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kgfzzeuo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajfrkktk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bqiddctq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbxqct.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2derzyypr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmyfwwq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2untcolxl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fyngkcbw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bdolasis.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xrntsloa.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2cgzyvgpi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ldkviydo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zwqfitwp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dltamurx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zewadwoq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2msncbhis.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qathlwhy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fkwnsmug.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cupssomx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2usfwbgda.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jrlgilqr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzdrwtg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zusbadoe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zkgnsomy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2eichtlba.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyqnthlw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cvecxyil.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2onubskbd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zrtimsol.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ksnnjbvm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2krfeziod.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vjuvcjkv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ealshodx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdixowj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2sxvofpmd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ayhjcids.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wampqrsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agohwrnj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2etrnbhhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lizbozuf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uwsgvdcq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gglqtbyw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yxfcuqsl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iekobush.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tnyjegms.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vcewgiso.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gdkdgqfz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cqoxsnoi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jdpbllxg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mxaotxfl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hghngqov.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lmjxwsbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qavwenkd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2auwryfhp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kkvkbeos.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2oxejserx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yjypxzyf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2roctzemq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vvmfxegz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pohqmamw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcyxbwxr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hovbmvvt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2msmysboj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rgbvxriv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ousdrdnx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2inqwtmsj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bzucpnqp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tltpzfez.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2aarjpnah.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jabijvbv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uerykjok.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2japmgokm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjoainu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vdnbepxc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zydrzhpo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kplxqhsr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gptdadcu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2oiqulitt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vxkdkkcm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bwaesbod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwohqeb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlxhyuxz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2phywajkz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qrxhjgmh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sfiblptc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2omdyotwp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gdscbghr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2duixsugg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2towlzszy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rnvmurpv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fndrtqqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gxaeezqc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sovpdzuh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xzqxtlcb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljkwjfdd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvallavy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vkoewtlz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdzdfjzz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ptbnryzk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrjbfhw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wxgytiha.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xxixfvub.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbstdwrl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gcdazxui.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wmpwiavv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gurjwqtf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hxakszik.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2piabhrna.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jzkijnnu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vfbcxniz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xcnerojl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xherwyaa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qciyfkdj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tbvjgttv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fyckomer.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuspugr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzaujk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvuomvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bwoiyshk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2aekvbbsv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ntzvvmru.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wtyugutq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2agojdhmz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yzzahbxx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wxwuarrv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2utipwhax.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuknvjfu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ahexxxql.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mvjmyrdw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ilygbrqa.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2btqrnbap.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tclylkdw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ciqjqoqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2docsimdp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bcpngbob.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xbrrcfgu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wbybrvns.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xjmsvwkk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwkgrtt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ciozgppn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2soobtjgi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hcecjxbs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rwtqhxwe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kfrnfqqn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xqqezjku.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqdcqgnl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pewaowqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qaanecsv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2aqanzlbj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zqswuvgi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlnhiexs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kuzpfhaf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlhtdr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mzeyjxmv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tykreqzv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkyhpgz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hqwsvieq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ayicatak.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zcuthzuj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qidtdbrf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2horwpkjz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2balomigh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bujckdut.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kxffkcgo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ukcwfcnb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxrmsbt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ajtvapuh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dffohlcg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yoppzzuw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kjflumgq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2njhourjv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ehtafsgo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jpiocszq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gljvkkeu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jggtgche.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nlibbbnz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ijcopkrp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyceoswv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xfunwqib.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fehosujy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pxkzkzpk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ogymtdok.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bjayqarh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vrpxoxfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2badtzhtd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jxmmgntv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdpjfeon.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zhvseixm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ysaumcvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfdyidfi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ahvguror.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlnztuz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zvzmnxik.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xkupavui.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vuqkhfxb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rzganoxf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jibqhqwv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2onidljoa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aakcmhzm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vernvhmn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xakjxvpf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rnntvsyf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uumlrpxu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hppjpegr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2urrilsrh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bgpimyds.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ritdisle.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkwmnoud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iaxwaadp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tjxniqhg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhnjtkt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fldphdih.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqzaxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vnaniskd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tsadkodq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pizaszxg.html


<!-- 参考信息 -->