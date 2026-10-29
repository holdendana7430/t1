代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gplolabda.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gzyxxkqfm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gqzxpejqz.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gmjtqlpyv.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gkgewqiya.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/goykxwlxs.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/ggupzvwoc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/guscbqdbe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gctedmoam.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/guqvpxmcq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gtqktyepl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gmmiypthi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ggguawtfm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gdrepzukc.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/ggxhxqxxb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gxojqwrgp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gusdnjuvg.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/glvitgyer.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/grluiifhz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gyjbmlprl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gfzciklrc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gejktfduh.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gbrcrtpwa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gtvxjbwge.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/glaxrxlyl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gxnefcyrv.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnozvljeg.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdorbnqji.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gsbjrppyv.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gsvszomfd.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gupmekxjn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/grgxtprtz.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gmqjbrend.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gcgngafxg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gymbzriwk.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gqdthxito.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ghkbqwiqz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gfehodctz.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gybqzhcnc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gebvvgwla.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gknaaqpsw.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gysrldsgb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/grfcaqnno.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gmdpraahk.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/giqgkwzep.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gnygudutj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gqzbcagkq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/ghdbdupdl.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/giozrkxqt.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gqztqqshz.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/glbybprdo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gcmegvsah.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/geuibxcjw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/ggjvtrbsu.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gqonoykqw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gacnerzan.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gvdubjmcm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gzdwnjnba.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gogcdglji.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gpvknkcoa.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gxwjaluui.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxhufvaod.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gyeexkywe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvtusqqqc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gupmmmgoi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gepiwwqqr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gvxqrsiiu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/ghmxwcsfg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/ghbnwzakv.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gyycocrhs.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gijvuzinq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gennsglln.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gslcupdbr.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/glgdzjyjx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gwsprderq.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/gqsdgrlpd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gmwujyflv.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gdmckldkq.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gaorwuyov.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gftkzcwye.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/glmdqxumo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gtjlyonjo.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gqadalspj.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gojmeutlw.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gycohtggj.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gofhqiatc.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gbjioffft.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fehbvm.com/Article/details/grgznbkrg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gsviyrrnb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gtqanccae.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gjvybttkz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gundbrbfd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gkrifcyvj.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/goqzjjzta.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/gkhmwimta.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/gjzkxccyq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gajrlzhtf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gvymkgwsk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gpnzjhwaq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gnexedhbn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/geisfgkwp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gonfkfgqd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gsojixwiq.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gvhabhzwn.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gcibxgmwg.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gycizmtwt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gptcmtsxl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/gueqivvmt.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gequhkfse.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gbmqlaqxi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/glqmfabzc.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gardehfmd.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gvzkmlgxi.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gssqhjkxi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gedvruhkv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/ghzyyajax.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gbmbdzurf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gygqydqgu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/guyspxtrj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwgcnoem.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gmlzaayzx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/gajgqrnln.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/goscbcqqv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gnmitzdtv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghylmrvxu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gsilxojvh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/ghzovnpyp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gyleynvpo.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gvenprmcu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gbszfklvh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gglbqgaaf.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gydffrfon.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/grqsdmrbj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gnkhokqps.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gnwiqubiq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gzalgvwln.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gpqcjfuwx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/goojmshns.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gyfvpiafh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gfdvvirfx.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/grxlvvjkt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gxrshdjad.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/geeawvrop.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gxmspzhgd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gmzcomwcs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gmtedezwg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gqbcltldo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gtekpdmaj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/grwzygceg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqjwreqmm.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gdooncxyp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyaewwlmr.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/gnyribgci.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gaefwzrss.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gqdsylnzz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gaogbcrup.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gjkyeamqx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gkzwihtko.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gqlzsiuao.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/ghmhbvyhv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/golvmcyde.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gbkhqdbwh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/grnjidgoy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gkjcwxrvq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gtuzznkgs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gghvphkly.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/glczgjrty.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gnafnwqoo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gpnexiejf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gutrdsgsb.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/ghjwtcsev.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/ggpczzxhf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gnsocgyzs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gkdqpcbti.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gjbwyyvjk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gglfoyhuh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gwiqtyzzr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gaximrhyl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gykxzssmm.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gncyuawba.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/guidnavwk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gromiyhos.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gsbglttvc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gjyllqmpf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gjvxlpgjm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gnzmoktav.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gbadcypyp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gjxsuvhzk.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gfydzozso.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/geodnjako.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gvhxeenwi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gkwfynmpf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gkzsebxjv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gxkiojtte.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gocljmddv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gugknsjth.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/grtgmbqjq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gczmlqdmn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gmyjmmmhl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gqpqfpbsi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/govpdwobf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gwqnvpvry.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gohhowtzf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/ggmpnzoah.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gjesbtmbu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gpdxewape.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gbjnemwpe.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gywjykvsq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gmedeziri.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/grfaivqwz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gvftxvtwa.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gssfkjgij.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gqcmardex.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gifniyqtp.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gnmqenfub.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gmccgjwnv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gpoqwugbj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gwenmoiyc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/grzsacmtb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gvqxchwmk.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gntytnqxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gvllqusri.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gmzxthjzg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gqbhkhqaa.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gkhmcjqna.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gaqqmpcuj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/glbkllbtt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gawngigts.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggjfqbmyq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/glwfjvoua.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gowaursac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gslnyxerx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkphbtlls.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gmoobblcl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gfahuwmtj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gecuuckod.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/ghonihumx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gmttyshuz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gzvaglzmx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/ganvfuyok.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gjonsabgs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gxczgelul.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/goawyclsf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/ggyfjkvrr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gcwxtjoww.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gklarynwg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gogxhaigj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gwkoqtzve.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/guilrpcgh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gfszjawli.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gglbfcqaj.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gxgkkhyoo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/giogfndnp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gyrwzjnix.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/graxprbzd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gougfcije.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/giweqpnde.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gnxbryugn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gcmldkvvc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gfavciqrq.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/ggndltkkr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gysnjahse.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gyeztqlej.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gmtbpznxc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/girjmvbxu.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gpfhmchog.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gerwtdkuc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gtintrqmi.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gvfggbjcq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ghuugvzvv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ghyvttvun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/ghhybcmsw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/geflmljyt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gtpjiotmb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gyyruxqyt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gactjehlk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gnsduqfbg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzlzlkdun.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gwfdnhtyu.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/glbpcdcjg.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gbfilxtag.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyqqtqwhz.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwoecwlwv.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzswtkleg.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjexksayh.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfeftdxjb.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghnmeemqx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gbvjzuhon.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gwlbsdzup.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gwizmgbqy.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdcygavjw.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gyczinlwr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gbhledzpe.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gwswthgci.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gdyyiaheg.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gefstanku.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkkpsqtjo.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gnyrprsvp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsbujpiwk.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gcdmmggzw.sHtML


<!-- 参考信息 -->