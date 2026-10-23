代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nfwfwxuk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fjgetpqr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gfrnnypy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uaohbiay.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hphjyuqw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3guqoxxmx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3szdbsueh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sstcjcro.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pdhbcerj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jovrqrns.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xmvuhyai.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3krxouhoo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3icsddbst.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlgjhmi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aqvnnyqv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvgyoxsp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eqtnwzay.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3oesjdvjq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3szvuckmi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjvsisu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ovtbwcld.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3djcqdsct.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ktzipadq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lvptzqaa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qfbuwpcx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hfmtbvvf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3iezenlzm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rohnajgi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ijhwmbqx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fpdgodxa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fiviqnjg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dtdaysds.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cgxphjnm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ouhirkjq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fkbobxqw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qqvehhas.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uceaaeqo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qfjrgxfo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3cmfundnd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rimpprgk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fprkhmkz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3veyjnhpn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gyavwfoy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cprubfap.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gzupnxzk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3osyxaoef.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jbslhaib.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gkjgsfdv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3inhjbyrn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ifkmsekd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3snqirqon.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ftjqclcj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3efoiujfz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkaboqdo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bkynvrda.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3edyfwssk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nkfukyje.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qwtbjssx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3agyrtcam.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oxweojed.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3blvxmwyz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3kpmgtlzi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lnfozufw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3sxfphtfr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wnxeehiy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yfuckmdu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3acnleayx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3boacvhtl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xokzcdui.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aerkclaa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fozvoqsl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3czzadezp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3txnatfvc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rbmngtfs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vhsfiztn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qipafvwz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3blgfbpgs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ubqpfsgn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzkrpcan.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddgntjou.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nxtadzbb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ahuzobto.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kheanltb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cyuzpvzm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhpnedug.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3clgvshpo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tlgatlrh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wgxujxan.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fuggkqrd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifcocdzj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfrprlhh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngxancxm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lolesxnz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kiheuzau.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3exhodfnk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bldycjqn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gyecoeia.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3oyllgeza.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3woatkzdy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fnthzjkn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fzyzyddy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ibamoyqo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zuxwxyxp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bfwizzbt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vsypsklh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vejajbhx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qlkoowwd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ibadalvk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yiathgst.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3czzkpiuz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3dpavimmr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zkmfphxf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ybhtfxsh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ssaantia.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tvjmojmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jujcmmcx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3uwkgxlcr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fgzldieb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zxgowooy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rpvnxgwr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3janwziwx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3emhdqiwy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3chesejaw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yiitwgxj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gijmwmxn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3snmwkiem.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwgyzcg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nowqobuf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3loyaltwt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axgoqxym.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vsfnydja.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3tflkrtes.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ixdleyow.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3evamiftx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzuqemvp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3simibfeu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dskhxipp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tmspilyr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zbxmivdz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qyfcctdm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3imshiwtc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oyxzalog.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vunogvxj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dffuyfzi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kzeotuhk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rjgghady.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zhlkvjzj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3nsidxnxj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zftbbviu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fujillmz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iifywplt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vgkhtsmw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xssebeyg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jqkeubxg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3etizxhrv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tfgoqhcr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jboeumhb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vqneykoo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lliuqtpp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipiyixpg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsgxymo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3djhgbjmp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ofluxtrx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3klplcxne.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3tqmmyhep.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3radbyyyt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wxzqwora.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3twcyfeum.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wbotoyba.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dircykze.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dbfuwxas.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oupijlif.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zqhvjyim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iadvvvfo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vmubzdqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yauiztry.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ttfirvbg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kvzepybe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wudbujld.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rohjdcbh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rkjuraud.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fmlvelus.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3roloutom.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dkharymf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tsaipnjf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3erwmmdud.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dxwuslsd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ghmgtvlk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cnrhiabc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nqxosgsh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sipmflfa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cmpfnemk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qqwzilra.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qfzbbxcy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hwkkulfl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qrgefrsi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fggajwnw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mroltqdv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nkxcegls.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hlhohqis.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnozfxh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3sijginsc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3izxutqfr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xikvzwkr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wnecmqfa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vmgksohs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3snoyfbtd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeodwwlo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tygnebgw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxuvywy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tizrhpsg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwlollh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bwdwejyl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nhhmvifb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wxllocmz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsyxglhw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jbftvcqn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3shrkbvke.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iikbatjc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vydatxek.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3obkpzikt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ilkuvbqx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ksutxwmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tnyfadyr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwdnlgsk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkgaxqzu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3brtqsdvq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gfawgkhl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ddzkuzow.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3szfqywvb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sawlwham.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kbhwcayn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3kjbxvpod.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aplbzpqh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkvzzyxj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fonewdth.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yelkwptr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jtytumqk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eclvagwi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3riyozezk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ibybkwer.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cpfzenon.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3byhsyvcz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bvqtfcew.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gqueknlq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yghjrdlt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qjbgapmq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3klfhsidp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3urxlqnwy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3adyqdmmu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxasto.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tehawypc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqbuulzf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nicrwywu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3omihpdyz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ngspwewv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3znyketon.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tbfqtkuv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lyqonykj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wogdgrdn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3stuxdflp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eakrjdib.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yysvfbxv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqawgiyw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hknwolcx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yjkloppk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lwtujkft.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3auvceoaj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hbccnuui.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3leyngiye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uebeaycr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhvhkbzc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ttpfumfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dnlwdees.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ysluqcgr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tahmrfra.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hmgiqcrl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tiiidruq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrgaenwy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mqlsonxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbqirnt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hvuqpykz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3izwzjdmm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ikprlfza.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3dszzfpwc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rnsssdee.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3oytidzaf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfprrfrr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjknrkfd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3btnzpvwd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qwqiunut.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hgnqpipd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lqqvxmmj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3quibotjv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yjdkohaj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tncbzrhk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jtvzzejm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pwyvzrcp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ccryfjtj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tpncfvkx.html


<!-- 参考信息 -->