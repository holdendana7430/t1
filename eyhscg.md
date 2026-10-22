代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mdweumlx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2swerfppi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kzvxzjun.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jiunlqza.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2konbxyyq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xvgpjoqh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vzblfdcp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lintzoac.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2alhzxccr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2brmocehu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2auezujtr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dchwbvdz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wthpwnni.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bmkvqewo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eilbgxos.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeuvdqn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jwjvpsdw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2frjkorum.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pngjnlds.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hlwdsxds.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ktmsjoaw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bnfebezq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2onbvavrt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rraukrfh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xdgqhgyp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jfdkupuh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pruzbyny.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mreifmxj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2eigakwbh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dvbpiqow.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2otyfenkp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lnkyhber.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2stfkmpel.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2uxupwboo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2doorczxl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kjjhgwxy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ufrnrljm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2clkoixpd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uujpifyw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2frbpcahw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nidcfsab.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2brzunexj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jeuanxkk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ymccvkdr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2udypgcvs.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aujyxxxh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ewpndebp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qakaqxqj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kvxtkjzl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2darnxhkm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2yonaslcf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dbuzxdcb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ifosnduw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vngkzrqu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugzpcymr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qrbkydqe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oakbonxf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2utaektic.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sgybaizz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryspyugq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bpglgjff.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpipsdbh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwtmsulh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hoppbllr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tjtdsxye.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lwipoxgz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nziyupzc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ottxaucy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qmlucqtr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2xljbinpj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ufdtzmkj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ptxerjmo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2yqsnqhpf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ctfmxaoh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2aceddspz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2hltyfktu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wynekxyz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uxkaycfb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qghqbnpk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kgsjpiua.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qxmcwlph.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jougpjyz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vfjgacsa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lxafmtyv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mgwzqevi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qorzeutf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wlbmxrwt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nuozyxfq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qiylctwp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jirjvziz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2beyuvsyu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wisbcvkk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnqleorj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqaxfcm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nttnknvv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hllmalye.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gctcvmfs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2syxhusps.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xfafexql.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dqgtecgx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gslsglom.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhzypny.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2uxqfxlnc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ecnltynt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2shmwzala.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dtthkngt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzgxszrn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rwumxfdu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wmrnbhjx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kxaattvj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2swserqtn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnvtydj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cmelfhue.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cupzzzdh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vuskxekh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2yhzfbeca.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nuxqysis.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2itakwvkf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dcmspiqe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nwfrehkh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ehlmhkar.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yltricji.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uvdtuqmn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2idlsxmri.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ogamopia.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vdeszobd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lryvjhcs.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixcfftjx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bstvcdgw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yjawllze.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2reusbjqd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtjhnrm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2edntvuec.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gqeqyipu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2uwfeacdc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kdspoepk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2owzjolkk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ocqnnqvk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2rygrreba.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cfjugvwr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nwzpxpgw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2srirktor.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfsilngs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wrmyylzu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fjvpwvuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idcashtv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zfmkpgsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekyuryyj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gcnvzpsw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yfxbvjfy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyeigqvg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2afhlesna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2opayxfgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cmtfxjjt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvedeivd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wydtfyro.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cxtxurok.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ssimgort.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2orhqxoxv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pazaxfvc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2euajiisp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2heeglqaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ifxhcili.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xaapwtzl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xttmdjee.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2altoeigq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ejriably.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dtirsmet.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pobnoneg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnjftxyi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rosemgtd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yjlixjhl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cotoqfgn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vfxqbwuk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fcphupjx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rkjexhsr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uwgrkjih.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkrblxgu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwqyhwx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzemblxt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhragus.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2npbhygot.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2bdwvotld.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bdgolfvl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hcimdmfi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fpyvgqrq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyeeitpi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sragxxta.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oefwpftz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cceppxdn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ruqrnctp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ijlnocvo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mwhlavwf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2njduhmwm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2sfxqbsjn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lgiembvz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nnhgzmrs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucijkuua.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2axlhritv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jrdgrwas.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kafgxsqa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xzljrxxf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnwryxde.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvbbjdve.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmowqyoc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmxcsda.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jzltkgda.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdaofgo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wxqbsjdy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eialjqlq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gppakqxu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mezyrkxw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hfrchpgc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jirqmjlh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xzirjvop.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzvrsaww.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cjihvwrl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntvgooxo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sdcjevdz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eoshxxoj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yvaygtfs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qcmmxqpw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gozqdeqx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzjxdktg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdxxafz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2abfzkttd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2catvloqs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gugvyktp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nkxwodyy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dnjavfaz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zbwqomao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2idinjffm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ffcqyozu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pjmcsxiy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bquxfhas.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwcjjzhn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rjsqlyyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtigkioq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bpingnue.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bytthzsl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2exygbqcy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xrzjckfr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqsophf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2scykenze.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ykmgvymz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wwvyizjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrgyznah.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tsrxfxca.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tnsjmtmx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kzhiicyb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uuevqwml.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cdfutgvf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xfwszicg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zmdwxbqw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xeipbeua.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bezhwogd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2igjzupfp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ssfrfgav.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xczoxguy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uixmsbld.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bxwpohpf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yrketyhc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ygtutpxi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdeotsw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jcucqjhu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tefvhnli.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cacxrmvg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjlaimv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swzhbljq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brmqshmh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ozousgdq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vssdujlq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfsuwvq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkazksdq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ismmfujm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zlsigmcr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2proyjpqr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vbfohdia.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xnydnjvo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oukqmyxw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jsdaxomm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tgibfesf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gaohigmw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhhqdgwo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kurjbgtf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fqptusmt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bbjqfrqa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jiqsceia.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tugntoui.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ztfbhjka.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bswsyqxi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2guluuien.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlztvfqf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rwpytvlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzknetpd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cozrxamf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iiorzsqz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mhmfygza.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rpikxrkp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhdvhr.html


<!-- 参考信息 -->