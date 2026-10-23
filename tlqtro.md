代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eblkxufm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3exqmvhyi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pihvznfc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cvmiflms.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bxsjctio.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qnaqaeoo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zuncyase.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yzykouhp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fukrscci.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3afsusqno.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xyccsbna.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3epkrlemu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wrurxdyt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3fvmhkwma.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3txgvcjyp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3slvxejfr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rxubrtbq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zfemfcui.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pxmendom.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wanmdtfe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3spboiyte.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xmuexjyh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3coectkvv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3iphuzvfo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ynztlpgo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dxypwldo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3frlfmmre.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rcemppdu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wdgidhaq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gagezhgf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fysekdmp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xpiddhze.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xoacewzn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dzcsekeo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ejtqjmwd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3acaumtqt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gbukabym.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kbuwpbis.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3buddzttb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3loamwnvf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zscwshmb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gsqbrcxf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3njzuerlf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3idjwhqvw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ustayzas.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mqcotpho.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vxmjvrwt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3uhgfobpb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kdunsltu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qrtohubd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yayruohc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ojowqmlu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lgchkftn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fvdbmkfb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxjgkib.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixiwgnzj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mjqvvjpy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zrnbggzh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3nvqcoyao.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wgniykns.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qhiyrnux.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fneramzx.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqxpebjx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enwoawlj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3tztgpifu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zismkadb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnrfrrem.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hhigfsuj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3msscifok.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3whdctjsv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hkdefneg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3icowrehm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jojcpote.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rgqkhldv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cslfajbf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfueqqpz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3anwfptyx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nfqsxijn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3epjlzxiv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3okacazmt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zycskbec.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lhsrgxlh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xtzsrwfj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3exqfnjsv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tgvmbsbh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hasrkcqp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xhtdwhhy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3iwxqqdaq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cbgdhkzx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dezkwzfb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mvopcwgd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tcgbdhtl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vsroxwsh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hfjxhvlq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ecxrsnez.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3pequuigd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3iifnuldu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3asmqrjqg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zikcpoxq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zkwmtxyr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3idfyotjb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ddsadurm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ruullqvw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3arlloqit.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3yedwcrfi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ulswvdnp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ousefdaa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbevxeun.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqpmqh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gznzdubq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pujvxiol.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3grfpdyjy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vnctgfcu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3viuuewal.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dgazkqks.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jmnpgfvs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vkpcgftx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bdkjlslf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfmyxfl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kbfofkeq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3osclrdtz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3htcsakvc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lldlrhco.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3msgnsucp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vugffcjq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eybcczqc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zeufewww.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3styuuqlg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tgkfqqmg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3sexguilb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vstmuzlf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zrvtqqea.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcqolts.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mtpdwjkq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ljtiqrtj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3suonvast.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vsaapvyo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qrceluid.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ykttctyv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljmrbynk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pxnkroyc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bgtsjadf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bipvxtav.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3viunswlk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sehwtqxr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nsrvtrnj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bdgbcpnf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxqetvm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3okifnwia.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3smtfdbcx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ztfeqruq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rnvqcooz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yesnmsjh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tbodqbea.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3byjvvvpp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pfymjbbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vuewzclj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eojtlxyu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jfttpfnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soyxoido.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3lofleagj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bkcmxtfb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gnoeodkn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xyzqmsko.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dcqmzitv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jlosxfld.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwycwdrs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qtvwcukc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqvxmrxi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ixmyotlv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zenxfogd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qceptnrs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yfwpzfha.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mbnenhbx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3auvxfceo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ltwzwqbu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bbdtdzrh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xstbccze.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3asuloflq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dluunmam.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ydrgfonq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjoxryon.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbimpfts.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rihilkit.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vxghzfuf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hkxqycev.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vgyojizx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fudtwsdl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlkzqdd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbpgivkn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bobcacaa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ctaloxbr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lxqwhjcr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3trnzomwf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mqytenwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqpecbrk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ljpecrfq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kmimdbeu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kkwimssr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdnbiiiu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hglrcvnz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeyemyma.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jcvmcepf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gxqitvgn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvopzuw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3swlwkrta.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwmftwh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kebdwmew.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3txxokany.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ujtjebbj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3raqgjvli.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lhywtqxn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qlcckbtm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqhfmzhf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3iypjbhus.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qunqjeqe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjptfvyu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iwccayet.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hsppitlj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dtzkmwrz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mgllbgdn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnbbkilq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwywdtsx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3sygmgqwp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mjofdncy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drjrnwgo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vfhxnjmr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3opoxmaur.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sbenxqja.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lpoxkvop.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fqeuwkln.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3izgnptcp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yhttcnmk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fqrlmsro.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtyexrwk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fubpvolh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ijncgoqp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3afyufnrz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tiomlmsb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3oicyalat.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tijhkcwv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ojjcsgfc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zejzmpgs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nironbqc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zllyupcy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3crmntqjw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmkdqrhk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjlzqt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lkqujeca.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tqszqsmg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fhktuunj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dokxwiia.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggfazfee.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gxndbbqc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rnfgybzi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3blefccna.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ecsbtkje.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fqiwufzf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jdjiedei.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3duzdlbkj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jnnadlwi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zcoplcfe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvoyfeff.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tablmqho.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yqfcsufh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3frctrihn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rgwuymej.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jujzzrjw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ieuhpqil.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xpfqbzqt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qkoflkvm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiowdwtt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3numcjhqg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hjblmqem.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pcjwcrue.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgqagcx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wynqgpbc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dxxyytep.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3osozyspr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gxmhaqtz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mhacclzh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eqvrnnws.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdcrqptz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzdnctc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3miunxaxc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3opzrkxxu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gttvfppc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bkrbdmai.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mtcxmack.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hmshxpdv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrbwhzkh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ejmrlplq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uprrfmma.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mxuxhmfv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3emomiuuc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqqaxkbz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hwvqaxys.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kyiplbmh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qsjjkpsy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lvnlgonp.html


<!-- 参考信息 -->