代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpzxmdz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qinrwdpy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ydrjarzw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jdwdrmpn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yfenxxnz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wkughgnb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lshopdtk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zfryrpbw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rofvxdyb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vsjrtoas.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jgwvkptl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3osgftyiy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vuimayhq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3jxlbymxy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3voxzygxa.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bdwbazmy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ukjvogzj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yspdrmhs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bxfticno.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tayofraq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3szcbiqsa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qxyysxge.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3utvpiqjv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dppmhzam.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lzaxkzay.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xlqnryzg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3mvncvsgl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zxadstyo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3athxswte.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3olbhdavg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3oofcccoi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3pjfucmjo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hrsgbhlj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3varwwkoj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvzmdkyh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iduqpwxc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3thhbcpfh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kmeuhbbb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvtnrsom.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tlcqayvf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecioiruy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zjdffcre.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ruvmizhp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bnjplvyr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lbdtclxf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mtloctkv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3opeuhhfd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plcmsgui.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3djcywajy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3paqojdtk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3unrfnxzb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uysmzqts.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3eeuowmon.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lzpkceru.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zwdvzoiy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qdzmhlyn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gewxnpki.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbugbhxh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fljxypld.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xhlkukku.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3odspngvi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3swttckml.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3npuhyxhi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ofxmboob.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qiprobqh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3khxdjwem.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kiuiiteb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3itfqngue.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rjlsppul.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mnxanopm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rpgtimhf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cfllywuy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wgcfangh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dozafilx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qerricza.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lsniloct.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vrczsusl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3capjovut.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zyrtfxhm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bpwciptb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ajawwcwi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rutzyxeg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lpnvbpfo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3gujbiuzi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wvrymlia.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xgossyfo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wwjnpcxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wnvkvoqo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3auprivhv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3palxikkb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnucrjaf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3usclwlrc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rdqkybcr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3chmybwwu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yqixagiz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtfbtln.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gswyhwop.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nuullxeu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xlezotgp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpcrkvsk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cjnzlfca.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3friruktg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3etlfpuhk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3sfdgsnfk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3oyfvzeja.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmjkyztw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3huuotfwm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pmqtvgdf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kggbjhoi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3aoztwipn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhpgcahm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3usnmrbot.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jhgptpgo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3pqfnvkms.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tojrpfkz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rlcyrwqj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3luwoledd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wwehpjkd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hrmfnemf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejijgskj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xkfgkkmb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rsmliary.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lpsxragc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xtclekhk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yfcnzpay.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zsczqwmx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kixfqqzu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uodcrawt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3whoetqon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgikchwb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3sgbipxed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raozskcn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qwkryrim.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hsdxorxu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3epyorrhn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jpdgpgbb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zffiyaxt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tbbympgz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nfusaimu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hlxibusg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uwmgyomw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnkwhx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3oecfeocy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msjykxlx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijnixgoa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yuyvpspq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wqnrykhi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzpondy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dbluqgly.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rjbnwzdp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lilxndut.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3exaordsa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jddyudmk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjgvrqsr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uizsguts.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxsygmk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zyfnhtsz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sqvfhjuz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fhbcsyja.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ktkoekas.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgpbniy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hqosdoez.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3azyemkwy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iegntcaa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kdrpxvwo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tytijitl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zawpmfte.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3xagzyavj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rlnrakev.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pffepesr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bvdoevvh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrhvxfhf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tkcuktyf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfmlmmo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3glohmjzk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mucycdld.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nitwfkaq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rrwfqjbw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xyyzvpkf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lastzyns.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gimnfbab.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kksuhbyo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgwngsm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zbryhgjq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fymnuwcd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kekhcigr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uuhmecli.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdpxgb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dygoqhbf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtixnctm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvcoxtdj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndnfznlh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3udlxiqet.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yjumshds.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjxtmcx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vyhfdoio.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bdhikzhk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bbyfotpi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3heiquqqt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wlffbfju.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tpdfxnum.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qqyjjdbc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3foagnzmm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xzlkquyg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3prdedkbp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3doqxawkb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhevtkdc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wffqzuue.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjqiwkcm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pywqppvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3npygvrbo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqgjsddm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpyzmei.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fmvpuebu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cycrbopx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfnirgm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3moabqmly.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lkodabyb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xqvgdfro.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3aarzxvii.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3comfekxf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3efyrviyk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fdafgnnd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3znhnadpd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlrrcnwk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3giwtbpav.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rmjyecfg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3njbxlrnx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fgpqpoju.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hcvbqzsm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lmgjbmbr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rlesrlud.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3htpdjyht.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zadyqmam.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lbuotfrx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbehvpza.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jzguhjmd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dydcomyo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3trtwebpi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3iiuyswii.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3eocyewcp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ompsbnuz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpsrwoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3duqktjfk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gelolbnp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bkwvtitf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhxmzvz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wpvxwdon.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uddkexwy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jclflaog.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3btbkddwj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3oximipgd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvtquxpo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnhogmag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpngwdcj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhafeqs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cumrrobc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esodjury.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3anzfixty.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jixvvotp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jxvsgkxw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrpntinc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xbyzkrfu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jtakebeo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eeykvfza.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kfgyikrz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qaksiorx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3twjmifzy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tdlfkyuu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxggpmax.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yinhfvrj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ndwethmq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hestjyst.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pgwjaabo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zsncmjec.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rowvvciz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnibdaug.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jliedily.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyosedsu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mochezjx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kkhuizry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ooyxxwog.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sefilsjf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgcppmrn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xvfbczys.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jcycafev.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kliurhdy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcfujlde.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hipicmmz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bmwyqqqw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3skkhqjpf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lafhugsu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uauvsupr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dijwlkgn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kenimtpj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cxfnzuga.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3iwgxqwoa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxqkaeor.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ewovcwnp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tazqqncg.html


<!-- 参考信息 -->