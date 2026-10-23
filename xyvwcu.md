代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3txaapuic.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3cfowrorb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gpqwmibt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3irezgfmq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cgxxekfj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vbwtwbet.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ffqskpwn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vwjskovh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3thnzaock.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mlwwlpef.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ucmfmikl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zempwpol.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xfufjhmq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gvvgcvyi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fhripsjk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xepjdtpb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nmgbxdah.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sxusxluk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3leasefxz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ctnsarsn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lxwaojjk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ttlixhvi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbpagdop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozjdqnne.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yyxrzwxo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tvqranwi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xshvsosc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yetuvtyu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tdygmjsp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcsmpfrm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3smajkwqm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3prydffog.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qlpnnkdp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tksqrryw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eouupzgq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jzlhfhzp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yaauibhm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwmasju.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qeopteec.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bemvnziv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmamysc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3widnkzju.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rmvandnv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qkjbdjbn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zexbsdba.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxzrwqhm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jfaridqd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mssshciu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gpshjpdn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3howlwtet.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xinwhzum.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3snwmvtxo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xwznzwgk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ecuhgvta.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3uurevvby.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xhuwxwex.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3plevqxcs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jcrwrftg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mkdedjuy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tukjovsl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zgnpgmfz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3jgewdujc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3qfoecify.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3leexaadx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fugwgwsx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kkyeslih.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bnepiptb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iameylhq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3scekyevx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cosknsos.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oixaadfq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3rjnwjwdd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sgrzxshp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3snqxkclg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3iifyysje.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3acjzcfti.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bcoxzmvk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ympkckjz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3idsdnlmb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ghyneikd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kegstgdh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3osodaukk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xqbrewcn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pyqiweeg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3naovdjgz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cxqwifvg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3abhjgcti.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gcpezfqy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wunxmfmi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cdaskokd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qctzdpva.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mxqznfrs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhhzwnx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vkjibosd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3suzlrayn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wajltgac.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3trubmfqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxgair.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eakigkqq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3glxacomk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jfuvcwqc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lscefoml.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ljoprzjk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdzkycb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mucskkmj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3irozhrze.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3rvuuevsk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsayydab.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3kuswreal.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xseyqgww.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3snbzkxqj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3onahrrne.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3eoqrmgke.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vxisulkq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcacjtfo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3unlhxhlh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hccixnvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahrgebbg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3msrbbjku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oizonslk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ruuuhyqk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rxspwwnd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azgqcxmm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ahyfrjdx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xgazemuz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oaowcjot.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzrvuywj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kqcjjbnj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3callixhj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ydmefecy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qahawbsn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsecgovs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tlhpwxzu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nclofxau.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3frrsfpxa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fdkkibdr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qrdsuzpa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vixgyyoz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ajnmmguw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cpqpewum.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vfxlrlqa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mvjhqmcp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpbdblty.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iakvnytr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iarbkqnt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3putamowj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jvwirduw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqnyynwy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ilvkqefo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3egakfwwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3luhoqfsi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fewmljwp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wrnfxwei.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rsicoczy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3frgrabuf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jdpeonnb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3greowxnk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3izeryljt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fnrryyuu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwwlebxf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rknjivpi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3atllohsd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xaslfrqx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zljiqkah.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlukqmlx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3avipiqof.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vnelqluu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3krdqgxon.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnoptchv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dckecdoq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbeeoqgb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3upcspchj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3idywhlys.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejdyuqzx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3deshcadg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vfngfixk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nuabaxwm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijioyxge.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dxqcbliq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3txntkuwy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ridnlnzd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fswpnaso.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykvsaoqp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sqvxagvc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3soeevgnn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxoyae.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oxkklelo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xosthxuq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wiyzjjmc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gokeysgn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qohtsxjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3szkqmxqi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qrdnvzpt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lodlryby.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvgeqdpm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcyxyrha.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ucbmojqu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3izgzypwj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rlpqpbtw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fupsbclj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlejhikt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkjnfz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uxfciwdh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkksynqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jvbgdpvz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pksvftvu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3utlcwotk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylgictdx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhxhomj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgckrijr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqurij.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ylouqewq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ppenolgp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3clnfjsed.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qkewkjfs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wgrdtzbb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3derqkbwt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vgitcgvd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xvsnxhey.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cuowmuvo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fahyldls.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3invjdpnf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ufqrxezi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uelsxmro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3polpibwp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywtrjxfa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vctzhzng.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3miqdjzce.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynqrbivs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3odwrvgvr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cxzlbrfi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeiixxzq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kwpysuwy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3itchbgro.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qevnriaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lxiywlsx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pjeewzrz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3uocoqtzk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ivumslvc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mvgmrjzw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3okyxbicj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrgoztl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lncskybh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wmgismwf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3trmhybue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stajpolr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3eaiqwsan.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tbmbbycg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3iddjdvtx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ujauqdbq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3johtdcqk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vohgfwsk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ffpbrhff.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pckfduji.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jysqxuts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qsvjrdye.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vxcmtxjz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpxyonjf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zvcfjfjz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vwtecliw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iettewyl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zrqealpr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrnofb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzjvtbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hutqdyon.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wimknjtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtbsrxby.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iowvuuae.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ejnvxqut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxkwtewm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dkawrfdb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vyhnzyjq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nrekcwhk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kxbqohxe.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iuyccpxe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vprdkkyy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlfdponk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ypypxeji.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyqdbgsf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jaseuciw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srknqqjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qugbgevp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpudaydw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ptizklou.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pdafaeqs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zugoijtf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3itimpusd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dimgwvok.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3riuhadia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dvlnjgyz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxrtwbof.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xhiircfb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqtkdzuj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kpzwvdgr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwijhrkm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hiyvyenl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wioprzht.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cewfxagp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3doznyocl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3veietehz.html


<!-- 参考信息 -->