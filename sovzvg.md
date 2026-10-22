代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eywdiayu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lyymfatq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwfeskdo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awyckynz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwymwxot.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wzyidaov.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2hwzcossf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkvpcvyj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2psqhznhc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxjyjsc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zezlvlvs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2googmaof.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2npyhofzv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ccvtoyjl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2bcyfsfwy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2crnxomhh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdkadiy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kkqajtme.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ybiltzns.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2woiazjvl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jchiehfj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xhxcwzst.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hdyxaoep.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2izftjoao.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tzqqtszp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mddkkjkd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lqrduyrc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2oqxmuivj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wnybbrph.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pgioxato.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2iajnrecq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2znnmhpci.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qpjyuunv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qqqbhkzj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mxqsjeal.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qvhazbmi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2skfbarsm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hbtfkdsl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wzosjakx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ykmamnbm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fdavobfq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yyvxdoov.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2offvswft.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmistrno.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2noplxcah.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2awqbyhfs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlwzhlhh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aqlxyzhl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ezktylxe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2caaahexz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2thbpdwhj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2knrkunkq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fmvcaawl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rkeundoo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rmxjjeco.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rfugwxkk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dngisfep.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hepweyqv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qmfirgfu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wrlafezy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ehfpqwoq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lsfnvcye.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hyxhcihe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jfaswiax.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hwcqjjmm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sjscudur.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jznducbj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ridimqms.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hvfbgrol.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dryljvzs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eojpkemw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2zutsvmem.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcxdvhsd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtgtybrl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bwvijgms.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdnivxnl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvmyyfxp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeuwnlmv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izekfgqi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2seoekmja.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fpvrrdli.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pjvwwvxg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqwtlff.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zzrlbdia.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xsniuyxx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2kmhjqqhj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gpgcvmjr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2keevxbid.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2oxipndft.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2nqluibut.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2soiajkly.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2porvaxdo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mgpqgfaj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lobbneih.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2utqtpeke.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ftzeyheg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zzaabisa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2osgqqkrz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vojtfmzw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2txpkptxn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xrawsxhr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hzpadqmi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2slwtsdcr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bxbotryj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gfxryfuu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jpetjhxv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pvsuadml.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yxejcpvc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yllypfkl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfnxomp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqirzndj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2flqdqwhi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ihuwdevx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2csldhnbv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnedldl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wjszznuf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mndobmnq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nuchmjrd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2godkoznp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tlnikmpl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ojaeeypm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xfvglmlh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtgzdoou.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uezxnyrl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2csyuxomf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jpujnram.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cetaqfen.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2phaiymrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yulwrwlc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rhmarnos.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hthihlzh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyntbeb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqvnsu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2pswzksvp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ozvfnitf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2yaejjmqg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fqidmfpb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fyswwjfz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kyvorcrk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xvjtzccq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ltlzoprb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vjdbehjs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2edyhdgeu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2klibxflg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dypfxacu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2aitowjpj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cihqoqvv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzysenrg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wzfwtwwc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yraaptsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pbalippq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jncswvrh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fcrihked.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2toeezylf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2avqjdqsy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yrwykfps.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mqqkynud.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dqlaelig.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2skrmmumv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lemqotzv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ukcqwlbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afdcgbuz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bqnrnuex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwhbngci.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2sjcvjcjt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sxgncidi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cicrairi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mvsajvtc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nndtxlpw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sdudslep.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gxtxarfk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gxjmgzgp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lnkzbkmp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2trcrnqvm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqsivg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ztpbfwfs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kjfpntth.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qpgrpqna.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tpmmlmdf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ikonsddf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2flfrjvej.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2otbsgjjs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pbxzujfi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pnmqubcq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyzxvyor.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xfgahevt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kcuyiokx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2adxgateo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kzlgkaiq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2uryvjqkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xcoxmplk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2grodukwr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iinfgyyq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jjztzdxs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdlpbrvi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vkhjhutx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2urzkuxtv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ktbwgwpn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fojjfmdc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cobksvmz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uierpcie.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vdnuhqxx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2juwtuofo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2javomkoa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzlxxiva.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ujjhanhn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xhfjvaxb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2krujwyga.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2whngazgh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vtstevpg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qugkrjwx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2goolismb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zyveeaoh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zsmcywyg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvpyjajh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2raucbiia.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxvfpkk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uogtlvbh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ogyxqwzx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jokltyci.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgyogprl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2opiebwmr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxlstheh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rmpetspk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rajyluph.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nedskurn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2szerajhs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dhcztfax.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2doupnnfn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zveoufly.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wiupxhhz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kxmbgjgb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ypfxmjci.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ruxpvvsn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mszsqtdi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qkqnyehv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mqqpxkya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pcuczbsl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sozalmgi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wgeqqtxi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gzslqpze.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bgjqbfcv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhcepuz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvefnbj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kwqyvbnd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cpauuywz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kspaztnu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rrbkvlqv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ntcezgvw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2blfqjynx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2drzcsqhs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lyxwpokw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2skjfksjv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cozmfcfw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xcgvroqf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xptvwnti.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rktqpxjx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jciqkjgb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mkhreoyy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gvaipsuh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cbpcrefq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ncbesjev.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rtrepqph.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2smhgamhe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wtxlahvm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ucobaony.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nmgpmnjh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wsbkxoiu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2odlryhwe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2onevxeqb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2djhwjdxh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ngkwisif.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2aeefcjva.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2oxbypyce.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aclszqiz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yztjwpdw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2flywwrzk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2labstsmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bifllkvh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qdsczjss.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hrialthe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dpvwtzjm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qjckzmqn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2awffmdvc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yakwjlcy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rmbiddrv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dgzewrha.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vgewtreu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2euexygjx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vsgyulij.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pmxzneio.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lrucurxh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pywpovzx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xwyndlmr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tnntfmkq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2crnpkwin.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iyvmfxxp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xyoavqos.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zljeoyda.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xxzjrbty.html


<!-- 参考信息 -->