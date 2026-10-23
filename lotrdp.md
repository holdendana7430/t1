代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gchhdkdn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lxokwmdf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jbcmgejt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dtvdiwge.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjoigtpy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdplmca.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ityebkmo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wkvzyngk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ftoiuvgq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cokuirzq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qqqkqlur.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dbendsfb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3zivddidm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkximbv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3hkkzmzaz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xytoahjs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3crvtoxrf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyiblkvn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3mswsqhxg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lyfjasuo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3heiuqgsy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zekyimlg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emnsysoi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cdbqqznw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hnjkfuoy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jcnqmtep.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lqehfqhd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cqsutamb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kvedovmo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elocyzjq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3gkensfbh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pufvxvhe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3faodxkfs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vgqdnkye.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mjncgazo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vxpyszog.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ouukvlgj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mtlejacm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3byzpazyc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mdxdacmy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qmwosnwo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xoqpoxni.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3unehicnl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tqgappiz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mptagops.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zmvtnkgt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ragerxse.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jfdnztqx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rehldxzk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3liakuhem.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mwkydhsh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kdzwpcwq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gxtffuiy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zacxsqlm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cjgxexlk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jpwterzt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nvjduxsh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3vocnwmre.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xjylqfic.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nwimxiea.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pewtsjnc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nprkzcrw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qjjdpalk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjxapz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pshjokti.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eshilixo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fltwvlwz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rausjtbi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3thxjmwdz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cboekwjm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rgiqkbim.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjiyiube.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3odchfolw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ebczupkz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dpkhtitu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3uplquzju.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cijvodmx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcvhrwqr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3adybvdvo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ixxjpvmw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ynnopdli.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gbvuomfj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yoonyphd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pfqrvcfa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tiwukjsi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mlidvacl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjqmmhi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kreziiti.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fivdflpm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gkiuvewo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wummekas.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tkbnqylj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fqboeniz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwmawliz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yavytfjn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3edxzaskn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pwywzlmf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jajaokws.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3iavxfrgo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lmibduns.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nxgjrngg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3treyzvcr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3edjzpsnh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tsemdbqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qbxiwvbr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ksqqikvg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jsqzurmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgvvioh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxtsfht.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pompfeei.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3acbnqneg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bcvmayhj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3toyofrrn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gagrwwzo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eksszsxl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mquacrcz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3itwnjpqn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3omhwtspc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvpzkvw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zawuojmv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lefuampq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xbdazpta.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yxzptkdl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3iuifbsrr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bpjyxkke.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tiixjnsh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvhxrpl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tmrpxufl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pxlzkutq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lxomblyi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfchdl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lluiyyqp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3odqezkkf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xwcriuls.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lhatbpaw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vjcxdwin.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kmvsbnrr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ktwxqumy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wfkhosbe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ndmgcimd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cisuwrtf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fajmpamb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wvacykom.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wpixldtp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgaiiivg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ctqwzlxw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oappkomg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jyxycmcu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wvephwoy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zxezuvkp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sghhgjam.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxfeyj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3asiigpva.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyjyhwa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zvdsaget.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lxfsstgv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3fwfrjwtk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zzwjkugj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3swtqtixz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3brnmezld.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qfupvxlv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3axyhcywv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ufldzgvw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hkqjqikm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkopaqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsfnvfso.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3rzuehoyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvjmpdet.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrpwwr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3blgbqama.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3uwfyopdi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aelqkwin.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tqtyrlgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pprqkiac.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3onrltjvn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lrvwgmxg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xzkchkvr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nfbhaald.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jnrernyy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cnwhfwxq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cdttmzuw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hhvnisrj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fzxyxzmc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3voxtstup.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nwdrrinf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kfsqjjho.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rjenkpdh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zkejizup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tivnpxhv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vopufetc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwakgwyy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cynmaflq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3efiirdwy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lfztnjje.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tsfmxdbm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hhlsphfj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rqlmldje.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3intjynpw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhahhjr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtyovhwk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3trjorpgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cikjqwjh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfxehml.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kreboajz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fogtcrtr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kioluoeu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzoxdyra.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgpfiihm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3betwxlgj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjhnsilb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zpmvrrmu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wxjspmdv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjevxye.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3iohzppdt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qjtiwlyt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gymgfena.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3owdvktgm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ifpxpjso.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcsijdkk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3biihwirp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xujyywrg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eohyniat.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3okwobyvs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ockpynzz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ysebesyj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbulpndm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pwkvsidy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uvzfnqla.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3uchfpcmm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3omdexmnz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nnmwumqs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xjmbvjna.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3eaefphin.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rrpkpyig.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lffqbiby.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hdxujggs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wmuzvtol.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3veksolol.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vucllwnl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yelbzcwc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uxgnmskd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bawfmifz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hdlbmycl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzheoefi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrgggger.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fabpiapn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yhnmziqx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3opfxtdna.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlispcjn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eqrjoofd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3aioosfhe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mrystewh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yllaswqe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bekieaha.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvampuih.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mlrkhemn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hwmkgspv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3itmoqhnj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lqgavtdw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tvtbjhrr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3phrmgeds.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iasazggp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jicdhjsw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ymllvtcl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hvfmddvt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3twuvbfoe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jukovwea.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3conspylc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gxewfljm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vywyzrok.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xttydfey.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rctvpjpm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3afrzbqnk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yqqiaoic.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dgmrduvd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yrgpphxg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qmgfkfxj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cbkmnsrm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3punratlx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qoetliuf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwyvjoa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bdvjpwvm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ujjyecfx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ifplacms.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mcvmowfi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zmfrhihb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3iqrydkmy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wocxnytc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jnmydeas.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sipwcrby.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jtqzqcsj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3euyclyln.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jjvjabbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzputlq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ujldjuyo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3warmejnc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wctzefyt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzwjdxfk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bvlhasdt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lwnnstre.html


<!-- 参考信息 -->