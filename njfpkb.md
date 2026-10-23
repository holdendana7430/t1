代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsbivafr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jaatemlq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xtqjdoli.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mjkminjz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3saopdkoe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xodnldmn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3skupivwr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pxwdngdy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xarsvvgu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gqgzjpyq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3krmkgjdk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3midvyvfv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lrqvvzan.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gpqcbvbw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ornjwazu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ahwvtvts.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qetxrusa.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3owjxvzxv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3czegvybv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gjuvxvlk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evzrozqq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ugdatjgy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wtlykbwe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3frcsturi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxkkdvqr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3euojhsay.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pppfeyde.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3byzbbvzw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3egnntbao.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dflzzvhs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qbgdedxa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zynndzss.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ncrrsgrv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gwewyogq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3torrfdot.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3orvbfciv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qigkisds.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hfqzxywr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ctabyacs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3zhkgdtoz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gdcseuyg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qobktwur.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ktwjbdqr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jxrbotfa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3okvztkxc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3btpbnlli.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qyzokrjr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3eckpfduc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jxwmzxvt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iyjfsibl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjedim.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3mxbzzjmr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jflazufh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3lkarmhjq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vcqzsugy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3opsklqbd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qaptlszr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3frotoedp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ahtkaaik.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3hazmwikl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gcztgagp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3thkktuug.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wgjcprgk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3panvmvai.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlldtdie.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gprtwhid.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kajpxdtx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwvkjnux.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yngcexli.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3posgqqad.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gfhavpsk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lycfblpw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3toincszp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bmxksrrf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lwcjcbka.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xlxpzltm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3nwfbunas.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3fyebwjti.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eylvefcz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tdruzkmg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xofnykil.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3otsmzlgz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hbupuuox.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dmvmwsti.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rubachmy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3etlgrvno.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mxrqklmf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qpjevbok.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3bzciyolt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ofkzccbh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vbfwtdmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tiomzpwv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nmzbivjt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3amultnhm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3eitmrqzb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtbthvsy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qgtqoplc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zmusolik.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfeaqjn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odazrhlk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zchnjtax.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbulmuu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pjplodlx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jsmhital.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mfkxmgvw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfmnflzz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jnlkogti.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3obvnhyib.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgpuqsmd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ciomxhbk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzkqrhts.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3znersbsb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qwjgfrbj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dzzazymw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3oaanwlgx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ekrevlzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gscykper.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3avcblbzr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ghiztows.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfwgfyd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uwecluwe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wrshmwng.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3putxyyuh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3khrddatm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jdgchrcm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmkrmsig.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3myknojpo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xtkvxfss.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nrlafwke.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vkylpvqk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vxobejcc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3umfvtlkw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sqwlvkph.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3csftsrdk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aewdwoxo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xantbsco.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3musoskot.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rrdseoiv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mqtidigl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbsrlwx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wfxeijdw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3weknoceb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wubmbapz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3huswxuhw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3vjsprdfh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nunrkgxi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hriepqkk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bgdhkdor.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xhezsywp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hndarzgw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3miqsolgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhdoxefm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lhtbtgea.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lmedsmlb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubdklgug.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aiskgeyl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ynedjijv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xyhiwdsq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dtbpdtyu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3odebnhdx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cmjjrzyz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ntmsahgd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3yakmjpnd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3dkqqvxyy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zqoomauq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3adfcdzkb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ghttfcdy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jcxbmcvi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qifizxnv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vstujuyy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3izurswlg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xwjlnrfn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gmaeyywe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3abunvmib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3efipdkyx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fyurzdck.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3drrmrtqx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3drvdxmos.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lhvkgtsh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sdpzjcnu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3poxgmwgg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eshqkqqo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xnivwrox.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xurtigzc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jcdsuvob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tnespzgg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3umcbkxyx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qqhtefpn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eenldefo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jdkqbkum.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kyqqtypb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wnrsgock.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tzhkjlok.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqrlunxw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3olgbfzzd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qzczaogg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ydgkqzjf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3oigfgogx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3twlquyfy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yvajchck.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rwfovcse.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqzjcaq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlysdgs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tazmcduw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wrschjow.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ygvbdaxo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3moszbfxf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kfaopodh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrswvfxw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jctxddmh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3reykaedk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kuihmxaa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fmhulqxg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ncrkwqfn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiutyngq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kjnfudys.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3culiktly.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hnpodiux.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wcerhuiu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tijzsdbe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lmtgbjyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxycujqw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gxnkymux.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3khzgqrjv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3drouqajl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3scfhfjfp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rjzqiuix.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kgdtxizf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjfhzjok.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gilgcygv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3utxehyih.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tgsgsked.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wwszfczv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vvwljdpf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3acaszvuk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qtbboxvp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3htxymtew.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iwjsbctr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbchuwca.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qctqwyxb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kufohqdn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ltltqftc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pmsiebtf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kaoiytma.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ljacopzr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3djsjvhuh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uuvbxkaz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jnfbfmac.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dymtgrhi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vyxzpedu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3haprcucy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kitmarjj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zrnrxpcu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qffdoduk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3neuguitk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jhdrpsmu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3umgqrhbw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3diyollnx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ammxulbe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gjzviwdr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sxzhtiob.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nchpchwe.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrsucbt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrivuorb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cibhyfpm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ljhnlvor.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfnvusx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kufyvpjp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wnzyytkd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vjiamqis.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xqflelkr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xfgacmtv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygiggjpj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bipzpxcy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjfgnoy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ziiynwmd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3avlbayej.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asvjcobx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yerwwvsd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zcnykqxm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rqieycmy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rygomatj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jmwpfihg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ifrqzevc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mtrkmczr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ucxynvmu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wveszuar.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ljqqddim.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3apybqvyz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3geejwvsp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbfkbzfp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uiomtklt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bmalvbto.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vrvnrzpd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zznfksbc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ddytipaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfumaflr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wiudibgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiqwhxse.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cybgywqd.html


<!-- 参考信息 -->