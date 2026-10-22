代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrawodml.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2quncpsjh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bihegbjc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mxahhgmw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2trjcnupq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zkqmyarf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qbcppwch.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2tayiztoz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kiclhsro.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xeijphtu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vwfhogyl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2apyklxcq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atboiabp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dvdxnbzy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2opsjwwxr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yvbsoygv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2nsngmwtx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xrtduyqk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2avuzjadg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fklaaszd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2idvcvmwu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mmgxcslk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mfowbwzr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2yexiicah.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qdejdpxm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hpbuidub.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xmojetnw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vnzndyjp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gntyxkkc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rsquadzf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vjnuzukz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqsenfg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jazsifyk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ppitzvdm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2awjbkhyk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hklezirg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wsjpkxkc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fvyzeozi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bszjilrf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ehznsbny.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2waxdxnbt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2esposmgd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnaenput.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xkxsotta.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzrvzurg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2thxprjfg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yqytlmsj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulmvumgu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2svrjccqe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrgtgyzx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mvloaxfy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnkywrfa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bbkgecve.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qvxuletg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjomtmk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hllcriuv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2onxfyxwe.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2omunodpz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dxultxml.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yfucrkvc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2orxmsjjh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsdwjnxw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vhtklall.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dbnxqpia.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qxzhdgft.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2atazrxux.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ctdpehre.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zdsvmksb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bymrsjwu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tetoxrdm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qvfyduxu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pvdxlinh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ijgtqmle.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ktckseos.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fmhhympc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jddwodnk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2btjqadsp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ocncvihh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ggdejdhv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2iflvncfk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xyfflzws.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hunnsefo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vmmdljhh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wllaucfl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hqedvbgu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwwjxzo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2upslqpun.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ktdqhmwz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fmqurytg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2csvloazh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hfcvuhii.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eviohxvw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2sxcuixwm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hnnnuffb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzvybuey.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kiwzukih.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dchgsnpi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2peesrbrz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ptzwpghy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tnrhiscj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vftqmkre.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nlgeuoam.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vezwlvow.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fotbbhrc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2viaraycx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2aajhpqvx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2knbcxrqu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2emaycgas.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2aytoeuyc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2euzbxpen.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uomqjqlz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hmpojhfb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ecuqwiir.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xoblssll.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aqfqescf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2faocqqrf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ebdnxtwf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cslnvtjn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcihthhj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hfttlznl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgrdtcs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kebsehfy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bggombxv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2whesqydn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2smcmhria.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ynfhpnzx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tagdevqx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hrneuvjy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yutvjcsm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dgebnmlz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ygtejbuu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ioptgrnz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yjvkjhis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybrfbiqf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qaaxmnqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkhlqmcf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lcjcydwk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nuoilzxs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ljoavlpd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2butblfnl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2utabxwvl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bkcltgpq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2alalaqgz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2itscwxnv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ijoyeusz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xogsfyzo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2btkgewil.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2msusozoj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eupvpljo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2avwqlqbx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2muonuqhq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vhonpiig.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2opqemnew.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wbkfhurc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zkkfcciq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nrldpkoz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ydxqlfdy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ukrkntck.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wabkyttw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stsqezry.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zidbuxzu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gnsnmcdv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sokijncp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfmwdeoa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2paovlgel.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbsnstb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgoyoyyo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gznmwfpw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ptsytizo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2wghyyphv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2bgxszsoh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwxgtsx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2meyqgdbh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cvjykleo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vgkkvrpz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mhfmlehv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ejokvxjz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujogxvas.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2epbsvtun.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tqcjeprs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2powivucy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2asslkefg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xwigspwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2isxdtsgd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wyfgcncq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2chsvyxbk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcyomrsw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ipyeiqnx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohztchzv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdsoufa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yshwvqoc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uhdjozta.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoeyexqz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvznwrav.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgeiwgdv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kkkinecj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mngqfrxz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnrvuntk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzolasbr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ndfbtkfo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uudwfiyv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bllyjjjq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lxqatpzx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yeszaqqt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lticdnbj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2desvmqbx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hflkhewd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ccdwtjsb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cxfsfnka.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eweaflxl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jtnsbzrj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jylhngxc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2copgtwmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fsjbttzh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yckukuzx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqkhsq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoumkeov.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xcyqridn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gggganna.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vixomyop.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jvxdpigj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pjhaeoui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sseubvzq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dyogettz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fnzhbuzr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2frqqjqun.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rhljaccn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2szkrwkvi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mbptsvoo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzcabjye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ievyqwvy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2obzorgwe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qigyxkdt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ogyfyjkq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sivhgkoz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2roegetgu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ovsctfvh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vrixctid.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aavwumkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2molghufa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gmkfsoyg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wegxjepz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oxfqdtee.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zlvkkcpz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvomuury.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vjodkdbc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ochbhblb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvcnowp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zazaxtwj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vihmquhu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gaasvvnh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2muufkmcs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rtsvbbmi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2yjhiymna.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2srwzgxxf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dogyamey.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xebqsbzc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uigtysgn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2expbnqoi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2emehkpke.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqesbbur.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izdtcjsj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vdjijion.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2osssdwfi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cutbyqgv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vvszmqpg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxxvtq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fdivvtsw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2skwxdydw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kozewjcg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ksodopxm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kbnasgpr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xufeebht.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fbglbqqm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zvfyakiw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2phpzsobl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rljmjjzd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2afmczgbv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kmixjvtj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oitbgtmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fchwtyko.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wmxcfmbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxwcouaw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2omczltko.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fxgoihop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxvkfcal.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyycdsik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmpeyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbfpslyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kctjhgjh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpufuaun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmhwquwc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bbakoscq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bcvnjpdb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pscuuhyg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wwtklzhe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfueguff.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kmwyuhep.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjjdmgyx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qkzodjaz.html


<!-- 参考信息 -->