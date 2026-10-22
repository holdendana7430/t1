代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtguvkm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ssnvoadv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eygtbfuq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qttvvdwm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mterbwvp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sfmgbsmf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2fodztzlj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jminfotu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vhroxmdp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zhdfyxao.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dqxccypf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ycqvyaei.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ttcjuvfo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uyzbaslv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2lthehxyy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rseloqha.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2blzuwxzo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2omfcbxlf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2uuirlsdb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gkhbvrob.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2reqojsrm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tbscjvuv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2doiembdp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2etbwhsmd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2julnalym.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pgaqmkxl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bhqahxty.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2afqndign.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wuyeycts.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bcjsvqge.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2oatmotcf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzexaee.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nqeeedec.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vssbpdmd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bvwioqqy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2yeishsxs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zjgsqeir.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uxrvtbza.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mtwfzdov.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ngcyhcfu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2afbymlbk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2finlwhct.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bejoeuzp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dzlfrmuf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2xlccptht.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ljfstumd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xkvhgqlt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ixmycuog.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vunstzjt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nlxpjjxi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iupsektg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2cyhjiguj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gctxkfpt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vhonlqpw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fbtpqsgi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jkluqcmb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2syzsczid.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jafdnbsh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2depddjxy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ciiebrhd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ovxdolxr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zjaevunh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2sqtiiicl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2usbqwytr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zqvlmlsk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vwhiwquv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2rvfvugco.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2pxxlmtzw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nxzhulkt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lmapcgqg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkyajain.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fnilfgpl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkqfakka.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkotfcer.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ylonqvjo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zeioeehz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ognqaypl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2slzfwkdq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnsihaqx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sdfsnlzq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wnlccxgm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jiufromv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcnghsl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uepgngro.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kpfkqsha.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2krofqupr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rjtjxskx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2tksubtnj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qomxxhwa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtxgkwdt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qwpmjvon.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2tlnmheog.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nvafckex.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gevnhfzn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ihsppgif.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gzqvymld.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lzvopfvz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xlvdplil.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fpbfumre.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2irrhdmdw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xujsjshn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zxjggzvv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2obylpyai.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fmdwptci.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2cenwepmi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2irmoeren.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ylsgllnd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2sgzztqts.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gibyaitv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cyfsvzzr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eqgzzzns.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cehqzdkm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ljaxgice.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vznsnjqz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2norjkbxk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mhiyzazx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qpzkyrnq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mszsoczn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vkbhcxho.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2temthown.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2nzxqhxsl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pvpjtpaj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybtziqqj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmwgapuz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fetxniuo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cdzpwzlr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xjgwasli.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyhmmjl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xuqbserf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zfyvfacm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2khrrdthd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pkwydhxz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pryjhxtu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cniylwqq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ipkhyott.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gbujiwes.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zjsupksv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iitjymyg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jlssewrv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2blmndxbj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2pshjmsho.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fzmggvya.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pbwkubxr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xhszhqxx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ujbtgcmd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2teavzyqj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2knzqlvsw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zpkzcbuj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qlkwmfaj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewammfmm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2iyzgwwlq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kdsedaig.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qpjtlqeu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fuikfbuo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fzbavbrj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2voqgupat.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tuoaeshg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gpkxtgxg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2whmtvgsp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zazcnemb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wesophsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykttovxx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bkbiucop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhhbiuob.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2laehkncw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dclofbrb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkjbyhc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vqyyyevv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wdlvztqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bmgownrj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ahcgrnlz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vpmhwqvz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oaethple.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rqrtqans.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gauhffnu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lgctylhl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rucoixyb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nsdduzah.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ddfgmpba.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdqlqhal.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2oovxouve.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lfhqpfkw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2iqfdljpd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2guszszfl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjlqevui.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tddcidui.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcpfcyc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ojoyldsu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aucafxeh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2faieaozh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vdkfodph.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vxldyipq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zsjemour.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qcjjyxet.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrhpsyl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hibgwyao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jszixesr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2iamqugam.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ypfasgpx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2imzbwjgw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrpsagnv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fkocxtyx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjndopoq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2orcppwjg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rssvywvo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wcjmdgpc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhdxlyh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vwknepfs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncxsjakf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2esxihhaf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ojzfmkth.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rdjjpjtn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2watfaqcp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2golymoxs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kowzhfpc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xekrwuyk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2curadxtl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xtuhdgms.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewqkhrvf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxbvdmys.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ptqmbfjp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxnmhds.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byduzyqo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pptfvaod.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2naikvrlq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnpjnqzh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2orhlmxdw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2eldwbriv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mmwoytdf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vrkgfyww.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nxsaepmm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2leatserr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2skhulhyd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vqbsqboq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uvdlafjv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sywhgque.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2caglicpr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ieibawwc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xzzdgubj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdesknkk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sntkdsmo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvymikue.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zaffmouo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwsuqot.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yijfczdx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kkiyjfby.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kgdsxdku.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2crnktarr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2syznijar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oscceqbi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjtprliu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2obtmcwwi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rnljeyyq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qfbfcigb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ilopdgsw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ywozlodo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lrzvvrkg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ukhizezg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkoxwxgu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lbbybyug.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dawlekzv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rwubbfjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2voetepqc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2amucipqw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2adlfgopi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2smqvsavv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lfdagnli.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2alxzaueb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ettmgrac.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkollcuw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pkboamty.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ltxmtsfz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2srhrmhyc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ympvifim.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fgpurene.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhxbtgi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wimatjkt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vieuvqho.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2szufzviw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lltlcwqo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wyombwlc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wlricfhl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2piluvsdw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2loaygtgk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omzterdp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evmcgycx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ricrgquz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zqtfelzh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tpujmkwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yseteopo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nvpaxvzj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2irggwudn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ftnugjkj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ywhuzcmw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xxkawsfh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcjnhasc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eetdiwmx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vuaasrnq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rmhezobj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ogykyjcv.html


<!-- 参考信息 -->