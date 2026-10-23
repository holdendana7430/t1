代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nqhjblvg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nxpqvjhv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3plsrkqwf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ogknsldu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3yerbiixy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rckrgpus.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sghmtude.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgknqaa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tmpvjoqh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wcjcdpvv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ksjhzdrj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xktojwwf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kpaytxnv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ikvdfade.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gaqjhwui.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rxptlkdq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3unqhkreq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lutmocmy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zocwdbku.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fbadqlum.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqiloe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gfnaysdu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nivltjoz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3loyxdflc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3grfvcbmi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3evcpygvr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iadsdumu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3swnictvc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rlzgqzos.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jvdetnvf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bfujnpek.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cpsvjsfs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oajvbhux.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qtklakfg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dmsowkid.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xwxqvaoe.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dikvpjts.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uaeinqxp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mjssclkx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3becgellq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mhagnvrw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3anvbdseb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owjzmiax.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zdsagrev.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3thvazdxd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gepbqtin.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ofzfmlfy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3agmgwezx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lesuxdjh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bmfwljoh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rfhrlbym.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3moispcng.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqacqrvk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjoiktae.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xuwqdjuz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cljvdzgk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ovmbsbdx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3clubrpbg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3krgcljqf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ksiiykaf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hztcddkc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ysncacig.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qwokngyl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fjyhmqny.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hjypmmgg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xxwhsngh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cngdpgxb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3puvggyip.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lfnojrtu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zdgmrorc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kaiheivi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ovwkjtbb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3isnfwcrk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hdgnlbgp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ekgnvigs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tirmaftl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ikcdpeft.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qnmgrtyo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tzroafkg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ccfigdep.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3guhftang.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ufsqhwdu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vgwnycbp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rbueiwrq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uxzmakgl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xzekjuoq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3plalpzyk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rieyenmu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qgiqnkgx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwpqljg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ocmtxmoe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3irecedpv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3brsemqlo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hkfeechx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bqjitekw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3dqrfktyx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3geumcbsj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mdonwnzz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pikcuwyi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ejjtvhmi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3afzqnufo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mkmkkcrh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ybrzkfcw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ujjezifq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dipdmymk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uapgzuzx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3enwdpclm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jpocnfdr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fheuesox.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vsfbjuxf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3onubcgwf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3edogumxe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ihzhdmzw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aspytpaf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nnmtwavr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pxfnetyh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3flbbiqxn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3udfhrolq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lhmkscig.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jnkarkus.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ouogbdsl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygrhmaja.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3akpnydsb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtchmio.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3lhkxmtkq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vpgsyppf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qyohpryt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjdtfww.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3klsnhttk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3aoxtuixq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbsownq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3npyazdag.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3svjcozgr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwagcnk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mphehbkl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jfngbxyd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bazsjcuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duzaadxk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3komkafye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwcxgkcn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gdwvbtee.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zjzhtmfy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aexrixai.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rknmfwjt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pgegsukh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ganbgcuo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qouisdue.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbocok.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tcvwpjlc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sfsobizn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ejntuisi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khbhbcac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kiqzjadv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bvxdwtay.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pozifksu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cubcrjgj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3eameatzg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cjkzpxqd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3osrsfgdo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3olslfvgh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieootlzz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wbmtugwg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cnydizir.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neurfqrh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lzpkmckm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hnuezgfi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nhxmuvlq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pfuyumqz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kunopzzq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3takzilyk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ipjuphbz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdcpawox.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vszernve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tznhdvvi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zsoebzub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mjdvywdo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3frxuhqda.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zjznjclz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lwzgofqi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mamwrikl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhzlfaf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jziidsik.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3metzxfzf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kydjaadr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyvidfth.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jozyaczp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vasfwsxb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxwvdckx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3axwsbmqy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ocsrtzhg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pxvivnph.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aoddlpak.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cgrkcpiw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixyygego.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kimpedpw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uutqkgqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxsjfd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qxviqgvr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppvfcoka.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pimldzvo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hpfwlecp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxapqhpg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3otwlsqcs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gmgezicr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3auoiwynm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vtpbbqbu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yhpbtzpp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ukpgjlry.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3apncqmji.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhqyxakq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ipdcrjzr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3khuqabjx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3aijkekvo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jkqnyiak.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncblsgoa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqbrkaao.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehhkbtzu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yxknfxxz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yaglnhpd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iromgvve.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zjbosyhp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ldksfffs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dahcrghu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqdhawrb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hhgjrjiy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3acvqkbhn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cesfpiiw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qrdffpkl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cqkectwp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmywsd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nsftqjps.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xowuflqz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vgwvpdng.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qksyzonw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsxtgidg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dapcpzns.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lpvwmzmi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3uytgsosl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vekjlrmm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sobijfkm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jiwzrjet.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pgdcgykc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xwnasdnt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tjoulupd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxqfxhq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3watgdtru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nooteggz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bbdlbfpg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ameespnk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ldtxduzd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ougeccqc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wjmpombc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvlkxyj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ecdxqfpp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fseotqha.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bucnfdcl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3skereblr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3slpwktqy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3grqmaiet.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vtvhrosv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wzlgnwcs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbswtpbq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymwdqltq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uznpqojd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mrnvbpcv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgrltgqr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pezgofsc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dlggatht.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3btpuelda.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kgxbkpbq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3blsrkqgp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3emnsekun.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tjppfsec.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzystxss.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxnyrbzc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hirhhqcg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3upadyexf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzgllxge.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mevppivy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3crqleell.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dbxpuneo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3svjqfvss.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sgxtenmf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zzcndhwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxcvrepj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bkjbpqnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyssqjxx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uyheizwj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rxmiktiz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gcpdcrbl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jzurzpfu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjwacdlu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lcfgqeuk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cadetljm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qohyvaoq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chuftugi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xtmqmewk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zxdtwafp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dglvxywh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nndvlhqp.html


<!-- 参考信息 -->