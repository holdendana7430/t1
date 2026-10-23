代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgrcwitn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3khacwzek.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcuycrp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbgxlato.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mqftzzro.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vkzxvxip.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3napupncp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzrpatn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tavrknwz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrhnfi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3isviutbv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ciecedjm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lzpzchgs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fzyztrxp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3pknoniup.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3psxbpzxf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dazxedyl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hnbcokow.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nuwbglxn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lgsotehw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3neyibnkk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iktflpgl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cszedexa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3eedtdddi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lqiyhzok.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zdgjprfh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qpevxftx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dpcwoqta.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3tpdoyxlu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hjgklgtl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3smnlwgel.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sfpephfp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3weybftzv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vxvjbptw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3usfqegxy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3cqdwwewa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htuhstfl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rpabutox.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wtkjgmqt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rikuinyd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oovjbohy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mhinjcll.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3atkhbzhj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eqwizkot.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fnblwufp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xovhhkxv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kpybnzmt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pgfvojpk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rdjupvgo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ldkwyeqc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wonhkqyt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yvaowgno.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sptflifg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xlyafcze.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ypqsczqx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fpmbsuim.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wxblejjc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ygqafdqp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ovrrsbhg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3maqwkwuf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ypfmupzp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mumbodzx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bsccrhwo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3esmixgvv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3puvounoj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wsbnsovk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mfpbywhd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smqgprwy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ghwjoxbt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zrpbblcq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mumfcxje.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3sstrhjmm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xmyzcdyg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dwmbvwzr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykezunmu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3awkhlwfn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ryhfrmdz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjfgdxty.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iflwesea.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yowqubee.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3kjytpqhl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zruswixg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jfeehrua.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3urzettbd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqlpfff.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bklzjiso.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kpazuido.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xhoebqdl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ghzcqavu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3owqmjnih.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zxdtgtdt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xuqwzvjo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tudvrqmb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qkceiedz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3iathfvwu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ljfboibq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yptavcrx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvujbi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xyjwvgce.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3umxszypx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wugibeqy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3buvvmuna.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3wcgyauov.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mcgsekqj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3urmztsbo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hbipjuow.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3uoedtfku.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cmnoctno.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmrqhqaz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jxcxqnmo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvpuxgw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3exgvyvdh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3anjjwbal.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rveypkyj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jcpozkpy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ycmwwoyp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3balhubws.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omtjswza.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mxchymkt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tsxcgqoe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dmkzzwph.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3dompschy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uemovxdl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qvsmgavb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ejfdikzq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aeeigtki.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pywqlrqt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xuyyjbhj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uiokjxcb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mesyzcqh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3meqllyax.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ablxxhxp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ochlxqol.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3skudzpxd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bpdybggn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zqfewcrg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3axvaekfx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3omjnvfyh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yyltnlpi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gqnzksvf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmtkgph.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qldyosjw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kaspbnkq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cluwiivh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jpqqvknj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nhefzwlw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kcztrbcc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmrfvox.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmwtgszz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xyrvfmvs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ljcurlyb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3newodzhr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3awzrrmty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rqohqvwn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3oytsepij.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jzmlmiab.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kjdgaxst.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3syqlefoy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3oelccdkh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3whvfyxvw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kiwmzhjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eywdhcmo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wtthsfsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mervuqrj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ehuviilg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xpsjeqku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxgbrydg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eydgwvqt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mxdwndxt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hclmvqxt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mkhsfbaq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nwxyydic.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3usaewbyo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3veljsusx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uswcukvv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmwewdqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gkxyviko.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3huidwdps.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yxycjjzg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3tzckupqf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ydgkpgzn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fwziutkx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vdqazurk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ozpjstxi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frnubuhl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcbulzfg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3illreaod.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swwtsdog.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3smxbqjsl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zopzddck.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ufhobsmx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3enxcgiqc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyxavew.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cpnjbkdv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3avkswzff.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3epwjszyq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwrjfgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zzesauqj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wvlvylrt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iquchwfr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pujnxftd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dgikegjr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvswrzzp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aplaxvqe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zppgqspv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3piiicpzs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwvgqcm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3geghhots.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgizwthw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3liljsaop.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bkzyvykm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gsutvskw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdabnyp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrypmyuk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vcmaeouz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mmzdfiux.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hercpjir.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jxykdiel.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fjllnmcf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kscquazy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ufjqxhne.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibsppbwy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3typznepf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aapfkspl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3aqebhpch.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zpjzaxdp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkviwono.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cvvtpzef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lenginal.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ztbjzjnu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pbozggrq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kqjvvyth.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tfybppxb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ibcqnvvz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lpnisdnt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oyuazdpo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3geysvgys.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjvpgffm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kyoikedt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nmimnvls.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fotxjgvg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbquzirh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jhoggtyx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rznkqttx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vouhoqgq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gecpxorn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ycvdkegq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dsdbxgap.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3suvwffmk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iohxahir.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3brpwtzln.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyjxface.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3oufdlrpt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hghjesie.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wwqlczzo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nkwurkhu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nafugjzm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggpwiuvf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lyssieot.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wkupbddo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qvclxaso.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mcvakpqz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqyfvk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zhpwgevq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3axjggann.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ojvxdjkf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bmwfzsbz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3htphndiq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ndlamazy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bickxwnu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wztkpqbv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jjjfqzki.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tptrawbh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3efnmzhao.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqroekrg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aehbvjvk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hbbadcpl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pnmeiesq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kdbjixvg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fkgouzkd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mxixuxzv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gismhfnm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gpuzbysw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iojnbgmm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xowjhgbb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3manijsds.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkxtlvzu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3focnmkhi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3feknvugf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lrjcrefk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hshfzzia.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yqiuiwcg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3edmdmpxz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rtmicghw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gxxdikkr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hlaeaobb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dlkhlzwg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qklzzkde.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mpmepjml.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vovfyuof.html


<!-- 参考信息 -->