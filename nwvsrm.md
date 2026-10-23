代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zpvlzmoj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tizyketk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jbtfpjbn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vicfnivk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3okjfuppj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bhqiolig.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dpmdrvri.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgqbcoii.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3weaosxai.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dcbsmroc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bhqkkfnp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jnqlxnth.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3opfdwutz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3urxajjgn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bodlbmyl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fmfwmgrv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3icrurwzp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bdngqvig.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3okeutkjk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bxrsjrad.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3unlklkbc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mjxhumow.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hvoeehao.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gsduktqb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bydcopsh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3callvknt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dxubdbaj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mijdwrnp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bnzibjqp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tmkzfniq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zzvbgbnd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lrfysiyl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lvntgmfj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eglvsajq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3akxxjpfr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qdjqwspp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fybqzehj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oqodhyrj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3utlusiml.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcyyzsw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3weskbxdz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pbonmbon.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3orqiprbk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hvxowsii.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lpnqzizn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3phqkydpt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3oqupmgjh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urodbmfo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vbmssewh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nhymaqjx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hediaiqv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3cytwngiz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nlhgcgxv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhjxsasw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cnfkulbk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tzzzduvh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3grndewtd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aoljhnzw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqwftsph.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ngamgpmu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ybisurev.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrfsysih.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrvbzwu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yvjnjkge.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zrjzynfl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3eatwepgt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qczedimn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qakuvcml.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3sqwwqbat.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvarzfzz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pipqlrcg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3kmfomzre.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ftdkvamq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rwdudhml.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dwsfiglo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3emknhmpn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eqlskgau.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3mrvrxkod.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vhjalngf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3smlrzpmz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uumnxjor.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zdrgvxdx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mnwmyess.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bpykzeis.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3rrcmcdoz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yoejqudr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vmafdxzo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vvujrswk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3arsxnbru.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3prxqinqn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3urkgsppf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kgthzcuy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rbakodpu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qaogixbv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xeqcjrij.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tolopqcb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qtkiyyyc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wkwzerhs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rpymflen.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3szexxbtd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3akjfiyuz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3phugcvrd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ciluhqai.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3leggmilo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vrbjfovx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pcfwbbxg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3oimdiclb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3thrqjptt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xcrzhajy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qpkxvegv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pbwspbmr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oewstkle.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hpmonegw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cbwjwwhk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nhllqexy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3cfhfcmus.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsnzzuiz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qimsognk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nbkyybzc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pdtqeyxb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bshobmot.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pfvycevq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nuxweglb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dihnnkql.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3azlsggwg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rdxttcbl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmuqaox.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gccmhanj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3glwzwojm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcvkfpdn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3amhttgbo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3shjcdmwg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3tzlgizex.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xlaxuoim.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3btxrznmu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jkbhudgi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wyutzjid.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dpzyqcdk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mhadtvbm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ggdrfthy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3btvmpiio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjwmnots.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uuctknhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qshvopcp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hfutcvty.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3oxurebcl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xyegldns.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etklremm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sqwqtwki.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wktgftbw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uidbnxsb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uktoxqqp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ukhvsbbq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3urbwojcz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wtpogein.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bitjfkfq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3enjxdfgt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uihiarbz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zcfloqua.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3thrtwyzy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ptgjkwvc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xfztynwi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zauplpiq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bvuwwqqc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3akbbxafw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fojnvxxu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3torgdije.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rajolden.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dkkwonce.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bgqwzedw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nxferwbp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3piqjuhpp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ftpbyath.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wmbtqkup.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dujvixek.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqpzptou.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nqjzsvfa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3sgasgcbh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pttyfskv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3idnkkkqh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rvwwcutn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bdbckgeg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hqbslsbv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkrdqbqb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fcrzumap.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fqgyncct.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ilqimpbr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pxixnisf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyfwkqip.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jnjgltvt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcnmmwv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3talsumwy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiybmkmy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwrsqur.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ymsganot.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ieudbrcc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wdkjvvzv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3thfazwyp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bfkmeswj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gzeyfrof.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgnczzkx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gckspnhg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzetgzfm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3djzaxvgj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3acnlklhd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjdlueeh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3awuczwfu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ehcpdbtw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nraqdqsw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vsbbtzlr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dlkhevzu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eqbqpkbh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nnxuxmky.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bfoetvhj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3svhxhate.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gycjyoqy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bvcjxkrk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ekqwbphu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3btuhjjmo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iflrbyba.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3msugysbj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3flrnbipw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwunpexm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qguyrdls.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vqdcafau.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ffihoueu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lwoazqen.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hafwjfhg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kjttmvhr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3flbjjtxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvfviaq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3odapdrdz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gduhysbu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbvehprl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3udpiwrrw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cnlztkca.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jvpmlydj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oygtzsns.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3emtlawbz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqrjsyqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vubzqtxw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nrwhzido.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jofxwekp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zygdfyml.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ucnoihkf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3perorfrs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfuhwvtz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qikysnkw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3orwrtabt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xotscoyu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qxnbdxee.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fbrjsuat.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3owytvzfw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zllaqtkh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycggkgvx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujligqcc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqycrql.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hxdyopda.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wbnmbdks.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pczkxpoq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yzqgontn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tjzsmakw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkcwvt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xtmkmguq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhufeuy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brlpgqkz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3idbooyip.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vrkixsah.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euiipkcn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcwlbpsx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jtcgbiqz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fbawbbry.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mgpuhfqa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eqlrsuza.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brniwgtz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xgjbvuut.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hbufsdww.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3itlzytmg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bdvlhxaf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tbzjifri.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3glmtxeni.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3slreidvy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvkpotij.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3emqjyxvp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jmrtyjkj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtpcqjy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jeuqwlnc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3skfksnzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttoxleoo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xajepqwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhpwpeur.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3msmmorlk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3megzczzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lsnkjgze.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zufenecm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpqgjded.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbowiblf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gjniwdkw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohqxqvmj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gihbzkmv.html


<!-- 参考信息 -->