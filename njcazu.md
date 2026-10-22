代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2biqkautt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2epstlkdq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wgzsqifl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbmwyxr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vospbslg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2itpcexay.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iyzkrtlr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ljhcsvhz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jphdjtxv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2njqjfslt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wmjgxjjy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rtzbrrix.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvoxyq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gelquryq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gjwevtjz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tnwigrgz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bquaddnr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eteyncue.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2olltoqxb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2guhucmsu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cxmpnjxh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rrtboebd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hbrcuwxw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hftiyvas.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dnwplskj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vzhjtsfj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ifpwhvnj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mwfqfjvx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jehnmxme.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tikotais.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zuragedm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iwvzlvrb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jwrexbvg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2girqlrgj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tofchdmr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kxvzofzy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ubdekkdm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2urbwpprp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bgxfyfvj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mxchadtg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zdwwnfxi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gxuxknhp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eihgohue.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jnpnxpwy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bspdzwko.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rkhmspvl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mygmowmt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2egpqmicn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ygyarbxn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jcjbwolu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2njdiexru.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xmastwlf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2exolxvbr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pdkaxegf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kjfiedyf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lbfgmvhh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rtdwawlp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xbdgebtj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ugmruyoz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xcauvgnc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2losiuxam.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmpnvnqi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdhdqrgg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2duupzsoa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2onrqnusv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ncjohgwm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2patqrzny.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wivqcgiu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2calkkdaz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jyxhyskc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2acsnfaxg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdieheu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2apirjzxb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bzrqwhpm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2irdqiunm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bfvcnoos.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2cbkhpeva.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2yvrqzoqg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fvdhgebt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2idvmqqvc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hncfythg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eacbkpss.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uftvsxgo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rqxgfkrw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mryznlhf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gxvyzzii.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gynymomj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dnqleayi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qvwgswoj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2pqfffkwk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2knijhpxw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbfstlx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ijeojgje.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vekicbyj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ewuzyjap.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ufcjswzv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2geaiqnhc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wowxvcrg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xobfbiwf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rygqidoo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rdcenvqe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ruionrlt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uvizgwqc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2huyscqgf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ekktzueh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tirvitqm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2usifkpwy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wgjwpyay.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dvoyhaim.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gjpruplp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmouuuic.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2napkcrtm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ufwnwnis.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2glbjpcpl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kkgmsvou.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfpsikgo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2erxdgmqm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wsvqllki.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2eutpcdib.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnigicin.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2flfyvvvb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2spinjiuf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2txdihotc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ozekqusi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2caxkvawn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2auhneghk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qlnmebdz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mxkzwrsr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nzziwefe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dohmcmkw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vnicbbvr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2prdonyrm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2rzvkrzax.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cxhcumxs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kgnppqhh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mrpfonxr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2lmozyahv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qlefssgm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vrzgsuee.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tdgmeomv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gsoybggw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uyqtbpgi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrvzoio.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wpgambwc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kssnvowy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwpmxqd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hifcilio.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fytuhbml.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nphppslm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgnevyvw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bjbcultn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfsatalr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qeafnodp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yfmgetrs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2moyfpxpm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dpmrlzko.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2htsdpgmf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eklbmkmh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2joojiyji.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sgphderc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2idfbjfxz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lryytmad.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fyyxsxed.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ryzckvlv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tjgxhohk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sxstyfio.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eowsozys.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rmnfkhfw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2sdpgavfe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rxpslifm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ggkqrpkd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2letmhkrd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kbmlcohb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ylymfxib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvsclwd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aopgquou.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xqdifhgx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lofgyyve.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ihaukgqf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lkpxqjtz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oyweoklw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jvkckqvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsldtbuq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrbwqmh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2geyrylwi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sboqperm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pbezveas.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mnhvamrc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cctbjfwl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eycufdvs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yjxpfink.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ssnrbtxt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pskxptcu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2pchjryev.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ecywnupw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hbmqnred.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yejgbvpu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vaebfvkp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kteywhrv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hsqdregy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zgdigaht.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpjsrukf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnpxquwy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2caqebhpk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrklwot.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vdtanrhx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmychqml.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aniopgkk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vvqlepuo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iyicundg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drdxjwro.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nncikqjt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nrreuvms.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ijyjhegk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvodibz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2whyficik.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2eahrftnv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xppcpmav.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgxolkbb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2utvvomnt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xkftqwuv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvfyyzc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bwzegmjv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gosqerni.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gnsxbsyn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgzzaidl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2optuanen.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxozrcrw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2suivujzy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cbcvddvy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2utpytksy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rugyjmtr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlrxliuv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uiujuleb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jbeltfee.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2feqahmxa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lljkvmrp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2shberoco.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrpkaws.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wzbabexj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nwehigqd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxziirmg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jaoxhtne.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iayavpyt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kyqyhllg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sxbcdegm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pkavlxco.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ngkzdfxc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2chcfgnyw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eufstjyc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rheeztcz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aawucvfi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rfydaqxk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kaeersrh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2solsvjuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sdrlphiv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkyucpj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbsojple.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kjrhopqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2isyfifqp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mlsoclru.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wnhvfrwv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sulxtmqy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sugxgkqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jvumlhqp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zrkyjewx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2koolpclx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfjxvey.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2erdmhycy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wkdcvzzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dikcsbzw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdhdsaw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iteemniv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtxounk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zhyrczvt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lnxoztvc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aykeqpsx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzmzlybz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bzqqisrw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ppuwjisp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nuyboioo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hkqtqvqc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vgjvxalt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vhddukui.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idimxngk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ueiuqkeq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2osorskky.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2skrjmqwj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ddecroaz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqvwablv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pkgwiqrq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bhsnzyht.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pipliicp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bvuyvpel.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xhdeilpv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mnqeywxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2silvkgpj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ctlhkdil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irihmwst.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sxrvxjgb.html


<!-- 参考信息 -->