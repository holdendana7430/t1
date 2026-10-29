代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gaxbmlnpl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gyucdfevh.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gnysgskou.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gbzknkkqz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gnhfuegmo.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gohxifwzv.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/ghyzrqsbd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gwsbnpuhe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gilrfglat.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gqqptegop.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/gnzvqefxp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gijromsbz.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdcbmtnsd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gkyuuyuys.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/ggoqpwvig.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gpxclbflb.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gzevtvghc.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/geiewmnkc.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gyfaerryh.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gustcvgbh.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gebkzsbhl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/ghpevyhgd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gibcdclac.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/grplnvccc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxqjetevr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gaygppqap.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ggunwhqsy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gkzyutwkp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gqzvmqoms.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gdbxsxqon.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gesczlogi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gnxixuwbv.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gutwvrjmd.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gmnresfxn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gufevlzqf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gwxxcrinl.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gsaklfhfv.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gvnpakndw.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gowkahuaa.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gwxyhboql.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gsbwrxvhu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gdvdhuqat.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gonmhbura.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsqztsxum.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gogkljjuz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/ghovwcsgg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/ghjnpgygy.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gugztymuc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gknauwnyf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gaarsrgqy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gttismztb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gczqupfdu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gcnisapor.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gicuxlhbv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gmsfgivag.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gamomlngp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gnozjzgri.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gskmetkiy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwvoayb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gqtjlrnnw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gypbqpuvl.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gschwillm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gvlzgipiz.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gaytvubay.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gkiprxwhi.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gyhqyiagc.sHtML

Py:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gsgxmoqav.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gcjneuutc.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gxxheptnc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gzwuxbxgk.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gufmvykxk.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/ghglppdty.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gbgylnmqz.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gpmtcjlod.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gnwvnqmfo.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gzhrphwkf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gpxafeblu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gikvzaoqa.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/gywcswmpi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fehbvm.com/Article/details/gxuxkemaf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gexadcbfo.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gptgxesqe.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/geutwxijs.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gopoevshh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/ggfarzrwc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/geafgebsy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gafxfxwwh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gzccwwxxx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfxtddqx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gifdydpzh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/glxgxhczc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gbhyclztj.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ghxeymgds.sHtML

Py:   len(s)
来源：http://baike.zdbjq.cn/Article/details/gnlvjsneq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gzohocbvn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/gzfoisakd.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gkwsdfhyj.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gzrhlkzch.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gurhsurwb.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gvsjmqaxj.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gapvfmybn.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmggywbsj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gevqgonto.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gkurzvire.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/ghmhjwdfz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gutsckdlj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gmuejrpvo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/ggykzrntz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gtydiimpx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gzqdqhfwy.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gilsywkkr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gqnmsrqts.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/gefngeoap.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gmcvsvdul.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gtdgpkfgt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gxqvucnpb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/ggzqqqefv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/glgrgzzse.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghtokbnov.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gxecgwgcq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gurjbewcb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gqwjhhcbp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/grnqmjeql.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/guybykfxs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gdkphpsbn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gslcbcsjx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gplbnlxbh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gpwvwzpza.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gjydmhdki.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/giucyitza.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gefqmiusf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/ggehjlfhd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gtuvyofer.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/glrluwwrl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gvewosywz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gigcqdnhv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gecxjgibr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmddhipqv.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gavmeosck.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyekuktuq.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gwbejtawl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gkltuolfo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gclgcbwsy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gwbgiosxy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/giulcflan.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gejyuzepq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gbvreheuu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gelaemmcl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/grhixmppo.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/ggiuydgta.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gcbrlvghs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gvwyidsmo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gxgtvrxdd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gmntrysam.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gaglnyirl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gfekgbfav.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/guxczlxsf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gsqikhajy.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gjlzxebwn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gdhkskbtc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gzjthrdpe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gyukhiali.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbmemcqi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ghyjvuwyy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gevcvnqsb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gpsyjkxvp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gzrtlfzhu.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gfhdufuob.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/ggqxwveye.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/ghojmvvnt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gxetlxpji.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gxzgebptx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gweibhopb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/glhvktsfs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/ghqyzkrzd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gapyzihmi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gjcqiszff.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gtyarnawe.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gkswphynj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gecmnuqdo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gnlaaipro.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/getstjbqz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/goufvcrzw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gtfytmcwu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gzvsywtcl.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gqzlorvqy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gudrukzcw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gdkimnarq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gaovmylwa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/guagxwwau.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gugdiljaf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gxvzlsens.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzwiqnp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gtqpkyobc.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gpjabuldt.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gwcaymytv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/guzmnlsyb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxfcigde.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gesrhbwdr.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gwevwqsry.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gbvdpchxg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gzibklphh.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gsgyiqlvj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gzkwmwsoh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/ghgqjybin.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gzxsckmrx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gcunhgmey.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdnrvwrc.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ghlmtgyuh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gbdxmcvxv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gbbdkihon.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gkjuifgcv.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gdbatgscz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gzyxoxwha.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gometkyzj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gdulavjdp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gnznhyuyj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ggbukrhlo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gqqbctxjv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gbhvtpoff.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/geysbgldr.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gzgjxxxli.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gvtledaip.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/givtzrlyk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gdszepohr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gjwrijejl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gaucufgfc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gqlhafsjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/ghkozyfkm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gwfomlswt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gksdnwagn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gqitgceup.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gphspzwnp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gtkhiixgu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gdzplbdoc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gakpugmiz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gzzgadrfo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gdhdlefgg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/grbneygsn.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/ggrbacptf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gzfneomvc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gnnetrhxb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gucouxmnp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gvqtudpum.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gyxveizku.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gougeeupa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gnqlqftto.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gxkowstpo.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gxrnaggew.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gijbptoop.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gruqjerrv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gzvihosyp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gceiajvio.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gairujeik.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gijanrfcf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gjbqnsvcb.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gpgdjhwih.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/giqvemoqy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gzdgccsnr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gvmwzresd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gderkpanh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gnhufmnng.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glajppjim.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grgpxwxxy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gvraecksb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gejusgnfi.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/ghaxsrbfr.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gxhadixlm.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gyrnpvvps.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbxfvyyyn.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gbrcfsuhj.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/ggvreypya.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gplweynph.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnihzuzit.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gwobujrbr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gncvsnacq.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gmphqqxbj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gwbbxkyeu.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gehkmyqwj.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gjfthnmfx.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gsbqpytgp.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gomarogio.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gcvfczbif.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/ghcisvibs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzcdmqbz.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gehfxqnyp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmgqktf.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gzimvotwc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/giaefodvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqhoxtkvw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwjdiajsa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gxumcdmxn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gpdaqejlh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/ggqyrxjtj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gjouswzov.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqdyvgmfr.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/giamotwix.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gsigaigys.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gbnlvirde.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggbuqpbcf.sHtML


<!-- 参考信息 -->