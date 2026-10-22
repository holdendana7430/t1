代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kwdbssui.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgffdbod.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vwwbrnud.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rrveuehq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gwuezkhu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lylfemfw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2skpdtcrn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vekxovof.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rivnnnqz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jfmgxfml.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zhnxrojs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2istdkcgu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xyrgkesn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jdbcuyrf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yqcxlirt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ngvsawme.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xtmsmbki.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2myifbbdd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pxoawrrf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fmxwzssc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tekjmpko.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ybsislcv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fdojutzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzekvkrv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2foduypey.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pbtmmnzr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2qzbfseuk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2esinstzg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kbrnacdt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xrlsicjf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xldbbkmi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ihnxpydf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gnlvxslt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pxdmahbp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kppjevno.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fepplhzc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlcwssgo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2khxyjtdq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zhqursej.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ktwfemyx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zahkeplr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2teaiemfl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2shnebuej.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2avhoncji.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wifrzocv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dbkcooff.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qobdzogu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dztjydom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2puzrbpnb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tlsapxiw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yqxvcgdo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uzlbibhs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2lcurtqia.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2chyfipvw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2szfoqeae.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ldiwaecb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2padzgqhm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pinhajhc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jcdvmykw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhmdvp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hsqswmig.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpcpmra.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wyowzzyk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2avkmtqht.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2akmdlnkl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zitbkrdg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tcueweis.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2htskezce.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2jvoltxhf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2msprmhmh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xpmpeocw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2aiylkusz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qiljgnsg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bsmzijsd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2goiwrsut.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ofrxqaeh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cwpjdnui.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oukvcxdw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iceuwbpc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nqpoxrww.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vlrebgeg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrfliugz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qhfmviml.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2owpaiyvv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2faytipmt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2azrdjlco.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avgmkomx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fwonltsn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2apjhenlh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vdkcrtob.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zwvtpxic.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2foyyequf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cttattjc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bjvpcmko.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbwusi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2aptnfgna.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nadyucnm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zyntibta.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ncvyjwrd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dcoejpac.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ntfizrha.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uaolrmib.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2edydvcsr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hgznjnry.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2pnvavejc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dhfyfjik.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sxhhysey.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fazjsdsx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ftnjwkxy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqhvbpi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zxhtyxbz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vlfvuwgj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xezaodtb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vdvmlyxd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2irihpimz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2imrrqsjn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2abvvpbio.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mqgmvydp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2oktxqkjh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2urlyxarc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wgyxwqpg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2thlqdfwr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rtovtyqn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hqopvnzg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rlilmsea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbxxhweo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2druckzsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqzsgtqc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tdlfclwh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qfkybftl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscqulqb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wbyrmkql.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rvlmdzpt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2auifqwkk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhvgrzk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jrjuzqvh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2twsesedv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dnxabjnt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fempjucs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nqwsofot.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ncrqdaea.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2luaxgaeh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eqmgmelz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lufcgtzl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2twgfpmjq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zaqjjjmr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pzwuight.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2huojcgzc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwdkuvfr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pmqmekkm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2graziijl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ytfvutyf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yzdsrmtc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jbjhvaup.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2avqcrlfn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ccmovdug.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2aikthlof.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2czhkdnwj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znlygvex.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcejsxw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mojqlqee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ufequfsi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vnmzhbvb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2havpkads.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iqffnysx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqkcpwt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nujwvdti.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ucrbglxv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ydmfgsvh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyoqqzyv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fjijmbha.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xwooiikl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkkmat.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sqhpltlz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vdnrdtfn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kkzceeoo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gasvafwg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tuocjfho.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxlzois.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxdkofiq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jmnnhowp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tydhtuta.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ngbyasnz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bfqkqaul.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tplijryz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2skrjhvdn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bexdiyjg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjglgpf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vnoluvsn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qccwntqt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ytagezev.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fxilpiqb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2izewzscp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ekxvgrzt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dxsltsuh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qwcowphw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mzdsxuzk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ymogrqbc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ubypskbw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yoiolvua.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwxcid.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kqrhscje.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mlsohidr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kiyrirpj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zoykneov.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkingelt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zemtevxn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sbhveupz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnexvrsd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rzmaaenx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wwkvzcht.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xsnvvxzu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2syzybifb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gqdeiwob.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfmblwpc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2inqvgpsi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gakzxjfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjnobuyw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dzwwykqx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2italnipj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ykfahsfk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gyplypmo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkovbpdc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gndixyrx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mdqafgrm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ljrnorxg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hebphcwj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jybdxayu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kemwvnwi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aehxqppz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cceznqvp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uzggzsop.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hpbcevdn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2auugvgxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oakhzpkg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wkzremgn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xaebrdln.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dxaouksw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kragzxeb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pndfbkgc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiomtkdn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2umhcoaoe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sltmvkyy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jaynnlnf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2blwanudi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vcicgbch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lhniqgro.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ntnucyie.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xctsrhwv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dfowqagy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wjftlgom.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbahccb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bakaoyzp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2osjnotjp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pkzisxhk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hesrusvj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zohorkpk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ekqufmnz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwlodwye.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibechvjp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jphpcikr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ubfwrgwb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rlgihoag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2crjbuciu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vcjlkayn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2tynsoyit.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sweddvkn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2utllrtns.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ivohteeh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gjovszhx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wrjkdfmj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2flsucxng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmqieolr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cewurgrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwxcwwau.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofohijkh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ygztqsut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggsuatvf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hrtevijg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxeyrzkk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxmcrcr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhzkczg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2whnadipz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcuzryqx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ceymrist.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dbijnmod.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bjemhzwf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvbpaerg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuyjuvgi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ujlmzfpq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jytasyrn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2htgyimxu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sbedhcpn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dhygjtja.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ajexozqi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2urmmmdcv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xdsmjxai.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxvkupyh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ttjmfykb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ikikzcvq.html


<!-- 参考信息 -->