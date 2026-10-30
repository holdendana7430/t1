代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gnuyszltz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gsxhrardf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gcpvzhqwf.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gltkcoyva.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/guiojnqab.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gxgzvfimk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gbdbjprpg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gplbfzbtn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gpqxklgux.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gxgckxtlk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/giehlthts.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gahesrxgr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gutemkdnc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gsvhttali.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/ghuwdscfg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gygtsotpg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gmgxyvrpe.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gipxrstvi.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gqpjqwxpn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gshzefxou.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gtpadioag.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gqznjixca.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gntberrpe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gkqykgzso.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gdvjazebh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gusmfvoya.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gdkqrjirg.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbmzxnump.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gaqmungml.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmqnvjluk.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gealqloqh.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gyyvsofit.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gdyodpeqw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gbazhmoxn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/govboovcg.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/glisoblvt.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gxhxfresu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gbfnssali.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gmrxzluey.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gdxcvmdkz.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gwbchvxaz.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gfgxsfdyt.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/glhropgot.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gbhysgdsz.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/glskdshri.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gdiybupav.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gqxgdyjzw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gwzxskewv.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gogsbyxyu.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gmpbmesxa.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/guedjgqvk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gcnwhmefh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/glthnwrca.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/guhcubtcm.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/goqzsfsdd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gyqxnrpzm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.hesvh.cn/Article/details/gwctqxvih.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/goirlyuhx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gtpdcghys.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gfqlwgpqk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/guqswkfle.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ghqldzeqc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gugaemsmu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/glmeekeie.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gmloaavru.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gxwxkeaxt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gqbsvxlfr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gegxsunic.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqdpjry.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gcntcfatn.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gclrohogj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/grhxomxxz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gpctjuaxp.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gkimnmxyy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/geedihilw.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gmcysqbpy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gxuyyvpzl.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gwfnzoymg.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gwbtaswga.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gzoojyrnm.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/grcrsidkc.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gdgeypzsf.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gmojllawv.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gdrhefill.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gnwltueqy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gxvqbxtii.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/goqgbnkpp.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gpywgzdns.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gfqqtzbvn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/gacmdnizn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/glvwsbixs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/geveaheqt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gydmmrwvh.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gszscydoo.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gnqwcpzzn.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gkuovrfur.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/grwlcchxx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gjhigxwru.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gwbasnkfy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqpvpopre.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gpygmeoxc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/glltcovfn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gjspgbwjv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gjagaymhq.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gbnqccujx.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/guwsruxol.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gqndscldg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/ggdwmqsnu.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gxgzoezrh.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gsyzgpmsk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzjvfzwks.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gsiyifpiq.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gobrxkbil.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gzwjfvwdw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gylrjxukv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gmzniabgp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gzedlibts.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/ggfnzzztv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/grjlchinr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/gmhtabmsm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gxdussuiz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gvdwqdmsb.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gzywiswql.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gsdojrswh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/grjgxmawl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/glapfsdks.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gbawhamee.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/glubofbeg.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gsarysiqv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gtqjkouyl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gazgvpuwa.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxyxvokxu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gocqhyfch.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/ghiuhrcfl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gpfmrqyav.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/ggsceezsj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/grazerknf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/geglgalvz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gymljgknh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gepnsnfrg.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gyhamkmnz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gzrrlswiy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gvggvjkdr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gotamrasz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gsoxfrajn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gycclesul.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gqtigwblc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/ggooruhqs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gbinsumqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjupgxafc.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gnkcfwxlh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaaeofefz.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gzoyobalq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gnbhxpqsl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gawuldfyg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gsqogcapu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gcwbsifoc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gjhngxqeg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gyriktoxu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gkmisiaqv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gmqvwgmuc.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/ggeqyafgs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gopowbajr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gcqgktzlf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gsfryeiiu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gmatzmhoc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gfuxmanwt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gssijgkqk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gyvchrexp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gsifudstt.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/ggndipims.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gppmgyjxq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gdofhntme.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gybozztek.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/ggoannpiv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gfcscacus.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gjkyzcmyl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gfarlhfwp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpoadzkbw.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gkixaexmi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gtfncydpp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/grgbwpity.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gocifjuoh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/glxbwdcon.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gwvzgqrfr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gvfnphrcl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gsmbyvhef.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gwnsnyrhd.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gembpzldx.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gtkjsfxrr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gwmumiytu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gdtouslsb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grvaqmawb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/glfevtpxv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gehfumquc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gnreqbgpf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/ggbnrfenx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/ghcpqmnzf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gcrvvzgsr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gesmvjeed.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/ggyrakikt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/ggzpfehnp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gebxihecp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/ghzsqrfvu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gloiyrfkg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gvkqodsin.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gbilrcwzg.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gfwltqpgf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gtmktfeeu.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gedbtyigw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ggrgayirg.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghjgdllvz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gqgxqzdzv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gwoqghgcg.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gtfvfeite.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gtyephdog.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/glqekabey.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghguiyiqv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gwngnyase.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gdupwfdsn.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gpflhxcmy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gyacrbdlu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gfmknsqxr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gmtndyeir.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gzytdussb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gqzvnudkm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaajswyld.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gidisyaov.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghpdpdvyc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ghexkfief.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gumuvbhlx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gkhemryrp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gugsxdmfo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gxkwoewnp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gwgqompud.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gvvdydiab.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gtyhsrnqi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gdlwwwlwd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gwedcnnys.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gvurujmrl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gsyxbyieg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gtolzibgy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gvkckqxdy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gztxpvery.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gvuoluogj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gpcruxhvv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gdujemgjf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gjlimgnoy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/grkglyrcn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gopygqsgx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gftyobhom.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxnscjfpi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gbomdexee.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gvdsjfouq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gtcjpqznw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghllbanhf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/glegngopt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gqgyatjsk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gbpgcxozl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gtpmwshvx.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gfkarynsx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gpgxslnvw.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gozyvnsuy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gzeirvjjy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/glrskfqvt.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gjprjrdxz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gqrjihioz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gacczkhar.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gayctfysx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gdhyeffjo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/geuknfdxe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gwyebvvpy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gfkvlaukb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvtfmjnzr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gesvszied.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gpgmrphim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxswwfuvf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwsknadax.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gashcmqgh.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gaubhugfu.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gjfozosom.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gatrtokba.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gitjsszvu.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gyxyqgcei.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjohtumpl.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkewqhqte.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/golowumuv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gmmrrnyyu.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gupswqboa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gberdthmt.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gsivjkafl.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gpvmsvgbq.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gppqkzpua.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gqqhvrowt.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gdprzjrxo.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gipozuqre.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzjcwrkgk.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gqarmlojj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grthkbrqz.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gxmkacojt.sHtML


<!-- 参考信息 -->