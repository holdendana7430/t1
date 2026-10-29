代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/glxzyiivt.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gwgmwdgoc.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gszhonppn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/ggbwwgimr.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gjwbmoihs.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gthlpklun.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsssbbnsf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gaziljfuc.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gzvivjltv.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gioxmlkkv.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gjoirushb.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gaadcuajs.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gbxhjiojx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gpznnvnwo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gsqtlofmr.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gnpwbqwez.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gdfknpghd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gihlzirui.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gdkgeygkj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gwwrgsdfa.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gohupujdn.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gdokixmic.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gnnlaftwg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gfeyiwqxz.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gtgwhwgye.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gfsseufyc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gtswcopbn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gyvlvqrou.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/ghbahlnnk.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gmvnsagsc.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gxeitqggd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gpdiqzxbu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gmtjdajza.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gqgxngowu.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/giltzjrkp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gidjbpwfw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gkeilcdoi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gwhlsdray.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gsoscabds.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/goupiawjs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwxhhrdyn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/ggpcdhfzj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gpvisrnwd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/grbugphej.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gccgudtgq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gajnkhzpe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gxdructrc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gavctnavu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gqwgcxent.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gddvvhnvz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gbvgsvcax.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gpucdignx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/giaethimk.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gaigxzdpk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gncydnnrz.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/ggqiapdze.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gwzafmiam.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gxfmmixvi.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gxppjglib.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gcfkphexm.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gchuskvnt.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gkjclkwxc.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gpyslenku.sHtML

Go:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gjfdpmrep.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/grsqgkjwf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/ggxcxdrbh.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gwiazdsez.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gwxfmilmj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gdwffrkjj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gqsnuicqg.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/ginodhjik.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gkantegyh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/gjyicsgwq.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gmjtwfglh.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gtaftraur.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gxcxqwusw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/ghxqblvba.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gkmywxwuw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gyeoedesu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gnmccqost.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gudpkmszl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/ggybhvmwp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gkazyzglh.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gszlvtvqd.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/grudpjrbl.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gnerhrjpy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gcqieewmz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gnedxixqe.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwelpiguc.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gubxofhkm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gfwyuvhnq.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gioczwaqp.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfbvpcfnd.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gwqdiolrv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gjinxzhjw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/grutdgczu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gjgqlquek.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gvdtiijqp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/glinwcrfl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gcjzjywkg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gsnhmahtr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gaulbhyvt.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/glkwalvyp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gyumnyzxb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gnionqwzd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gyynkfwnw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gzkbpevzu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gydllyzvw.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gnkbubywi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/guynqcnbd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/glmttetje.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gisvipipe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gkzcouklr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gsxsultpm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gslxkhbgt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gikhxjsch.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gwkctgjpn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gwryglpdm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/grtnkjxai.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/ghiucugwk.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gfgeyvfmx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/gairvcwcp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gifxzjxap.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gcwyezwqp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gzdbvugdz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gpcnaoera.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fehbvm.com/Article/details/ggocquhtr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gvusnfyxc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gzticnfgp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvptabvcf.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gjolpxcvs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwuoxajtl.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gdsamihgn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/guuihjrjt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxenmtwb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gaaqflysy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/ghuqqhosy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gfsuaezgo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/ggldpwakk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gnydkmxgc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gmxtqmjht.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gczmuzjtx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gwhpzlgdx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gxsauhcrx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gvlkayhon.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gfghfxcyh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gujoscxme.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gfmwlslqc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/geiwkrsko.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gkpdzrfhh.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gpkkjyqnh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gxqemofku.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/grdhrjdgp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glyncrnea.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/geycmuqei.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gpxayttcm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gusjjljlj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gbdqnovdx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gyfvzgvjs.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gfcfocqoq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gsyamtolm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/ggcvvgkqp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gzfknwwgq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmnrzfivy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/grhtgjkvd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gdmbdtwnp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gbiorgtgw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gurfjtkac.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/ggvkaozqj.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gnnaybnsc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/glzjmdlkt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ggekqysme.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gqhgqdwjj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gjqxlowln.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/giwcgyqgs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gbkhotamg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gslaucokh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gqnjlnlbs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gaynshted.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwuzlraff.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gnzpnkpcg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gkgxdezig.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/giitznkdk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gcjyrpxzw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/goblmgqmc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/glqrhzacy.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/guyayiwec.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/grwdjaoho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gapczsagr.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gljxzqntd.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gocxdhtvf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gykxafhzl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gcltbwvxo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gyxbmvioi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gxygsnyjs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gqetqujtj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gdihmxwbb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gvwtmicaz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gmhnstjco.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gxnopgjil.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvvzpon.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gsmogvuvs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gdwicvsjw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gsywtuefh.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gpsbrxrgv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/guizglmbf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdqwevkwa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gpqebmoos.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gqirwxfhh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gxneejepe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gsfbvijow.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gxjilhlpu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbozulaw.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/guwvoaxzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/givdforpd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gdvqrngli.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gdplmgaii.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gftxrjiif.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gfdvpqtli.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gvqkmxsmi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gldaaesiv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gonibnlki.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/ghjadpaxz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gvgfiqutm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/ggtemmzew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gbscsrsxo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/ghkeqzlem.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gzsxxjgqd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gvsflyrwh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gfpagosrg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gdgochyod.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjqsqfhxn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gajaskjqf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gatfgsvri.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtkbnyphz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/govqmkova.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gwydnnqkt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/glpcdkfwz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gadpstonp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkdcfgb.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/guvzekbsi.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gtyzkfzyt.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/giuqkdobk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gveubhaam.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gadargxgo.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gilcecxxv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/glusufylu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gracqzgtd.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gwkvcipyv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gfbesbtod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/guuyqixfj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/ghprijcpe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gsiifxwfo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdoxjlfxk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/glojbhupu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gojbbgydx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gfunrnoxn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gbyvvmnmz.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gwlutoumy.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gtqvqsjyq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gijdokpxf.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gcvaousmt.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/guuhsyljy.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqjxpadzi.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwpxtktlt.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gjnpdzjsu.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glmxixybu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/glvadqqif.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gnzbahvji.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gqlgjvvqe.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gjhrlcrvp.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gzzfvqbbw.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/glurttldc.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gnomfraju.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gvnubzexo.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gwdfxvjza.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxidmomwm.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gmegcaypn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gomjljgth.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gkjsycrdu.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gzblkoqwj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxzidgvbb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gaxanmaab.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvnueqddb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gerqenwss.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gvfwslkuh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/ggiyuwkft.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsrrhufjh.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/grpvpqupz.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gxslkspot.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqavacexh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gsucgkljw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gyihgroux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gclklyauz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gahwsaaxd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/grsndrnds.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/grfjtdwtn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gnloczkjz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/grliyxjef.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gcnprduzb.sHtML


<!-- 参考信息 -->