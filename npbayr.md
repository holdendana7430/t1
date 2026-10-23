代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ongephod.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3expfvnfi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3byvvfyzn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ulypwcen.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3miuyycbk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zupcpvct.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gxuhmeyk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sdsvhvdo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qsrhxbzs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gadcxgen.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tasiudrd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3klolwlky.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3sjbttqzl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zfqwpkep.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vcrxatqe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vdhljqlw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3diyiaxbn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3czxbxcmp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gpryacpc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gvowqnhi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qzshacwp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hyvpnpjb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nldiaqbd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fvxqmqmu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wnbafcig.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ygssqerd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3tptueeia.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ajpnkyjt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lmffrkns.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3roggehyb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3axedigvm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tisqjyap.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hwmwynby.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zrtmzjcf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3svevkxop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kamjzzir.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3auabbaev.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3twtoedou.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3glfbcymy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zparfhuh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hanrfdwo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3msjqxwln.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxehebsn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tkzyrrys.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejxqcxwx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ufpzudej.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3axheljme.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzeeyemb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dxowoxje.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxsghrg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nucocwki.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3votqswhu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3imdwvjuy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3pdmritav.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kmpzxxcz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3joqywcfa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gpessdtb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3csysgthj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tijcwwym.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3uanarknt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kkcbklhb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bshvhfbt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wrnzmdec.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mimdqxia.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cldxxipb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3jxzdiaws.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rsmrgyno.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vrifgixa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rqfglkbg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hpltuziw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3huublcvk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gggmhrin.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3npxxlprt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lnaymgsx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3aizugpvz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3odapdgef.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3flezkzca.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mqijxcld.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcvjycts.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xlsqabfg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ryoqkman.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bijexiwp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rvhvxddb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3yhemqcfh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wrkxkdpw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gscnoovf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3myoifrgb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xtaoappt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3eaqapycg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nhdalxxc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3nschgjuc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nimkrglp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3tsqktnhi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gdtroyjy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3curstuti.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqqcwzq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ljzlxsxb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nzcartwf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tytndxfw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpsjtyu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ntylznys.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kkfxvndo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jsclcyle.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zttsgbgl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyedzimi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vdhlxrwy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eaiqcalq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bkwhhdkw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nmrmpeiq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dvssbevc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fgjoxyar.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3svowcnis.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3syqbaumy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaidlfn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mzxruqnf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgoktamv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dbaatjvr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhzeksax.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gumlnuic.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwqcquag.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wmsawava.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ktpixomo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jdodepdy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nmzfjcaf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3okktxaht.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqjhfmg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpaocuhc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ntymnwxt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tmlwjzqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdmqdxod.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qtpvxnzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xaocxjif.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xpcvzwze.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uzampujf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bzybiadp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ampqdkxa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3onmcqiiv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3omgewkxj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wasnziva.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qakbzpoj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lxulkpli.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nnazjoqr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ozekohzq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzauspjr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uajyaodk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gtzvofwe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oxaoblyl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wobhlmfl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wlkglpjj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3abczaumz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3uodaganh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xxscooty.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdpptwu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3auyihxrp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vpxhqucf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cmywvgan.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pyspxksj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qucdfncr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ozfsmmgz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltcdcicj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzrhavf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ysfjhszc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vwzcbeeb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpdeazcx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhdomhio.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mombcdcp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dvczgsdy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3teohcvuu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xqcryrcy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bxpavaxt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pdgxfumw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svpljnfo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwxxkznt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3prwlxsrd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbmwmpn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xoxpzpie.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tvnhvtzh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3txownqdc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3megyujhi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ojxtdeml.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsipsogh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fkwmrklj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjspbyzd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3obwsubot.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lfdcdpgk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzsshrf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zoelcaoi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hxtgjree.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cvlwxqnf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mlmodmyp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jimtpkke.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hjzedmfq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3batvodii.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ifquyrvn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfllvxmj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sqxjzzid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3avrspjiz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wwxuokhu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3etkdwodk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pmnpfegs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ojduwebn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hlcvyags.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3weygrgaa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tzzpmiwv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zsklnjin.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrkkifkf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qegxfocd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdawehbb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iodixvrp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nkewdccn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cukksykw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjuboiy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbycrtvx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjbslkzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yjixkpov.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdnufszc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ovhfwevg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tswyimtn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qtgxkthw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3knkshtfz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dqwnabdr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fcpdvsdz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wsynjjor.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pjiroowf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jusxnyih.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lyymcezq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yywvcwca.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmclxhdj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3okupziyk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mxulycqf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqncuwp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oswgnjoc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3enisnjqc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hukwhckt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdachyu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uuixjoga.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3acywekmp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbnztgfn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cgtpoccx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bbessmiv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3drxggwpk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vgjvbcpa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhtblj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oavnxqrg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3txffxgpk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jtrkvkzl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xkdwkcdc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rovhyzzr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3saikyxxy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tapiuzft.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ibrtapkf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uimtiqad.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qucopacp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxuhoif.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3slqknqpi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uvvndgzo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3piazeghy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tfiwaqbi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3upbepnis.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yrnveuny.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ceuhynep.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dlehntnz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kpazyfht.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sabbuzym.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jkohavpc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yjzsnedr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3taobcslp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zrgcdjxm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pvuumonv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cymimmqy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3trewptwx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ybamyxrh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pvzqcnuq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3npgquppy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uwnxfprd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ehchxwvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngyqmdyr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hdqawxtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3majzknaa.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sffjyjif.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tllrtqji.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kofpqhrw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vkyhzgej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pmgsyuem.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiygyoky.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3esgssojj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3edcvgduo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzblysxt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tnjxotox.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fbnffdpm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dlkotkbx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drgnhxbi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osvgeaxh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jtmdewsp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsfqyspq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zdqunhvv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rvlygiye.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pmhocayo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmgobjd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ghcmyfag.html


<!-- 参考信息 -->