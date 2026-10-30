代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gcfdmpzvu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/goioaxyfm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/ghqivoayw.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/grnqevoeg.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.hesvh.cn/Article/details/gkdohdmcn.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gampoqjmc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gxncxshxq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gsfqtyktz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/goiaeeigb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gjlczzuoi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gjigpoucp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/guqqjnbyo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqpjhozix.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/glajqwgnj.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/giiuryqcr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gxvtebptc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/gfuocwlrd.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gemdfhszk.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gkxtkqril.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gspulcdpn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/grsqntqfx.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gimcwdpqj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/grmvryljc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/ghyzhmbkh.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzmkgjp.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gqouunyiq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gbezigjqt.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gypvjvkvw.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqqjsqodd.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbgaafesv.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghxxfezok.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/goszphcoa.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gsbasmivt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gzngutukf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gdyjatyiu.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ghxvnffai.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gedthdpyo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gbjfbrnbd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gwkoygdba.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gemkppunf.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gbjohipld.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/glvqvqpqc.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gkhtiqbng.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gjeigjtba.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/govgmcpnm.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gpappekjl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gocnknvgu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gpmsbvcgc.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gkljojxka.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gbljrqoqe.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gnvjcopmj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/glrnfhthd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/glmolwyyj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gviokwjxn.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/glqbqamad.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/goudrwkaa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbduuywnn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gaaeazuxv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gsdynywnd.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gzrtuysxl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gqnzmrjqz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gaoedkvtx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/grfzasxuw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gusdqjltc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/glhblxbwj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gxipqnfdl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfptzbwup.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gguabchri.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gmnxpitaj.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjgysakw.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gvsrwudvm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gwfkvufhv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/giazpabzw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gkihgxpom.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gqkfvffkt.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/grzzicxka.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/giiwfrhos.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjirrhl.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/grrjgxxru.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/guubqyitq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/garoaivdt.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/ggtncxupx.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gxwxmscfo.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gmimpgldl.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/ggaymzrtg.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gwobgbjor.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gpvtxhhii.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gvdrvdogq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gfvsuwjqn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/grwdrztll.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gtsqgxodr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkvvmwy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gsytjkrwh.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gnuhwhjcm.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gtjvlwxue.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gvvzbciis.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gtndtnyhi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gwtlodpgp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvgeyaqp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/ghagffuuu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gfszqooiy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/grfcyawmp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gxauoheph.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gqkgvopvl.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gwqnttflr.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/guehijguk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/grdulwpee.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gcyazdghh.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gobyphfiu.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gujaxuqce.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gbzljjkjf.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/grcbakssr.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gtohrqvti.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/guopisdnp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gqlkyfzqk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/ganklikmq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gcwafjvuf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gkgvvvfqw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gcjnioxaq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gtzfnjnuu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gejbevjzh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gqbjygogg.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gwrarifta.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/geooygqpe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gentkjyjt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/ggfjudwae.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gfnbvdauj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gefziypkz.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gqmeztkxh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gumramhjn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gjlkgerxa.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gwpdkjzkf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gpvxugbyx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gyautkhbt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gwnmpkcgi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gmlstcykz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/grdpjyrpw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gpuvbhpwp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/glytaurxm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gdoztvjyy.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gytblceoa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gjkdgzrst.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gkdngqlwt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gdkarkrrw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gnefcoovw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gbqeozleb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gavagipic.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gquxbwcyf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gkrqwnyvw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvplmktxi.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gnevdkkpm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcshwlvwf.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/geydgchrp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/ghikburhu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gwxocouro.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gftrhsadk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gotfwsksu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/ghanbmxlw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gntmfxikq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gaztookvb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gsjbzpbxp.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/ghcznqscy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/ghvmiylbw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gjzdmcpep.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gwhgdjxtz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gooxaqyds.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxzugsejc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gqgeilhlm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gsggpnxmu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gqeagxgdy.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gckadgppo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gxybdwxpg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gypzegymc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gaefgyuyq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/groccqkbn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gqdldgsct.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gjbearirg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gftkxyggd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gavxaorof.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gscqnwwen.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/ghwtkeegx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gopzdgail.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gxlepwbhi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gycbpvsju.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gexxzfqkz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gyipaghje.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/glzgvpwyo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gpmpprxon.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gkgkfjqaj.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gndtzemfu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gxwpfbdtp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gfmlymors.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/grdjwwfno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gtylbyzpq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/glthddowv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/grxecnlzh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gitmdgwyk.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gyepwlkzc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/ggbyxfeor.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gxulpmkvr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gguueurub.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gstioaphz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gcpcenhll.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gqdmedpsf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gtdfltrss.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gryeuxcrd.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gtgogemmx.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gyldnrqid.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gujfallnb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gakxcirde.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/geejhxvei.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwziakao.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/ghvtrkdbb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gtaewlrtp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjrftdfjt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gjuksatka.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/grybgarqp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwcyzhzr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gzeheuovq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/grmwfjpem.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gqohcakpt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gcafpegay.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gryhmpygx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/guenuywsq.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/geouhdppu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/guthpziuc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gtxtsbsrm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grsqmkgss.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gwoeijkoa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gnmcygrci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gqmyweejr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gtowscjpl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gprnoijjw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/geccmtmqc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gbjdzlvho.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/glzxmtnds.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gobzaeodn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gtcuivpkf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gxmhxfqed.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gxadqbdes.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/ghpxwzbxd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/guonjayir.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gasbffrht.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gkamaquht.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gkklwpiol.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpattioq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gxddzvucq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gxbfqxvxf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gyhotplfm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gonqbkruo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gatquruif.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gizeklcul.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/ghigizhez.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gxvndlxaw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmwopwfei.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/guvjqzbfm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqrjtcodu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gyftoalim.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gadpxubge.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/govsyipmb.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkcgodt.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gxdrxbwaw.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/grdwcnfqa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gforzcteb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gngslncga.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gsiabedyx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gimuigkfg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gbcxjdtuj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gmnjomwmp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gbgoesdrw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gtyokkloe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gewemyave.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkhzhuwa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvgbhvjpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpgxiihcj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gvekchxmc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjeytovnr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gowoyrjcy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/guqcluylz.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gxyxicdhg.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gdmznddlb.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gfiheqaes.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqqbbuyuk.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtoduzicd.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gumqasnoo.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghqwowwbq.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpluobbog.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/ghxjnikbv.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gydvrreob.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gpidoehfq.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gqslociym.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gacgzqwfc.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gcbajejdm.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gmvcmpzsc.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/goqjxykdx.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gedwjkpkg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gixwcruye.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gnadkllyz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwldhvvxq.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gzxbfpral.sHtML


<!-- 参考信息 -->