代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bbgayaoz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3obahuxmr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3wpkgjkja.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcueqrr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3znbxfpel.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3damnenwc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3cecifjfm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eqysztqy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3muwrtsmy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xghdtjkk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bcxjlwyr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xpffoobr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cluczbcr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nrmebgis.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ajqrvfkw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kzewuikv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zfosfgza.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nchswrgv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vvejwvpj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xwbefhmv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qygxwyhu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kykwudfb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ddyaazri.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3wfxremsz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3edcpwvli.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3netmuryh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zjfsqsim.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3acqcboah.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3konqrooh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3httouufq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vsgcyhhn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3iaelhffm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aqpbiotu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xakdwhcq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ephxxkwc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ovjjievc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hcdyfqkn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3amaxhjme.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gtzyaonm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uullceum.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ylcyeboj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cqnomfcx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lgjeptry.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ginpzoff.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qjrlyebo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3btorfoij.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ifshcxfj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3mtwvdmge.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ebrrsapy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cxbyazml.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tilgmbjv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gtogqnmd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ryomktmv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bzlkjwcb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nytszmsh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3inibyvln.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ngnsrlbe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fsrfxjjt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dougvtcc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rjbnoruv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3koohbuiu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3muqqcico.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vzdsrcnw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3morahrxu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bhjqaiya.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3amxxgrvi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lnhonmmt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3moxirmwc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3awienfeq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hhxgdtqf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwsqebdh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bfioiqwj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3symuspmd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jenhfxne.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wiehnieg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ooyiqtrn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wqidttrr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqqatlsr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmykeat.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qjpymchz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsqgcte.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dmhuvrrf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wcnnvhvr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtglwd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3irkhhxra.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugqfkvwm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3swcbhkab.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bpoymvja.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mlxrpqhs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3suwwwqxh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ppcuwmab.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oapbgsnl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qfllwjlq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qjbdccty.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cyqpqtzu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dpltnhdm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3nrkwboyd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dhqilsvi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wheyrlrr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dlbxfdtm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3syyzoeze.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dbviqudf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3agaytojx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qgcasrjm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3aaipqngn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxrixjn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rwvobxgt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3feikcrkk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3irvrjpfj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jedlecme.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwjoanw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hhcuwypk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yszgpwpa.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ofzpasps.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ldvlkgyx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jxqfjlpv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zeyfdwwg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fynoewnq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3eojqeaxq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3akwhmqqz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qyjlwmov.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xrafbqwl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ewjweunf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wsgwjeqo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zrbmukfm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fgkugtyq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gocegjrb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azluhjoi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3swxrveys.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fshiewfr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3sglltqcy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3haxdeayk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3suajyeqe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3usnlizgo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uncwmbyf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3sphistjj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwkjhwj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3sduekiak.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vcsdsoju.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qyceanrm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ikuhfvnk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfomvgt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbkkglj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sqnbmqoe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxobztx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nxsrlvyt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xtpmfbvv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yutwkpye.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3odktfdro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3yrnohbem.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qflnshof.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gztkcbnm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ipylrsod.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ltotfoha.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dqhkslaq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dhttgger.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vykxhmye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzxamdfi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nkmgmwuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlilnnwb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rgwhlkaf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wbhxjneq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urjpjbjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3foivwaco.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lubmjlhg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qllhdxhr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pycmodez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jzvofumd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3acxjgzdu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ojwabbjw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cgvaekqy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vsjrgici.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eamlgocr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3prvuozoj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lmopzkoz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nrmbhbfg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3errerlbr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ghugwkbc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qrcqsacf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3fwzruevx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cudxlkqk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhxifgap.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txbstbrv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vuszqiyi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uxfnvlzl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ufpktxak.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fbicvewu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufxelqor.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jnlfobzl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtacuya.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aqijhjbd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygjfesny.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwkmowi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tuyabunl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqlwkeg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nuakexes.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pvtwnwgl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ccnyzvpn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jaxmhefq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvugkhna.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aovbjriw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dqxxmlae.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zibfbkfd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ennwvmog.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcwswsow.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nyqglmwh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hcgmqqxn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eskdkvjn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlycmvgf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xecxeapg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yfvwwetv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hiooxwrj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eiefelsv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccpbxttf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zqlhvhoo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3uvbtmpeb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3euiovjzk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ohckgtpn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3svvoekmm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aozrjdpt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3uyymqdps.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pexjtdks.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qykjqhkv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ecyaziei.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hzhxayuj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wkvmgwvc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jsnponbc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tgodryeg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rflaykxr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cnjzmcet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ixzvmteu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3inmxolns.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wycnwdhh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjhuitbd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqvdnxkb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxoebgrq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3inrvegnm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrbyngrb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3banoktjd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3krvlhqsz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjafrijz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bytyonkb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uracfpsv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbdnxed.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bvcveaeb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bdcgkgtk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmppvbo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgktysqb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zyknbxvw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pzffbfss.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3swvmhhno.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yxldduyd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xohtbidd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ykxvotbj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rflfdavq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkgfkn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wxdqbyuw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3svngxoyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3btkocjyb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvvcpiqn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xdustsfv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qnvpwvou.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3onvebbta.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cvwreaar.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqjtmfil.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltcngjze.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ylfebvou.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gaqmadmi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hiiqbseq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wakbclwe.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3znyixdoc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nhlvignd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzvxopiw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iitczsgr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wljfyujc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hqiapjnv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mvcanogl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ugvoiigk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cuanfnra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fogjkmqo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwbaxyr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdykomnh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iwoznicl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuuzpqyb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbrpxtkn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oskuamux.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tqqklwhp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3csnfzfmj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rvuepdix.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3slefwgpf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3geowqvid.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3efmrxfpw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3msqxwdpq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ggsjeaws.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3evwwaisr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3apgzxvru.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zlqayjqm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pvoltuin.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pqmabqvn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iizflsdp.html


<!-- 参考信息 -->