代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gjlgelsp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kqpyhibr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wwzcbrcd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3enlahhsn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qzualkmf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rhjzguvg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ugvefgmw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zvbjmqns.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xunjdyxc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3stufgypk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqydlzzn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vlesidlf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3sschstax.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ijgxkjlj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hliekhkg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kxfoxton.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wqqougzk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3unbrmiho.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oomressx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xcjupmwz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3veedffzb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ikpqhzgb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nyhvtwod.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kiynxouh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mkxovqty.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3smnwvtvm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qkhbbnfv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kwesqbuy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vlermany.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bbdxpsfe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vmibbebq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zwvitrpd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ovlobepw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3uwoadyzq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3fhcdfdrd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3suvpqkdx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3awbpxxan.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3glglrusj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zwgyiepq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ubmyitox.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3opxazcts.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bsidhmwp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3foslusqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fquhzdhq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rodgegwu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbdunjes.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ddwinedt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sofqoshj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uunsnfqh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzraqmp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxzzce.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ozsvzcdf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wejafugb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3flhbhnyl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3skexknjh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bpobdilz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yrrrbidl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xzpbpaqg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3phjqkdnq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mdvuivcc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cfdtnlts.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vudwzrfq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3agsghwmq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sceluraf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3reoohpms.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uinctlpp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3yllwckeg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpqxli.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3elrhadyx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ncbxniqw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qfcgrufy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3lpmcwjcu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wansxunb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bztksmyt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3opureedu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zwwtnmog.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dleikmte.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hoczddbv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3siirycfa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcwejoh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cvuuwdog.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jppcywax.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gweeeqti.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jmycgtzb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fczjotpp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfavrftd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wotrqjix.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3okuetijb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vhuxpyux.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nieoibeq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vggtrqal.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ftjzvhmn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hjvaffck.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tuhuvkyq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3qynohmsy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxafmsd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dfjggejc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hdyqvpsc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sevihgpn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ixmzrgxh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aefgaups.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vwlesulq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3fauzsblj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ijgaptjk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hkzziiug.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ulgplcdn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iqurjfub.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ipndjgdg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tcgqkrnp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jfomwbte.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hxvvgtvd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nuxgxgcb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jmswtllh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vhrnuoqp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wlavhevs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozauayjr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3meotbgrz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3avacfpmy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3smfomzrr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kbmgjpps.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sxohhpxf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lshtrsmb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pepruvmp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hlahznye.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hdokxazi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3iehexkzw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3pcgibqbt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aomrfavg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xulsppch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jofjimpb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qykojpml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umfewmtq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3thalndvb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3shzoooce.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzhxerz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cbpczusi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zqkyublw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xfixsnlz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ujvnjksm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3elpjsyjj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ayeuszmf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3asziggnp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zxcltlix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3szoeskwa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fwbtrfcw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jpicwbvj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zpggjhnq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wjcewryd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3aghyvsjq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xckphlfm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3reukhovu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yjeczkry.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ugcewjfe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbxhkdyt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kumpcgln.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djwndbvf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3osublcxi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uzklpmid.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fcscvujh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3svukewyc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nofhkwha.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdqjedj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eiholluq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3akjyucys.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjcipoyi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gmvsnpdz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3husnrdwg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvnsmczh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zimutljj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3gzokxelj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgnbjjdz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yohrtzuy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrfzmzre.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpnzpyc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eskfckcs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lotspxlh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlrfjcor.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3knepaawp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pjkmfaru.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqybjzsm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jeqgaqqh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fhmflhkn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dodbezko.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtsmuq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qixspcxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kkrgizyo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vurniifq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lyzzovxh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pbcycxgr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jstnlazj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tgexaovt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ilpvdpyi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hthkwxmp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvrjslup.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjahlzx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dipevvzp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rzuksrkl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oycvcclj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vaaxnrdt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vfuxjgco.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3possiink.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3prlnboky.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iucwdwub.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdzrhwz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dqimxnpr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zuavdnfu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cafzbell.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3orfcbloh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wggkdedc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hldrwgnx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozulzqdi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ywviueyo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhlgcld.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3iykpautw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xonlvoge.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xuvxwlmo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kbvrjszf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wvanvbub.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzixgbte.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3praycwss.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aoxmfdyl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3twgecdju.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wcrrbiic.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pdvuzisp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kmcaiteg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sbfhwnlv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ahxysipg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlvvupji.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mjcsshdk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3utblqsrs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jyegfhlr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjktdfve.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3eppzvfjf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3izbdpqib.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ostkdvid.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ackoksqp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xvpxhkgt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygbophoe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dncgvtel.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qhkkjihu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wlvgyvxu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tbuzxubb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3locnaqys.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmgznip.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hmpjpdnt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3afnmxxjc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kqplvopl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vxxkjdjl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vervxwie.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vajvoecw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iejgbisw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cpppkgsa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3skckrfna.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mdrsagkd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abusijpp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zuyqioag.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3opeifrbz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kjwzibsv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3epattuhb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hrutflrj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mrerxxhw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zvhkryue.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugntpsbm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swzhhzwl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3icpuilkh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3auczqxsk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqfloswg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jirpaqol.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gkkhkcrh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjoxkdb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3teypozxu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ljxrpbcu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tettbdon.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qdextaee.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ucsadffa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zrjfmkpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hoaipwkx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wgsrdiup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izipkpvj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uuaktixz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tdotqhph.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdgyjmdh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bphgzpow.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zzmvcdzv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3motmtdms.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ymiejrez.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ypdotpmr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjyrrgpn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfccmntg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kgvdueex.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3keggzatj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3labivmwa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bcphhqst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fbkokohq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqlnztem.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3twicpxxf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oaihiyll.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rqfymerx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ucaagcku.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uegozvre.html


<!-- 参考信息 -->