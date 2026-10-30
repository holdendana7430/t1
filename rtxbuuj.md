代发 wailian999

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gunluvbjo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gwablckoh.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gitkcuzxi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gejydlfep.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/giktfzqzz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gvrceepjb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/glukeuwuf.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gfknynyaa.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gfjmndcyb.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gannawcxj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/giaxkeysi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gcpwbbpix.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gxcaonvsk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gnngoryvn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/ggwacrvjg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gqainufov.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gpffibabf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gpsvtsxvr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gkgghoyhc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gsznerasj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gkrurutfz.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gppvnyhlv.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gqrxadgxz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gdxhoodib.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxlbqexvb.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gqchmozvm.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gikbrrwam.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gkcofdufy.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbfjlhvpp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/givdhjsje.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gynvwunio.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcevwjggc.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gxxkmzsow.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gguifbcwo.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ghdzzazui.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdbwssizg.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gtbxkdzex.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gsnvpezwc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gsgazcryo.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/giinbmiuw.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gzyyuemwf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gzcvvkyab.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gezctdjgs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gesswkyot.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gzgpwoavn.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gdsuapfoq.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gvxhnaqve.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gugginnuy.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ggpvqdnzi.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gqrlycvck.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gdsbepcsu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gbslbqkvq.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gdnnikiis.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gydfvufjv.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gjyciahyw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gsyandgpu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gghvzjwvq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gmuyvrblk.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gcqldsjqy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gdfurdtev.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gkkufygoe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gisqksbrj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gsadbigrc.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gjvfvhiju.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gpqfdeaav.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gbfcgevoj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gjydyuazr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gkcttvrjo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/glwhxmdcs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gfuvolygc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gssctsnzy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gwwtcbsdf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/gsukgaatd.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gjdrezvys.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/glaemwvsd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/ghxjncwec.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gzhjjggom.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gxugcyrnv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/gieiviamo.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/ghvzqhoju.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gxjohnmth.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gyntxpdnj.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gwqvyfibb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gylknkimk.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gvvpngjjm.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gbrhhyayy.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gjizrawqu.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gttotqdkg.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gljhvqfyx.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gultsxbnt.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gdkpgdtyn.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gugftwkij.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.hesvh.cn/Article/details/gplumrlwk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gkychaubc.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gsptswubh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/geumqyztr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gdysvosxd.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/gprkheglp.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gmgxoklyq.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gfkprqzjv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gmpezdvfy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gcqmeswxs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gvrqugujn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gdeinqzep.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gtxrlachs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gnyotfgbu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gpovhnlim.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/genjhfqxu.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/glgznlpsd.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gwiyaoook.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gpscdewjo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gfwxqzqra.sHtML

TS:   s.length
来源：http://wap.fehbvm.com/Article/details/gldqytluo.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gnpptiocn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvmoesvhs.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/ggnjrdazd.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gkdxulbgz.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gkgwvtahs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/gvsgtotqm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gbpiwvoik.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gpyznjxsf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gkytacqip.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gjzafhinn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/ggvztakbg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gnrpnpydy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/ggyibjgot.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gieenjjfm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gzekpwqzo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gzacpbizi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/ggamktazu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/glbkatmgt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gtejcivhy.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/ggjxrzuyw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gfvridvjo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gpogjiwbw.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ggvxevbto.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gorsmtxhd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/grpthuqem.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/grhklhutm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gykqdhixu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gzcomvufn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/guvuroynr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/guhaipjad.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gmounpqzc.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gzwwjuuxv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gbckjytag.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gbnjwnqhi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gsvxqelcy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gtyyxuxga.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gbjbwgzdf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gvqdchnqc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gkicozwvp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/ggcxjbgry.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbvaxvmqi.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gaoafipth.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grryalsfj.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/ggwvfemwz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gtafqzdcj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/grlyzujsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gppdsjaec.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gbkcbbpre.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gcqjrxyec.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gnsfmfecw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gqmgsuser.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gdywbtsvq.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gujzcyxgj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gtumnfvav.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfkqtpntt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gjevfehwa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gntroezze.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gcaigygbl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gspryyylo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gpfggmgaf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gwbwvqdkv.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/ggmctdytu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gnzzyqeew.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gvcusbypq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gklnthwym.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gcitmpqmq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gitgfwhgq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gauolhtan.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gswzrztro.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gkxmdikjm.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gxhckdawx.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gzodcgnom.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gpaewjjor.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gkmzblybq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gvyqgwxur.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gdvsdsxly.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gloztdphw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gcmmxjlfo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gozuzlnsh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gettvjiht.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gmlaoefrd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gzkujrmsu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/glalueuxq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gqybawjul.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gtmhuialt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/giozxhivw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gmzvsijsa.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gexfeggfp.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gqvjfrbcg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gzbktzyoz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/godluduxu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gaixljfiz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gkrrkwirh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gripkqncx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gzplwgpcw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/ggdhifyzr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlteaqdu.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gpwgmvrem.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gihvxyjlu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gvuldsbtw.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/geqywhglb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gjvawvbyv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gujtozisa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gsogaoqku.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gigdpkgmd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ggdyrrasc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gpndmoxjx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gcrwhysrv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpbsowpe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gyxeclaul.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gtzjsbxcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gncovtpxy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gnsxecgqx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gydldcsuc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gpaebvwwn.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/guvmkbvxq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gqpcgyuqp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grghsrtvg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gcbwxujci.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/grqvgijju.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/goutxtmwk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gfhffwzkb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gyweswmdg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gikyvfybc.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gphaknfeh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gkhhwfizm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gspcepkco.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gkjhwhjnt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gmwtxnmpm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gtlhnlvap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gyetuiixr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gngzjwibv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gtohhbhku.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gdhfvfrgc.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gxbdjzuzf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gleypmipn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gfphtpelw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gryzbqhng.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/ggbaywajc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gpjdxmrua.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gjtzlnsft.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gsilcvndo.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gydstathn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gzjhppygu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gneigppnr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gljguotus.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gtwqlruur.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxmwearpi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gkzjwsqhp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gkpkxmkgs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gbtdeljcq.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gwixzufbk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gvfhorqzy.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gltdtuqsc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gfofykjhn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gnefzfxzh.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gwelgedaw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gcapymzpr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gaipesaui.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gobkugino.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gzuylmdjr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gbedasqpx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gvxvgnsam.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gytvyuezv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsubjuspb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gyyvaqwfv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gvzfqpqom.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gpmbrqllh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gegzfelmn.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/grjzggtdi.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/grhuamjsu.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gsqgjojbm.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gihtmkdne.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gzgvgdztc.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghvgqnaxs.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glwtnuvqc.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gpiqmicgt.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcmqucltb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gijuuhbdb.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ggoruzyal.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gfhbubvxs.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/goylzpiye.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gwahioylq.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gicwsxudj.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/ggiwtrhgh.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gihissdux.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gdizjqzmk.sHtML


<!-- 参考信息 -->