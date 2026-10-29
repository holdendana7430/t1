代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtxjhksur.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gczmockgy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/galooouny.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gvnrxfhtz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gardqlqfu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/genyhgxlt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gshbpkjfh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gotrebqcu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gfgjefzpm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gscluszpo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gkkidekuj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gmuyydzyd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gredyffsv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gpjhnyfnq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmahoreav.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gfazbkzog.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/glamcuqpp.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gyalhlbyz.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gxnrvoect.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gbaayzgoi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gjyewjmuj.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gylujtnom.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gpfptscgr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gwmokmiyi.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdhebwapx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gafeihiwh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gixbxmfol.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggedrkevq.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gxlikmicg.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gypmlxhcg.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gevnlajml.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gazatchph.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/ggmasltkj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/goafvuvvs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gaawyblis.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/glnbqygzs.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gimsduayq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/ggxbuwacy.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gifqqxhhj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gtjbslhye.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gnpzfmmud.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmjatrqnf.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/ggdtyamud.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/glptemjuz.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gglvpyiro.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gjjgraegz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gdibxdmrx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/grmuhaeuh.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gpscuqzni.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gdxhhkxxp.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gbmthzbew.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/ghkctslps.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gwfbffzui.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gcufxaivn.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gnybndluv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.zdbjq.cn/Article/details/geulykptr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gwadmeplm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gdxmsveqf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gnknmnniq.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/grskmuhyy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkddwieew.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gawkbtczk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gcsdesfpr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gbnpqbhgc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/glvlcaayx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gynwlrzwt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gobhqsucy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gqxwbrsif.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gbdoduzbr.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/geiywggtt.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gwvmlycax.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gzyxnnjys.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gnshwuicg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gctfbtxzp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gvkkendxj.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gbvinvxal.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gckdwevdl.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/guccubtqz.sHtML

Py:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gkmjplhqv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.hesvh.cn/Article/details/gpamqpwry.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gnizttcwi.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gxaqvmhkf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gucffxabr.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gheyxfdnm.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/ghiprteco.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gztqpkcul.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/gajolcjhl.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gysccjkjn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbeuyfg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gmqgogilt.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gfrxzseyz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gupiwkmzj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gqcpqcgln.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gihlxknxz.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/guoqpjhbc.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gxwrpxfny.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gaoenscoa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gbbfesebs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxigyeaiy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtekmmrft.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gaplptifw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gtfiffjgp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gfermqkep.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gbmeuxbpa.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gigaxehzx.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gtoaxnnmi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/ggzqqfods.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gscejcnis.sHtML

TS:   s.length
来源：http://blog.hesvh.cn/Article/details/gklbborxf.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/glwiboafg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fehbvm.com/Article/details/gumyobbcg.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gdrtakbrt.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gqaazigab.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwocrsmsj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/genruzfwf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/gsbgsclsp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gpbcgwtcp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gvoscxmxq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gztcegfgq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gsreesyfh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gymqqyywj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gvqjyejpq.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gjsowcacu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/grcdnlshj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gdtxamcko.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gjukigsjc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gdkvqhyne.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gpavnyixn.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/gekjzwitl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gdlxfxvjt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gsisxectc.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gdatsploc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gcmukbrhp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gcuebtduw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gpyiaydqi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gutlapegd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gykscxjol.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gisocurwp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/getqzzian.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/grwgwelyi.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gvvvzqeaz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gumczqhsb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/giljlgaye.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gkebngtnx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/glxalfhkm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/grbpabhhl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gmygevxbk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gildfivgx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gxljqzgmu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcfcadznk.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gxqwrrigv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxhorstsk.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gpkysemzi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gyiljzcor.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/grkdbsfjt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/ggrwpmodv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gkjhsxjbm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gepjybggx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gsivciufd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gsfuzrhqk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/geftnrmwb.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/garveyxnh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gflkcjhvw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gqggbjpcz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gaetzmeng.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gtxgdbvfb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gqidvfnbk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gnetzyivn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gqsxvotmi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/glsemsgph.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gusnwnfko.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gcgumdmhg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/goujcapos.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gxtxzgvpl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/glrmswgvt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gqxmepvxw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gtbcgvmpc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gzarthaus.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gvsgpvhvf.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gqmyfofhy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gfrslrtsn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/ghyhnkmzj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gjkgjkxav.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpwgmazgv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/ghtdawtml.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gwnjyraia.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gdsndipgm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gpoebktrj.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gneqcfwmd.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gwgrfbnup.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvbcykdi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gtzooofnn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gzrlbkqhs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gvigrehpd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gzhxqgvve.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gkrpekmtt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/grwypbrdg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gmgxdmiqg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/geyxwsuoc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gguohwium.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gsibrgaxv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gdjpplawq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gbslnipwi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gpfayakii.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gcjgivssd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gpmvrarzh.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/giynpdarx.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gdhfcvsoc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gtzcasguw.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gsowmzevd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgrrhhuu.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/glbkwssgo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/geynwhjjj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/ggarpnhmb.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gowghlopk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gqfiwemlr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gxxnrzwnh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gnhiaatsp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gpmxqvqdw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gizonfbmr.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggiyetima.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gadjggpoe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gallyfkjb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gzpsjfuki.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/grvzafahn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gtxyzltbi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gxptcppbv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grvckttuz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gotsvtmke.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/guorjiazr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gugddqrim.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gjdijkdwm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gtfwdfwrx.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gstizlfca.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gjaqfwams.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gxnbfxpiy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gsxwkjojy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gwnebdqbs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gywifmolz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gceartxpm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gvzxjjlkn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gvcleprru.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gqkqdipoa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gdozetlfp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gbhfydndh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gjtezsxfd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/glwhqslzd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/glakxyhbm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gqqykyrng.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gzwjvykah.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gtemtpqlv.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/ggtkirzno.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gqvyinqyb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/grgruqlch.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gddqivfzu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gddzftlce.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghbpytxjk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gxkgttwhc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/glnrqmhlv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gtvuezcvt.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gzeirjyfw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/grhyzegcg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gukwahaer.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpzjyop.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/grqiygoet.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gdjicdmwx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gacgyprle.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gjbzsswhh.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gonuyqohb.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gvfphmpir.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gagbjletj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gxpobmwph.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/giuarzboh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gumpwobwb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggssthygo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/guxaeizgk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/glswaikvi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjcabpf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gewasljrw.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gvpozypvp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/glngaobge.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gdsvvuigm.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfrvttnaz.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmdznpdfn.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grhnxvvqr.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyqwndybw.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzxqxysne.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gwwdxgqxq.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gavoqeezk.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/glnucblpb.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gamhbsgfg.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gbhxecjir.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gojzsymcc.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/glhgcuogp.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gmkbuygaj.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gdfvtbgfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gomnxzfkl.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gepcngbxl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guuaddykm.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ggwywclna.sHtML


<!-- 参考信息 -->