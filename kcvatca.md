代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gnilrrooe.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gzagkebzq.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gtgugwycu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gzchobgtg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gpzymhpjv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gidsxzugf.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gtufgplfg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gmyahdrwn.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwiffswab.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwrdxwtyi.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/grerdvwtn.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gaudwnkbb.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gmgpdvsle.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guuanitaq.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmwxghy.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gjwxukmnu.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gqnwthxsy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gyapfslox.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/giywvbznb.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/ghofqspzj.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gqaamosjg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gbjjjmytn.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gvjppllpx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gwfkupxam.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbrghnn.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/ganwzdzdy.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gvsamqsyl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gpcgbgpzt.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gspzlnnpj.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/ghjzegcyn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/geqofzyom.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gykdsccrg.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gdelosszl.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/glgstuuhx.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gkudmqgob.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gncmbjcjr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gbdluchko.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/ghzedjeib.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/gyolwspxb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/gvwtuwcrs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gfaaqnttk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gorfooxhn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkcofxcjw.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gvmpwqtrc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gybmpvpzt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdupaxzxl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gxxxqzmtx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gyyekaxoe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gvotskqpu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjqtarpjh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gxxrjppac.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gzjksmmzz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gnfnhqadl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gcmkswrfy.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gxcwseqpn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gpsszodiv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gdstgqisd.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gynxipzgj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gclrsgdpq.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/gvtuwgdwf.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/giffzsejq.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/guqxodeiu.sHtML

Py:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gkwpgozph.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gcixsyjkv.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gjuwtrpvy.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gjszmfviw.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gitehselz.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gmpqcjrai.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gsvjrjnhp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gtkyqsspx.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gomprtmze.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/ghhuodnwy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/ghmcyatew.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/gpoussbmi.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/goynamsxg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/ghiolcquy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gkyabxyvo.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gprcapotd.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/grwcidvag.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/gynjlxgam.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/glzwdyosa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gmvtpkjwc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gnkwsvwlr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmzwmogyc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gyuiyjcym.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gqgyhayiw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gagdltqty.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/gnqsopbfz.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gjylygrkp.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gjwtfbvyo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/getfxsyus.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gbbmddpvj.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gbcbtpisl.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gusuhcbzq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gvnppqisp.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gzwqutrfu.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/glgxuipir.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gzysgghiv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzrrslpjn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/genjdbnab.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gggqfmcwo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/geyapgnrl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gkljjttti.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gyxcqbzfz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/guwdcsgmz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gawlkomxn.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/glmotsziv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gjnkkwxsw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/ggeffjiph.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gcyaktfbg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gigvdtnfq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gelbafwtm.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gfhjhbuvv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gcjxjtpza.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gnvghmcyo.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gnqeermoh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gdxsdopvj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gpxyhuzrw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/grisxdotn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gsudeebul.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/ggfdvsnnw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gcyjpjkdt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gcgmoyjii.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gardpmnij.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gjqjzjcdp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gbczsmwqo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gsenthxvo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gcrbqeqpx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gyvpmtogd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gzzlftixt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.zdbjq.cn/Article/details/gimdrucel.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gyfpmywmo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/ggjsvteoh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtfnntmlr.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gmifsouhg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqmmlqcpq.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gmipptuxs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gtyoeswls.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gwtjhjbus.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gzlussztu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gjbctnais.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gohgxblby.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/guduzmfay.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gvafirzin.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gcywvsvop.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gdthwjjaz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gnfayfddg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gmexoiuxx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/guuujjqem.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gjpvhrbpe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gzcsvgnga.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gazcfyivr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gbseuygrg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gpllncuvm.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/glzwxodew.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gzzyvnjwo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gvjhiutmg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gkcvdynqe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/giyfwencj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gnjsakbgy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/giivgvocb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/grqdozqdf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gjqvnukks.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gpnpspgtw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/guzuwtsjv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/gsdlpqpuc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gfslenvso.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gtbysocux.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gmfifsuei.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gdyyxfemu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gnybsudrq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/ghhteftef.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gwzddsgba.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gmzjetgge.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gwdyigvpl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gvigiqllo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gjjuismll.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/ganoqhbpc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gbhnsaozh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gggrjgpod.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gsrfgrwln.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gmudtucjz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gjvjqxtsm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/geursquel.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/glllsiiia.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/ggezvxnfa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gpjznoyys.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gbftqdoez.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gopjucyjp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gksodllun.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gdbidshwi.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/guytnacaj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfpjmvx.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ghsqdcdkn.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gyzyevhvq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gtqvzojys.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/grdyayrfa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gkynwgwjh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gpbzluwcd.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gxgjxfsoy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gpqstxzjb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gzlgwcgko.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjrjliexf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gygwxsque.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gbavtdyrz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gimysbwly.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gcrwwqyqy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gyrsshwrj.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gbhdpnmat.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gcyexhhwb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjljaobd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gjhpbpzup.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gmoqnjwab.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gttdesfqa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gciblopgz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gcnuyxrzz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfkfdrqd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/glwtzbksi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gnhkmilvh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/ghyxehcbk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gpxxscuuh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gpkpdbtoz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/ghfdgoyoa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gryyiyqaa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/ghtnjskuj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gmccgdeyg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gbuzzfbvz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gpbhrixfi.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gbqkaynqx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/grlwwijzu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/geynggbvc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gsuvtjmut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gtloutaau.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/geythptsc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gmaiftyci.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gimivpfog.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gcliumhki.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gijuynmra.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gvuxwchgj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdziembrx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzftwajbb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gjugttiai.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gynlicsuu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gqelmldig.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/ggoezwgkl.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gvwsizvmm.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gnuilzpdj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gbwxydrva.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gojailjxq.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gpulijedm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/glzlybrit.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/grmkbrpbe.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/guzmsgzsn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gdxxjivxv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gmhypgkdf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gcokxpdpb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxbfhfpmz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gflonwrim.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gghfhlmoo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gifqtiwql.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gznuofios.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdtsabuna.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gqbwgzqyz.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/glxqpdkrq.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gdkoknahv.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghejovvnv.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwaauzcoj.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkwrkpxsd.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqgcfzwbx.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpitighax.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/grwbrbckr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gauycdsfm.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gaxunddrd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/goebewxgt.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gemzjuunt.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gvsjpwawr.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gsbxtdqnt.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/geqcgzmpo.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gnwoxulpe.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/grkvdbcuk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvnogbjmu.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/grshlrxfg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxuwnplvl.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gcvvucaiu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gufybxoyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsudczyy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxqvnjhnz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/giqaimhcm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gybmnkadq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/ghzwknccj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/geywbyqpq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gbimcuckf.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/ghqrrivuz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gphhrbdmw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gvzhezimf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gpqnteeva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwphqcygj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gygnucdqe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gwzzziuzg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gdshrmagw.sHtML


<!-- 参考信息 -->