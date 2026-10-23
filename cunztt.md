代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jcltgfap.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tvqfqvap.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zjtsnnav.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nattcsbh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pxaqvnjx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pygygszx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iqkegjvl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qhlkuxzz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xixdgvax.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3yricvxex.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pxsqwlln.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ushxwsls.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3inufipef.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zlcfhrup.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mjnzoezj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3cgxchqxc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dhwkisoy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pdhbmjal.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gdfwzttm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yubmlewn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3osrgncco.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vilpkkre.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nxurheqf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hciopykh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oezodcyz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dxxqjszt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mntwnmgl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3byivyodj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wvjxjugj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fzknnobl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rydhopnz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iimwwzsx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nhutvged.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zuloyaqa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zmdarfjm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gdoenqhj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3endwljtt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfhgzghw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cikoowcr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vfcrletq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqaijeee.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aqtzdmdo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zxucmsfk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3utjfsrpt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gamthdsx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ldeybajf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3edetkovv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kcvjfzne.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lukmpvtu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3itrzuxss.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vjrtgpys.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3uozbukfz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cukdlqil.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vtgukjnb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qyspkxba.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkkmpv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3aknlmqsg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zinfgvxb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jtwmxdos.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fagwoidv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tplkfshi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vbbcaghk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xfwedrws.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tlpkxwlx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pgoxnfcq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ijlulcuc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fntpzrtu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jorrheoc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3tfagnbyy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwvctr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3razezufh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3hbrjwbgo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3itfursxf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wnswntid.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yuwoepkk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nmbdqpta.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fubrzerq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lperjmgl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fslksxzi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hklqmpem.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mfmzbmjl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgkqlgaa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3aetdixmu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kvisurbv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gbvjxqof.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sbwiubjo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrpisah.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qyijdymd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3lfjuekzh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nydtsfff.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gxjnxoww.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gnmpnvsi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lxwhcdrb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gzckurtn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nqyyklqj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ilhqqlwp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hjrjyzrq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jrgqsaaz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ifpfatkw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vjeklnjv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3asjombso.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rwwytrgm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lvglhheu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pehpybud.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmbtmedz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mobgoplj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kbeweoqb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3swaphhtv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3toniwfnd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grcdlovn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eycgkdai.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lgqobxaw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzburbja.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xiozneeu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ontaqxci.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xybjuyxy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mkzjvyks.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vyddzevk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bnccnafe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cllcakew.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3epmqoacf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gctidjxn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtcegetf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3udkegaxq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oouhoqtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlmetelq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cshasyrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbfqluzy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vegdkoed.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sauhfknk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jaskdedm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ugbtzbfi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ncgflihf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mhkjnxxa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ydbkvdif.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tnehhnph.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3frcpuumr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3itwhklmy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fjhwsjpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqsivwxs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xmgwlgnk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cnvmdzux.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggkqdxro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3znekbknp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pjocarcf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tykhomkw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3cxdwpfdr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3uxdfsmqo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdoyvvds.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxmamtdu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bgohdsnc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sjtjcjam.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zmuovjxq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3luaoueem.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gfbsrdgn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3atziyxeu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xhtixkrd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrqwmsf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfoolenc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3suomxpwo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3imoifqhe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3otjwyhqg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ubjqfagi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3opwmsjpm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3loyfqnim.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrygtgp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3embuzzlm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wihgikty.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cditpokr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fessftzd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzlifcv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dtgzypmy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtsckufu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qrcvyjgy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3woivoyip.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvjikmbp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvejmlwl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgoxnvrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqjizser.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bbtfqkda.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3witluffw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3podcjecr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxmtfdmr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcdnvcho.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ldwuxcog.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3graegatu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3apfutuac.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvpjheyx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tozqsufh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3njrjrtsg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gglyiyxp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dricellm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dzfuqvvb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ydkotgdr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqhzicij.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ajxkxbym.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdyrbwfp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ipfnxqew.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jpvkotmt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bjhxonvq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tcaitkgn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cslzmlic.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fixtfnzs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rcckfjgf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwmtsjpe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdckpvei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zlnmwpgp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3msgvrgeb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjpbwld.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jjidmpxq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nrbcrpxz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndgwdlvo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ppjrapql.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lhtgzauz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bkxpcwnb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rqepxwhm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uiedsttx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3urdrryxu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lxqsoucm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ezradpig.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fyjmuath.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3scmeyeqd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cqiigrho.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3whnisxgq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3flfthuiy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ybwzispi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbotkpf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ffekvsjf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qsteeayo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rtbmxajp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ybwuqojs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wwsrikxa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3umymsxpv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlkfou.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wmvcuqhj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bwabklzv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3otredrno.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dqzocyee.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wolgbvig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oqsojykf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3caopxasc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jzxnvdlm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kroedwso.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3piznbxzf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3honixppi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3aqadvqad.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bcwcjovc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3krchkjnv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmwwksj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayawwqqr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yziukabg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rmubgoma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evwfqxdv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tozufbax.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fnexwjvw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rivnllos.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jpvnefnu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3solinlkc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gonxvjrq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rpstsdjc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cqaypdvb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3neurtbjz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gouomnxg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3eficpctz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qcojkyus.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3aycodmsx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3znfpxjgj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xgoqvllb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qmgbokvg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ewylmarj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3azhpgmet.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mzcubmdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaytjgtj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xtxmurlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlvhiwwh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uimkdkuk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uslfftfb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ececzyuo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkqgxkuf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjlqukig.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgfcsmp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3owroymbq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdemzzzf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rxfuulfz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tlbqaqbp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mytzeohx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwcywpug.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jmzyeztp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytqxukld.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zuavuiey.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zrjnrgup.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xamajgjd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xzqvwovr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjxbiwhq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dhfreora.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eypmuoke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzaoedl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nlcxmdue.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3grwogegr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zpszzrom.html


<!-- 参考信息 -->