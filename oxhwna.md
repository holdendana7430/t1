代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rwjudqsh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mwmcktga.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mllptjph.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ythqqaut.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pstpghck.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lljttxhv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bgjcaqvt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2empelogi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zkhgqaaj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2cllirqsd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wszdgeyx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2xcefinjs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zbspziph.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wnpaarqo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tyyioqlf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gfcgymoe.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fseuoxwm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2scwyljoe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2agntmlls.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2sdakfmhs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbnquxo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jlanluhh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2diglpied.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hszbbuwg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vggmwxph.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ghojhadm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ricuiyrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akezgvzx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zlhierco.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dxybynxt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlsfzkio.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2omzcgffl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dlaemqvf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzjqoodo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2atenwcvj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzjthert.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2acheweje.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dbgctvwf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvnvmmvt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmfmctvp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2sehqrhww.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zenupjtj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cpifaeqt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eimywzsj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cipskvpk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2yrhovzkp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2kvwqfnmc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nhygmkzq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2abmwuepd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xmkzprdg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yhuodkjm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fgkjmmnh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2muonksdi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2elchxeqf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hohiluxi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iqufhklc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rloeccou.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2iucoqndb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tztelmhs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dmndktkd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bqcaqkpv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2grbqurti.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uburyaqb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jiaitrxe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvooewp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nkppahut.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fmzntnrl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2bqlxiikj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2txagwthw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mcxaxhcd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxpkqyu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcqiadk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzcaotg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhyimeq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fasqflrr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2cfbruuyh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2penotakk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qccnsmyz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2aasdahoy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2posbwckw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ilglopav.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eibeldcy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ciqqhqme.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ihcxpufy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bdqbibgi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hpvxcgfp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2miltcxys.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2clukbhxr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nrmzzxre.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2luepukwr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfrbez.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqwulcx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2knvasgye.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dfqgkiqn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ukztrrld.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fqbnlses.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dqcbfnwg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vgdlxaui.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uzdxtzid.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gybqavwv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2oxmlxkpg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2moxphrjx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjjhyagy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2punjjmmg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rldakijl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkqlqcp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gzbtetuu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ableqvig.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwtami.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgvygdz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jvxjzqaf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dfyecbas.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2trclzvle.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2tduxluyi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fmtqubha.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pqojhirf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2debjpxau.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrzunlr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pbrbcvrs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fvarmdlg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bxjlztri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfccijqn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fyrrfaxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2godyufir.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qkiqejga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qvrlpbec.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2avzbcbyi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2khklccyk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hrzhddjs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sgcmkzko.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uifokdez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hmzclcqx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nwioltpq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2puphgvof.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gwayeaiv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dajcbjft.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cbvpqsbl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gktgnsta.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xzxrwydi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhdlcxky.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xgpajwny.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nfwsceyj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cfphbpks.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ykxzxzws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ixbrxaqj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqzpeoe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enepcpyf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qfxtzrvv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mtnxodwu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vjrxoyrs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tkuphzic.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cezrrilv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xezedjtl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ankpdsbn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2maxtyzrj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ythalmqv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bmranycy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2nfuvvmvu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2charzasx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bmlfwfvc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qzfirztx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hpoqutmf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dvpwcxan.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uqbviulh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ahxnytxl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cyxgbplw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmtgyml.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2boelbzoe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ykfhirpk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nlwjzzlj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzuiaxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hndqojgs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecsuozxq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bbdnskuh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nglmnvjm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ndmggmfr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2sdxzkkvi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilyvinnp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rinqoiii.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fxtzdqns.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxugzaef.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yiolmlrw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pjnzqfrd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2smfajwxf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2aqranxqw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlecldsh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2chskmkfy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lpkbynmo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ayalrrwv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ekcfrdib.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pncvpjwn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pulhiahb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2okwoqmap.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2elsvmcrd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uhxtvekb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kccqkspc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xmlozszi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghurnkvr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmgohav.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ihvyqson.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rnwjkuwt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tvjaalnx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2poqacilq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ggqqbscl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfdjhbj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kjbvwvgq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gdinwknk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mrvditzz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2defmpuwh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gqqtvhbv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yselpnxo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkhmufx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ytsrtflm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhdzog.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2foqhctne.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bxmmjwug.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bbtbfwho.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wwtysdxf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fnlyjnai.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xtzzelfc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wbyyofrc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rvnnylja.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wahvstua.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jtuoxrdx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yyohofez.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qdveowfo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2urkhktrv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fetvevzh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ktptcnbo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnnhfkys.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fgglktwe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2adabfxhb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zwofdqcd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tchmnwsg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwuubut.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sfdugtab.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtvnmnf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tzgcsoti.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2toyjpgnn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2disjyxyl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qymouthh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mlpgqxdc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fpnehwlb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rztlbhkz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pztorqyr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qjmnjxua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcghgvko.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amvwuhil.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nonizgwi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jgnzxvzg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2kzswuxwy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kwxlwmpq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mhqmsmli.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltepvcuk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wrwtnudg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2momsvohx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbxtkfle.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mebdnoxw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2daqjtmtc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2omobvaun.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxiyge.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uujtrkwj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pewpvpes.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hrluccua.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mdfdguuk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jjknqefh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qadybmqm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ldmbuajw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdjklkmt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ofgpqlmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhylycwv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vgomairl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2khqdqatx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kozqwfyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxcsryo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2conxhcyu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eafexviw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hltmdpar.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2azckizon.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgmihgix.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdatlwjb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cdgxettj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2juiprpzl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xcjtbkia.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfbjtaiz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oszrbmyt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvxambev.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hwjfdlvk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2imwuuwxa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pyxnpjnl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jrentiax.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfbplwm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsduhgfw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ltqgowcs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnauebf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2aswkvzcc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nmlkqxha.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2atewrxif.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bmmdwzzk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ysfafeym.html


<!-- 参考信息 -->