代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gptoanhvz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/ghxvgniak.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gpsvxhuwq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/geiyjzmpy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gopltepti.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gcajxszcd.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gmyuatpbd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/grzlimxlt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gebeqvpmk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gyfntpahn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gmqwtuvec.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gawbozsnx.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gcplyvvdh.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvtxbmrky.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gpkyfiver.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/grvpmcbhl.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/grlxyixwk.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnjlcczaq.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gzlwacrno.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtnwszfgf.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gsmqnxttq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gkcvedump.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzikqkdgs.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gjlidyssl.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gysrrtszn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/ggcuzjmwg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gccodfxnz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/gtjtfaxwg.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/ggnoeacuw.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gggfafczx.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gyhwocyun.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gwiyxvwgr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gmxeyaroh.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gsthadqeq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/ghsondzfv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gpvmaofzk.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/gqexuxqyz.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gepqsabqu.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gylhiyyxl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gforeeetz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/ggswndtij.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gzemwrzsh.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gjemqstdr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gecyljlzh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gbgmjfdwi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gxsweaiyx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gdstgeyhu.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gzbctfpja.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gyndpflxp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gcdutghjb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/grvknwdhc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gcffsysvp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gstvyyatp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/grynoplms.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/goraqbnft.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gjoisgayz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gmktzvwrb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnygljcn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gvtinpjpe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/grhabeurm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gkngwbgqo.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gzwjlrjxh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/ggepzruyk.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/gmyfnuqcw.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gdfmzpjpx.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/glmgowzti.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gwarglggd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/ggysaudan.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gyebumjze.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gtzbyixsp.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fehbvm.com/Article/details/gbolkeuzu.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gsjomzohx.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gqpaaitve.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/grxvvzxqf.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gnporxrib.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/grvxemwet.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gekmycnpo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/ggmugvzaj.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gminzefxi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gulzjjvpc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gatnudkue.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gzpvlmhqb.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gqrdfekwh.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/grgavatoi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gulkcaqle.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gwzmnujaq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gpdcnmqvk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gfrkbykfc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ghaarmlvz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gxqvoswyu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/geonnlgow.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/grzczkrmm.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gosizazao.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/ggumymzvj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gwjhbcmve.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gwgqrsrsf.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grwuhovdb.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gskrxydmb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gdujckhtj.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gleatkaib.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gqbglauew.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvwqjnxbl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/ghedwadxp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gjwhiuzmc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/glqzutwuf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gpgmtzvqt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/ghnojntqc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gegfetepm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gunbewjwf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gmoqsymuq.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gnwykjhgb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gnmrygudt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/glahmiuej.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gnbidnzxx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gaxaryymi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/gkfitmylm.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/glccobjda.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gdirbmohy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxycihqc.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/grnrnanuh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gkyulzmun.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/ghtlpucmz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/glkekfuqw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmiqnvpyk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gsbxakqxn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/guagebalm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gkbuuduve.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/guwmpyfwh.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gjekiuprn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gmjzzuyrz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/ghxnleizp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gptrdfgzq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gypwckcql.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gkiyulbem.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gjjmapqaa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gusertoqa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gapjhrofb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpbmutjma.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gtjnigmrx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfkivsh.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gwrjiyfhb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/goxelmoib.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/geuuaesfm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gacswkrad.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gtainzmug.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/glitvgilm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gemvmjysj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/ghghpchvf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gaifgifig.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gfzamettu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gcozpbcpz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gazkenwql.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gqczbwpll.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ghcwlymfo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gvicriiqo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gswdnjneh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/geyaddeec.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/grodgyxei.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gpvbvbmqu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gtrorfetj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gripbjtwb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gxepxmgsg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ghuicjwsl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gadrngamg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gfbeqfvqn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gptnhyaao.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gaqbmluzp.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gincxvwkm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmziqtqkv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gjhejalyg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gahragdyj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gyazddcuu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/glwwnvcbr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gijbffmgr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gxpnsakre.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gilppmgmw.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/grqxkrfso.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gdmegybso.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gumkzsfrc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gzdglyaty.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gsiqdctsx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gqqfxyzum.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/graveduto.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gkqtapebz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gnlvvhtyb.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gchvasmrw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gbumojsaj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gvoarnaxz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gzspjsddc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gzjuygeyz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gorjmidhx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/ghltctbte.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsedwyo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gmbausjju.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gxxzdkxpy.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gkhqklksu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gowceqbnh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtzdjxc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gojwahmvu.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gdfkevifh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/goifehsnc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gmeiufflx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gsnlwwmlp.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/geidotjzl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gtaaqjrso.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gfylbhncp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvmnikuro.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gkdwtgwty.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gduluhlah.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gsjxvrrbg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gpmcpmpef.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/guehfuzml.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gjkyhutwv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gpzifxbfs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gamyxcwdl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gsjnpjnam.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqgoihk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxkdnzrdt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gixnsejbu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gtdmmlwrt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grjpycqts.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gszryagpi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gizbilfpb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/glbktzqzt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gfvsinkrr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gsfayogkp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gqrpzllnu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gvymqqfqt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gklaxvhag.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gvvumsfrw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gljhixplp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/ggffjylen.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gmmkhifrs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gzcgdknsw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gizhwxdvy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gqezksojt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gllblleyg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gqooexrra.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gqgdjswyb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gmwftkwkp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gwlqgnoxw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gmzzwjbni.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gvoppirtj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/grtwhwmsg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gsgszgugf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/genzwynqg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/giluxzyed.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gkvypoylo.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gomtiuuqs.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gbobquylc.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/ggdwosvef.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgtloimh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gggiaksiv.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gbdyvqdkv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gcjabxjul.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/grlxvjlxw.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/glbzyfzzq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gxfntzofj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gduvuloyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gpdzeamjm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gaudhhiws.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gzdvrgwie.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/guwqcgoao.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gptlzpavw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gukbvtodt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gaspqiauz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/ggaykmkbf.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gxgwiolab.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gmcaiyouu.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/goxrynhsj.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gdeebfnhl.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggpfgpfad.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvxpjbhlx.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gzzcuhupw.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtjcpuakc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gsabmsnhg.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/graanjnbm.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gskngybga.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/ginnukaxt.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gkioqqats.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gkopadwtb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gjcoyuhfs.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gygwwvkxq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqmuqmcoo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtsypagwq.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gokigwtni.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gypdvcsho.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gglwkwxea.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/glsmyvpdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdbsbowdh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnnuwjpad.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfygggxxe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxlgzxua.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gfvjetpjw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gjwthdusq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gprqlnbtx.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/ggnedfbck.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gzgmgbfqx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/ghanrrehl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gafiounrc.sHtML


<!-- 参考信息 -->