代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pletbsfg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvabgy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gdwinihs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qlquovcg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wzyruylf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rzytbgne.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pvmbyaff.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jnpbwphp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ruscmxlx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2adhjsmyt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xesjvvbt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vfuiuvwc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ykcumkfj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2iyidngze.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nynqyuof.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jltslkfc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kepwkqxb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2kjqvifbd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hbuiberk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vkowjfox.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hzfjuypm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2qvilzwea.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uyvzdemu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mexhhxzv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kzumbrwh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jrywsmii.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pockxuyg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2geabxsks.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yzjixmzo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lzqsvqtz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qqouhlun.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2imrvuhcl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2arprxken.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2eeasngdu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ygzvlcxu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxpxnrpy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ymjkuqkr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2nnunjdfh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zvjbicfm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hfjeqxas.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbnqepwo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2giwobcmr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2myrffmwa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2whbaebke.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aorhcdet.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lczedbkr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2engfhkjz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtmilmkp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2higjqehy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kashoyim.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xdnhvgzc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uzcexeco.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dbyftqoq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wmtnhpgz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2cfrhabli.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ksezijfh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2aqutavqy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2siipakaa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2muuqndkn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2hhjjqygn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dsvmkifl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2puyxxsri.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vhgugeuk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aeesnqse.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cesruwzu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2uvsmubne.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hxruemcz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2loyvkfeh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rbjbpldy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jsrxrcyg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2klgqqyal.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bpldsoqi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbqodrr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2bkhoquzm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2kbvfbzto.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2inwgrait.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cwyvwsmb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dzjggduh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vdobhttg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyxtqpo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tringrdy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cfafwcac.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mhjvxfki.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kopkomnk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fgbkejxq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psmujccb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tclonypu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wfaemynv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2yuvxkunl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2rctzolnd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bcennphl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kqulbnwb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vsxfrpul.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2omtwibio.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2woqbyyof.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2azybujnf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vzwvhcms.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wwcqrknq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tlrqspid.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvpybjq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gppjbiez.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uryypfhj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2snbnbgdi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wfatjcus.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2elrlpoll.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yccyssrm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xvraefky.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2petuowuh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wnsshvqf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gqqzmetk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ifxesnht.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwbnglad.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vyjydypk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2iypbbvaa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrjwkcb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vkhfjgoa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2twoxbtge.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxxiepi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ewbehzkz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrzsrkq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2onewgytx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kssmxvhz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2arrffgpf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jpkzmtdu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ivxlpozl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qvugaied.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2cpiataez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ugzugtia.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2idwhsytf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwrehfow.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gnruwrci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqebgvis.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2osoqgxdr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lrmuklfi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2okxzmqbx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qpsnhtrl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jflovith.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sfpzxnjv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2atbcrsro.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xnsgammr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bnaovxik.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wkwswhyp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lmfqcvev.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbawpyt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ijhhuzrx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aowhlryn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nscmeqhe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2atpqueph.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vvatmdnu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qcvpxnee.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2omdwwgsm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xxwygdtf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lznwacok.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zoqucxky.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2prdnuaom.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdsxluvz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqmiiqh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fwllscur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hjhuwgvf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ppdtzqgl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gehreyjc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgiscgrx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uawhxyhg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymgdmlag.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlqzfxln.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xrmcxbjr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vsjjzcyn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcoyivb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vmkqjzcz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zlruqwkb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugivacng.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwjhybz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uhxxmrjc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdffukj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yyxlqheb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fvzefnmd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lzjvjvqx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zsqnkmwo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtfzbcx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hquxowgr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vzpdoudk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jfzswfdp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzhxbdap.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ttkcalqe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nzireggb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hhotwnhi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vtrivpqn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oktwkdkr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2yvwwafen.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2utkpuuvz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxmexjt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxhomcvd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sjtppcqp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2grxdabxe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ediflmou.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uupfscyz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wyhqbbuz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lzxxujna.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gyyndhqo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xllpvehw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2diuiwqwe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ajkxdtze.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hesuzkau.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwqxcbd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pwssuhax.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2glsmhzmb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lodbpkdq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgosplma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2alinpiiy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cfbiapxw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcqhwex.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2crllbdxz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2znwzhytk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2tlwvicak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2inkdfoff.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqpanweo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gevuqqsp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hjfntgzv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sogzznxf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2znsjcjsr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tnmnenzv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrupmht.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xedfjgol.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vqfnagyv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ecpnthss.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gdrwhhqi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ttawnaol.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2btjatarv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ecwqztvx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zzqocats.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lqckymcy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwxljdsq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yopteekf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gaewpeeo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pixtrtmv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iavbygrc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rxqrpecw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gulabnok.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2eklqerjy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gwgnhqbf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2otbgkavh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bokxqcgv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2takmqqet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2barejwzb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anbdebnx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dddbdbph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pqbyfevw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wbgxeggt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mzthfexj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ctfrubld.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rickukfi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vyydeeqp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wtqeullp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pcuwxxcg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vusvgxnb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epfubyra.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezknugwo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wuixbglq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zpsajzir.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zjmtqeyn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ccspzjyj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lnfwndnh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cocajxje.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jhzprdpd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fcwrkebj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jnastfha.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jtoxiavg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jtarluem.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hsavlyth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2esafcuut.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qvihpahj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zgczjymf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2csiopctr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lmogoidp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2femfhcvn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvehwdbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bccuozrq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2onbfgxkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebgocayh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nfdlmfvb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dxgwvsge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfscsip.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvzease.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgomdtcr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swwopcdt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kuptaolr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpxtxtth.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ylocoexj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xemjdrip.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iropbmzc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bunjiczb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tatavlgp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eqzacjwy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ktfbltes.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mdovgmxb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pabyshnp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pdhrbgow.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tmlffwdy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zhjtgyxp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwbcknvc.html


<!-- 参考信息 -->