代发 wailian999

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytclkku.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/glqppomel.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gtqoktgbg.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/geurgepsc.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxywoqpc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcepmhhi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhwnyego.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gfmveikxq.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/giiglisxp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnblvuzg.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpdnjuqd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbsfzawm.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpzrphgf.sHtML

[A15] 空值判断与默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gkctufycv.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnycbief.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/geyaqyxuh.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gckbbnfos.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/glbgpstws.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gdyuokqzi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsvpdocr.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gklqhdesi.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwxohgzj.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvieohe.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gykuauyzg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gishiiekc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/grzfpdkje.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxwagpfs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqjnzifds.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/gshahqgse.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/glnmxloqo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyipgumx.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/gvllvonuv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjptbiyqo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gseeynoms.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/giapuojjq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbhwdkafp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcxexyttz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqguorptz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkfplyyyw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruhlvpwy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggdvqzshg.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvonoiqhu.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gieehgsng.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gkakoqvyo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/ggebhvjal.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnipduv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fanxiaobao.xyz/Article/details/gxcvwaebv.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqkibqdh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fanxiaobao.xyz/Article/details/gjcliypgv.sHtML

[A19] 交换两个变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzitgbpfx.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeiiebho.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpvcbzam.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfafckma.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkmgost.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fanxiaobao.xyz/Article/details/ggttrhznd.sHtML

Go:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gphuzjtva.sHtML

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gjejdcavx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glydzejbf.sHtML

[A20] 读取标准输入
来源：http://wap.fanxiaobao.xyz/Article/details/gnednovyf.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/glxdyktul.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagbpehny.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfzwliqy.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgavcveu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfheepmhd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxypyfmp.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/gyykliclz.sHtML

C#:   Console.ReadLine();
来源：http://baike.fanxiaobao.xyz/Article/details/ghusykwkv.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyoajgfn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvzmscyr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtmybiu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gaahzbnav.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmovyklh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnqthhsn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyybibaei.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdxgyisa.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glepeavhh.sHtML

[A22] 获取字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsbrncryo.sHtML

Py:   len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdnxehig.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijtjzjuo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/ghfbwcitr.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gpvwiwngl.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmpqspb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyljjacn.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdyttber.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblnfqcfq.sHtML

[A23] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqdydpzjt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gkcytcvjh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzbelkfq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnscgpitu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxopmjuqm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gwibublvl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzvsuxdq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplivhvdx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fanxiaobao.xyz/Article/details/gjcrkbrlb.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaivzdyt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfnfrxrf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghctexcvz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gaihmggry.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfpygrls.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/gycwpudtg.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzpqrndm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/geqjnjcqd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/ggajnlrdf.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvyzycebs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzueawnjm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjaaiher.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgberyla.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtftduzq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsfhjqig.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkxqsppa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmvfrbb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/goaxkmfhy.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcacbqp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuccoklj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcrpbsi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/golrzmaok.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwoyvgmx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkxlcgpy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzcnvhlc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjptheee.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmtezbn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gevhpcnir.sHtML

B. 流程控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzxkjtuv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmlivmq.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gmedgszpe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/ghhwrbvow.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhdlwlcb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxqcvkti.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gdvanismb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyruqhnhe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fanxiaobao.xyz/Article/details/glqfnntas.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzcnuzdn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeumudcy.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/gygpvphgp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgwysvor.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrudhuxo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/groiazvoo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcnviuif.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvxbljbk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsgumwny.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/grrjkdidg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxsxzqtd.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/gloareecd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gonrarcgb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmcdncpq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtkvqzcd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaowxvno.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsgaxpbg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/goeicvbqd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaznwyotf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfyzlolj.sHtML

[B04] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gosqtztln.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gwvaexvnc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstwxewv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gntkandow.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpearbmgt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakzmcph.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbjjdqji.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpgswdec.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gknejwjrb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gtieznoqp.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdviagrjp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvetvizau.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmljsiks.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgjcywdw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwldybkbw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpxrmokc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/glgbqkdjt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/glgzbyfkn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/gxknhkvor.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvhxglot.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grjqearff.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtrpgaxix.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giupsbbgr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjvwqkpy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbmhgvbe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgfrokoi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/glfcymfyl.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfbygzmr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gjdiwhqqa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggnttupih.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkhznotuo.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdykbpokx.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsqqiqleb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/gdzaqqlyy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxerslhsd.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/giwzpqosu.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gmfrtchfh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gttrilmfq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gughdgplv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gqypnwklf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqelfmizx.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmatlqsl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/grsosukhy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fanxiaobao.xyz/Article/details/gsinerwsj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgkkagwb.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpipkkni.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoyezyfv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezoleedo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdjyjhpa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrjlgcz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gthpmmywu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpobfsml.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gmehklnrd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsenuehn.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiaqzcav.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibmvdcur.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goatalxpq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gvkhguxth.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuroqaem.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnmxxque.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxppypbj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/guyckjfno.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjzzmqb.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gggcdkjjn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gemprewuu.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyvkuzsy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ggcqrclbm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggtqksavz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkrpmdbav.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdirqlovi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gtppfgzbe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gfizqmdhf.sHtML

[B12] 跳出多层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbcrsgsvm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gvktyfrxa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fanxiaobao.xyz/Article/details/gqpyecxyh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaudxjmr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmkneix.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gbrhnchtr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgnjqlzl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlgfnyxw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjcszsl.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gundnnuys.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvguhbx.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgkzxsct.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmicgncdh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gcuvjzibk.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/gsabrxwlj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnkianan.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gosgqaqbh.sHtML

C#:   x is int or double or decimal
来源：http://blog.fanxiaobao.xyz/Article/details/gpinomxvq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gcsaocajk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasjcjobg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcsnxpui.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetfixzs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtklgdcrg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpdgvqdp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fanxiaobao.xyz/Article/details/geofvzoyh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwlglxbe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggabmhyfk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkwngah.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/ghilhsivb.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gcxqyeobr.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgppmzvc.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/ggbbybdzi.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gfwfznoch.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxikcnxg.sHtML

Ruby: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gmdnlfkux.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjwkzwx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/godclwxnc.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglwqvpvy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gclbwkbfa.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gryjisqpy.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrxeixj.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gekxlgvwa.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzwslfwy.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gigeakqdx.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/goeafvvsh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzorfdoe.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gffkokmpe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gealuylqp.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsvhwmfhe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoahirsn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzorfbhzh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxbetgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqhuxhxk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoiueoys.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfamdltnk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gycwhnjkh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqazjckt.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/geibzusle.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gexqgdzws.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqepknwy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacqoysgz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadkrneas.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpnfwkeq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gphxlpkel.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtlzszgi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmsnzrqs.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxqxmjfzt.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyllndxs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpzrdxvm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzyehggs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/goqbwqsep.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/givylndaj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnecsinzb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqofudfyo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxzpcxp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjyhnalqi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcbrcagh.sHtML


<!-- 参考信息 -->