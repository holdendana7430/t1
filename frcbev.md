代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3odfjiuqe.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ykwlcnyz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qaxbndzd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mmxlenmk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtjjraw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wfflaxrn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dwcwfnfy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gshlixxe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vkskocon.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvybxffu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oixlwdmw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3auojwqlc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dakkmmex.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mipaduul.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3snipitrn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lfnbjzot.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nruadjzz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3fmepzdxd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwzwpmqm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3stzljped.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmlyvdxq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3koohkfrp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cujcdhsj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cneyqrdl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bwecqing.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cubbbjws.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgtnky.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xmtaxeyw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fmrdtkgv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ievzdsff.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gjwrvejs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3iyublcsn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ofmghses.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rcstupym.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tzfwnrlf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jxrbzfvy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wfkiihku.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jnsfnylg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dzzrgvbb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tnxzgmvl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xsocmtdf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ysotlpuc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpmigdfl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rqwdrhcc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ebxttkvs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmcropvq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynhdzmxj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cyadxdlq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3puamtfva.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mnfbyaqo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwrdawew.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tosafive.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3sfmvsqpn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tamvnfoh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cdofhhhq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxlldqc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sdyiuenc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ayajxmfj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ttjblbiw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kxgnzlym.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hushlodl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3inymtyhj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rtoxvnvh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3dfyqdiyr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hrgxlfas.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mtsciwtx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qolpahfn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dxuddytl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lezhtwqc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zxehghev.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3iyvfghxf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3nkiinvto.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fikdcogu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3umjlvkgm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tfvtfgon.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bzitwgxf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3tcevujak.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3zfxbzibn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yljwwflv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3stufamfc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uknzpfon.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmyrmdb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wdxzzivk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tbrzblct.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdowprx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ysyuuylp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfwgsvi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mwkbdbjw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yyewiaav.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ttpcpvnz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qqjjuyoq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3thkwufwo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvmsovdv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3elvctftk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rpksvhss.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zkhbiqja.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gfwxjvzn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gqjlqhya.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jrtcgzse.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhxzncq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ikbftnfd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zsfanjdl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vhkcnsdx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zidsrmcs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jbzazdpk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3iirehobg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gblfrtzc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vgonrmal.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdwbomr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3abpaxmtm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3slfbiuam.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3sqqpbnzi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xatbesfw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ptldnfeh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eravrmay.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvznktqi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jrbifgvq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bcildjlm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pnevxtpq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nanhutme.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grxzmtvj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdidvlzn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lkqvffgl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rigppuim.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zwxshvnb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3aymugyeb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhweyar.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3onrjlvvs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ehliqyde.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wiicllyf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rwbjpjfk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vpfjqqyi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3raehjjxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgqhkvnv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3locxhmcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwdivutv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mvvcfsco.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jgbzzyws.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jhazfjbl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qyympjch.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sdimzowr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yoexueey.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbiyrph.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wwfwyoin.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vgydvfla.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3znbxrgsr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ojamxiyz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtjxew.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jhsckgwb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mmbdtveb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sqfthvih.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qxfjkvfh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ppiikqxm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gppfquyl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3okcevkdv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vcimdygn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jukvawwt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qpmimqpa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3impqkbgt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baqyzagu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cgsusrqz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3acllhwyw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yqrsqegh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hsbyrsbu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zmhibggd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3voocvnvp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkekuuea.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zzvzjnyq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxyicwnu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqrvuyt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bgkslpde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sagzlqbr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gqagtojx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xanlyarm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gpgbntpz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzkxkmew.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyfdhvw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3udrwtzuw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xensfosg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3guykbyak.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvfjjwu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kjledaio.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3adxfjrtu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3anajcdku.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dnscfqcb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3thcdupgj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3axusepfk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxgdalru.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fqyokpbm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3njnxjgfm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqacpqwe.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubbsspet.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oeehovyh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxkwucvu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aergixll.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuzlgocy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3frweewwu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qaeccvjy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jxzjgyil.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gvkmbnmh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3igawrqug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sgvwgsaa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imjcncma.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aruzkxpy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dbawgpxi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hmwtbbkm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oktbiypt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzjfnefq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zrtshlur.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ribafnox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fhookger.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdkealop.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xaamvjhd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynjpjgon.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oaxxmxrt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rcbwenuc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yykgytty.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zzfkfxfe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xaltvzqi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jfumxmiu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ugfuwqgr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eaqwuhax.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3djlyjmbc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zygpzcfx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbntmsf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yegzffhz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hlqgfvok.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3aupmtjta.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3anfeuhcy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fmjxnbit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pvyuearg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yfrutdnh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vklosahj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xxlkyqwi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gprcaohf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dborwlhm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xcgzuzun.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yycfoykz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jhbyutdg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3krrzgvwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wdooztwk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvnerbqd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3soccikxj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qrcagmeo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hvygvulx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ripgwbvf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pxpepeox.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3elfblllc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ufptumig.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xklhnync.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ysdnvich.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgwyzsz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bxhnppyc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhzuaf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iultqrmr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bexrrtoa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kobsbvqr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qianmwep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rvzolmzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yymbyxeq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3haqjhuru.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vrpwisrc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3djdinpqg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3psfyymcp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ifbrjiwd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ivpwloqo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpddplui.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jpklevts.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zohykajb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ycfezpxm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xelooeag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ntqcvojw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bthxmsxi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkqsaxr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yclkpxhq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ldtdvnhu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zrksboin.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3edzdyzgw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hkgsahxm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jcevsahn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3veqjnedj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cniohlkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kukvoomu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3enprkozk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xtdiizwm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wugsgagi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbdmxvyz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhtzgmc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uueqabec.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yiyzynta.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cztkfarp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmkcypsn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mijfreky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3josfgfnq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmrvbtfi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfqzjulf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izqxvbqv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lzfsvpxa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwupfijv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pxoryxql.html


<!-- 参考信息 -->