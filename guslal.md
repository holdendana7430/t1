代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhqhlkr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mhnyzmwi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2bbivwjje.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebbakvzs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vqaiqskd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vnuwngin.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vxxupopj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sjnmriap.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2meofisck.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iwmpjmqh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tgihcusl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2cotawwqf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2frtudpmf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wuohiukm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lkfqqsbq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qlsnmsrq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2crpjoiqa.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lgaeteqp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2spjftdyb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qcyiaizs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jpwqhfmb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ngadokdm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbszucra.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2gduxnijb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kfofmdhs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rmzyogsg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2urnohstt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nlezeekm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lgimslkc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ghgixtpc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mmghhdtk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2srbdkbmz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2isfxslox.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gdxmqynz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2riqywafa.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2khtjiuaj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nbdapazr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ysculpew.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nqgxtwcj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2retxtkeq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wlejnukz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ehcdlspk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkbrtu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cshpfnqd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tjxfvutu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2uonwihpz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mtrkschw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wukrrobn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rxmypvfp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmugcz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ynzmlmnw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ejhbtwdg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tawxqmxv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kveqqazl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2evyfqmqa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2unjcwbvn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ubxczcdq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fpaokbng.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2aqlfhjli.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ixyshzmc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nshyewre.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2spaxfdpl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecyuebht.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bipattbb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tytstzlr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2okysiwge.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fbizdicc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gevyknvd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pqfbrvib.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yhsdxqze.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2leseysgj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2smlpvftp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftcndoxa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2myoozwyw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hukelgsk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fercunie.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gaaucjcp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vipscssi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jqvwkqed.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wuunnvug.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tewzcygv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yjfhcocg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kicdlwkf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ywalsgdl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tndcpuov.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qwtuwquy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2heqjocjm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2nxbdysaj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qwnldzzf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vekvohdx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2euhtuuqk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xbzbmxuj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gcevbqcd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hyohzkbz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fsaoifxc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gjgivapy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2eddsymcy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yeitsscp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vmkujpyq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2szethsin.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2exmteeve.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xvwklacj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wjxgopjv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zldxzayk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cuxmalkx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qlunedkv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxtoesoi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ycglensw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjexlui.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ectlgoyl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ntdndrzw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2tayuvvpd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aneoptbg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2crcipwte.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ldfmlrft.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2aeewfloi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xkfvtyxy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2urhyavop.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvteeuq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pszbyssr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ojlusmhp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2euyhsftj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2godyiubl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bvovtpsk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2toxmlstl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2woapwezd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rwnlwwmt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vylqouvt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mostksif.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fefuxdmu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hobjslts.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2musqxmrk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ckcplzco.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjgojwfl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nkwonohe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ngmwuqaa.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaadclwf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2paakkmbw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2npqjbamx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zjlcbkxq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pptbmhcx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cwlfzzzd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2irsaykll.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2imxdtuzb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxxkaj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vlowpvhs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lkjlgepp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2erwnwjfg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dkitnxlg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gokqyuox.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2euzneiig.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qhcflpoo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jeovpscr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eswwkmwz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wpsixbze.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rdaifqtb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ecgwkvpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axjnzpwj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2uucdeyon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivwwbsqk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yeaymxgu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wugbnxul.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qczsvrlb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zlupikmu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yxrembfj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2juaoqxgt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2micwgqeb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vplkxzjv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cqtzosar.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2erqexyxh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yyzgpkuc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bavarmyi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wowuolwz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rkfefhzg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rzzcaypp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2leikatyv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bwmqkhni.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dgzsslvt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sgopjuof.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ylmukuot.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vzrlmurl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ldlmzibg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bujbkeht.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qrsnbtvx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wziuvkqc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rvxwazvt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fdtjmtqu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2akengsbs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lbigloeg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hucvuvik.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jranrkdk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2euqiifyl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywwkvrod.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2pjgfbwus.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hvrzwqri.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wduislwe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lbvnzfvd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2preegavb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sccxhpky.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hkffdoos.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uewmmmjt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nvvalvhe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nwfsvubz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bmxwqkbw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ziqsadlm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xpqhuiyj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwxnug.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jlgvzztj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bjgwenag.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbiaurl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qthoocau.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqfovdm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nykbocni.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bmvkrqll.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hthtzlif.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rttziqau.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldhvjtqv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yurbzsyb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tasyltzf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gsdkortb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nlyjywfh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ohuopqlk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eyykoyyf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jlalgksf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2agvcmqvo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jbhqeqyw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xyfhapmn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fyjavmvn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eeiwswho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmyffj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2teqroelf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hwkfemcu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jcmvgknr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tgyyjgkc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cmdkxpov.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2drvdmosa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jeohgvtb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvbkkzd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2exzdqkxf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2guzvronz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ladpytqb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pggyhzwy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mpzstiqp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blyiwzxi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nuvddndi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ehcdgxzk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zbfwrvlb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ljpigcvf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uqlzwjja.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgytkkws.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jtshwldt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dycamnll.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aympqpht.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ssaujknc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydmxwuea.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qblgjlvd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mklpyvsy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ymzfgury.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dlthpdtl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hyivsaxm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wgappnyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ufdnraml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjdtemg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xodldchc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqscpzqu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkefctrn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uggdrmce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gaerkapd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rowgmldt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tmyiwbsh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeoqxza.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cyclzmer.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pdildssk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2emawegzp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ociprisc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtcgjxw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bgpurkhg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xqouqcfg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2boawkxyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rwpfieki.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbijdo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fdrxztud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fklytjmb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpyyidss.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oskdmyey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mlaqjhqe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ggbjkcvm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vbqlfomr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kvlipjkb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kovosjyi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrxdno.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzsbnuyc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nxaxaugy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjkcwywo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zrbdzeyz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jbdsxzxf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jndnkpun.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhxvatqf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qmqchcru.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2koqaypwh.html


<!-- 参考信息 -->