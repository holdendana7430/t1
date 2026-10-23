代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cnshgcnj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xfbvsybd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxgygvzk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hcxsfnqu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3mpdrhkoj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3scvpuxqg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3grewmbzx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dfhondok.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyacdgyq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3igsarmah.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jhsqbdzq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3onvqwflb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qywjdmbh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hhcunmcg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3erqadpyn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vatfnspf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eboatlxu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cdowgdue.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3txovqloj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxzsbbzw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sfxtsiqg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qwqtjyzo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3aytvaowk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ngneufli.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ynyxgbuc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3auwlybed.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxalvhzw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hzszjsdu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tfpvinla.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pltsurdz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krbwtmjn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nvhllbrx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmxzwdln.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vubyftst.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rvqsxbpm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uaetbyit.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vwafflja.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rylqjuql.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ojsgiubr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uixnjgzh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gjizukzl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lyzwmeif.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kdnhjkah.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rkwzasyl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fqntfuce.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3eclxjlkj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uhtrxzoi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hjjectrg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fjsxjfjt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpjnnbsh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uvtpmnwo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lvajnezz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tzcepelp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zixslegl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3alxveehg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oohhyaoy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oiwynudv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhavheqd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wwlzbdmd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ssbjnysh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwelod.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hjlmspvb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sbxypvcy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kcnmtplu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rpzrcaqd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3eersxejv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xgqvggdt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3shhwzuke.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tgyjpqht.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvvmqv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnmnahxc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ytshhsyl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gtqalzce.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vfiyhgul.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fybuoufj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3yqnmefid.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ymjmbumu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bqectgbg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xhsgoeuh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rdxdxufe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zavbubdf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vcgzbupj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoimzeed.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ujmmdioz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sddidmqw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3othybdpr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhtbavt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqwjmpk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ekrhevss.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rdcwqwvm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wazjrpqd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gcbcufrp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ffkdtnpg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mbsninwg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ierdupap.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3bcmbyvme.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3waktxtpf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uggomcsr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rtefdsre.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hopsgmdw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3didptyan.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3tynqldda.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3chlxlsfm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uuyddyex.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lzslbfmx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vazmatjm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iccrduxd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kezxyerx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yegcbqfc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlglouir.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3anzrfall.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vupjcfpl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bcinbzzs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxufrlk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qlnvatzd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgshfz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ymbxycwp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uhlnnpiw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gjjtbhxx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nduftaut.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3onafqkim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apekdkwu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3uqnwseih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrlxzidy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3lrzsuohs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tptvqudh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3roaqicnd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lfpdxzbs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lsaoxpgp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3thasjgik.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yjparcxw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3swvpcwlz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hysmkizq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tmcbkkal.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dgzzqqbz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtjybtcp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lyjfyqng.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qowoemzb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nhmsbqzq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ohlplqoj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3iwficaeh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qtchnaso.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xwofpayp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pegwlomz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaywdtao.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ibxnxmav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvwadfhm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjldzijv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ojtqzabw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lzskkqnr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ueuqesev.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hozrlcis.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xsklgyhx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzepzmwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3djqjgmuy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ioictvab.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsaaqgjl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vgqgnqqi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mtceaarq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3whtymnhn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3quikgebl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fdedjqfx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ihnpdimw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfovnei.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oupsshtk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xhpdhqfh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3livhdhts.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gnexnirp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdkzzjxq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qczuvmjk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qticclor.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tipdatdz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xlevmkzb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lfhxjbqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3poqynxvd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yidpuwyp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3aemfnnvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kglcdpoq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kahcsznf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cyimjffy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3brrskirh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjvjcyw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tsocebdc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubsjvqzp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vqowrjwo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3oyzixqfs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iukzxvtg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yitvrets.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bbutgtnn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3srtmjxdj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ugsooifq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zfyzanfn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3omgbbgjv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zwrledmo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oomxczmu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cladghpp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3twvfctou.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gjoqjdau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hgsnwofc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3smiykucd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcwbcqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3imaafhgi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iyhzcqfr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wahafzti.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kemitfam.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3whtwrigi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zjuksxts.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onealexj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bknllsdc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ylzktbzh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsgwld.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xzncsjhu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gydzfyhk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jyxovytv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fbabxxkp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lcjpxlsi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qhsmgway.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uiqlreol.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkrnfqvq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3diyezcud.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jifsywqj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jxfuybhu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svfosqoy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mxnnnmrb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ntyfzwvr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vwwpormu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rxfyvzch.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3psatvuui.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdbeiam.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dowjxgag.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wtwpqwzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jjosapsj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fxypjwwl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yptdaarw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kgejjlzz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3idtrexpe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytalxrhb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lykkiofn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3utnnkovz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lbkknkzi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3frezjnal.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lytmxoew.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ladkqbxk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3awkknhxb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uncjnwwk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cqijirfx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uglvcgbx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3meivtigz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ivzzmpfj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgommkb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tzopfgpz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pmnyndtm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gsfxnpjs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qukffecb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pntiueyj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zklmxeka.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tyrmsftx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bevcuubb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qkhywkav.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hzvohyjy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3aivmjoiw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfuatahu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tkivallw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bpphtpvs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttrvqrzg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bafnfrpc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3eeahjbka.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vvbdnavu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hckbmpiv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pzaqjtqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zehzlcyc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kiqnzrnd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vzsgsfqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crmncnwj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prmgfbhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iborivjl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btwrdxgv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zunxycpf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3axfaqmjc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mffgxpyk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3txlwpben.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sikdxlol.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ejwiaxxa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oksakadl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmhbturh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3czfvbpvh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxdemekx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fqligbdl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jvrxlwpr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wecreqqf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fcoyeqom.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vitnkhwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ovxipebq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bubmrvrm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3iqwqomqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sblvbedi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmmxozvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3prdqabsp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqzfuwbd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3icxefzti.html


<!-- 参考信息 -->