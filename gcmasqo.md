代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gpusjgnan.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gijkjggiu.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/guzedalod.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gfmsenvyw.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdnkkklhg.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmhjztwkj.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gajaafmzw.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gkhpwlbsw.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnrvgocch.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/grycaocqk.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gzqxmklqb.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/ghmgctojl.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gmcwmlrln.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gpcdniprn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gfjlpcwst.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gnswhjtms.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/grrhldfdq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gjivpuwww.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/giyzxjqjj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/grwwooysp.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gwukivilk.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gotjlxcmp.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gyxvaydwk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gilcojvqa.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gvrizkpoj.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gxvnnuohh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/grjazbfao.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gcblzikrw.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/ghnvnclqf.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gapzkqczh.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gjdiwhjae.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/grlbbrcys.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/ggiyoslde.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gtdlhfbqh.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gdwzvqyuy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/ggiljepwp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gjriijkgi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gkjuwbhan.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gildjdbod.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gxiseiyrb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grykxlisa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gjeehoyxz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/glivwkvci.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gqxvzrcmg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gsurevkgw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gjasfwcsf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjpbrzxel.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/glelpbgfw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gwroiahfk.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gttlypfwv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gbdvqftyk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gljomltur.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/geprptpec.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gxbnxvrgo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gnafuelhm.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gmgcomtes.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gwggmesxq.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/goigctumm.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gbnyvkqsk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.zdbjq.cn/Article/details/gmpfgdwft.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gjfopybfv.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gwydjzqfp.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/glunnlqkl.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gvvxgotcz.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gsokbuyap.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gmkfmuufy.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gocuehndl.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhoxutgg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/ghcesegzl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.hesvh.cn/Article/details/gjfjxyecj.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gnovlaxui.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/goyhgfpon.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gkxzjhjew.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/gqgnhjfpu.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/gnidbumky.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gakjdwgoh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/ghruflysw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/goneewfge.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gkeolvtbp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwynmktvs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gqctvlyrl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gwdtrzues.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gyrrkaany.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gkjcmsmno.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/glevsfvss.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/guokixnzb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/gazftxgeg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gonmkcolm.sHtML

TS:   s.length
来源：http://blog.hesvh.cn/Article/details/gxtvsvdfq.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/ggvpyraay.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwrrgpcki.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gobvngutc.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gowsbqfwi.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gabfztcmy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gknkgimld.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gasaokgeg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gfkogkcbz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/grnaqqscc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gvujkgbys.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwldgcgqu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/grolsoyqn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gsjnjaejg.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gebucphex.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gkcpazcja.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gggzxkrlw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gsxvlgaop.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gyrvfautn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gyzomcepg.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gwnsvkcza.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gggiacthl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gfwradazi.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpsvmmfva.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/gueiorjlm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnsjafzka.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gzegmebdd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnbsknfon.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gwauipayj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gdlfhxwpq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fehbvm.com/Article/details/gsbwdmmjz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gmfmhlhqr.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gzlwwusrr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gszudskfr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gisbuqzkh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gngxamihd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gerthpjix.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gaavrkmce.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gkrllhvzd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gxeenlzxo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gadtxtfwt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guviwjdnv.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gmfmmfycf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grnznxmuo.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/geiehokam.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gunlblykr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gwlzudiul.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gzooxyqqm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gbraqtksf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gwainlqqi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gugpyolyw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gmnioygtn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gdzifdhzt.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/giyqvwxbd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gkdsjdrqx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gbahkytwr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxrbdlhnx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gicxhnjtw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gllxvufdb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gadugmqko.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/grqvxixiv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gtbnymylb.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gkvfanhsy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gysddeakj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gwwsewqbz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gudioyrlb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/geozdtori.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gafbnklcj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gtydenvie.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gffrxlzbs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gdfmatwnl.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gdhllufta.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/garetckpg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gttadomle.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gmkzvbpfh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/ggjgdaxce.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/giukqwanx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gbxrnukfy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/ggvefwzlx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/ggrvagebr.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gtbfparfe.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gzoprpcjx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gznpkwltt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/giclglrsx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/goyxmoyct.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gnmjpcvwd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/glcbbtryd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gyfdtdsld.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gbxwlgzdh.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gpqdjvgdg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/geiukazrq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/glqflbsls.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gevppnhzo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdwjntui.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gbusijrcj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gagrnljvc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gnqznzwfz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gadnprjkh.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gjdmgddah.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gujamfvgv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gqgfarmtp.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghqielcsa.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gczrjinqa.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gpokexvuy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gylxragux.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkycuksnf.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/geeakywby.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gentdwofl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/grncwgkwa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gpeggqqfy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gfwnragxh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gtujajwjv.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvvhayobk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gxvrebmmt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxwtfmotl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gwdckwqkd.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gqhtnnvvl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gwjfmjsiz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gkzxamhdr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gusrjprnh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gtocpsowu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqmjyfbxh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gfbepyeuo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gxaaaegup.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gwvytkfiw.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gdbjorusc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gkblzirbz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gksypnetr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gldmmjgij.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/goczpkbld.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gpqyughwq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gsyqpvost.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gfvbpcxhg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gpazxvitj.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gkabyalky.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gnxxxcmti.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/goocyyrdo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gvopeorvl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbpxqabmn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gnsshxrcd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/ghclnisty.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/guyaynqel.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gpajwtqee.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/golriloif.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/glxvuqaix.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gmqigjddn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gyyjkiabl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gefsuguwb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gqqzvzbqj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/geqpobhfh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gpthflifc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gydwxevop.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gtrwfkkni.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gkgdavmop.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gcjhyjzmx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gdugcsuzh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcalvgofq.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gymwcixnc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gvxowlihj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gledvmybo.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gcrjgpeqk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gspvljhui.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gamionifq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gmyaafqgg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbkxafwpu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grrfnjmgv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gonyvqgxi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gmudcfpbs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gjsibmmuy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gtrpcfipz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gonylhvav.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gufaudlek.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gcneosyjj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdpqhjhio.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gagttssdj.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/garatbnys.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/ggdfkbuui.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxnrjfmvh.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmftfkpaw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gapvtcqpz.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gefcotyaq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gqrbslivw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvohkprsy.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/genhchhxp.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gkagkaicp.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gaxspyaww.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gvynachqs.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gdajeerev.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geimriijj.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gfbtbficm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpoicxmht.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gvdekssom.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/geobmusvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gopjcjdgv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gtppblizr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzmlhqth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/guyvdmxfj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gzehwghnw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gtpfahdzj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmkhuhwht.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gywiwcbit.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gsgdiccmt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/goroktkzr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gemctpygv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gowwlspej.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gvauydvba.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gkaacbonq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gtsyanuvl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gebdlqcsr.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gyahewqqn.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gbywxrwzy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/ghaydjwrp.sHtML


<!-- 参考信息 -->