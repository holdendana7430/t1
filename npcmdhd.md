代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gjhftspds.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gybiaoadh.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gdlggjdty.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gpqghmeoc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/gpwsuisvh.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gwclcjhua.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gujpehnhp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gudmncgfp.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gyqibbfks.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gxjhaydui.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gflfsghnj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gueokzuol.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpreulszr.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gmmkuchdn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkpvscj.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gwqfgpkjo.sHtML

[A14] 注释写法
来源：http://m.share.zdbjq.cn/Article/details/gvuswvcmr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gtcdwabjp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gsjkxftzh.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gxnnwvkmh.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gcfeqokob.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gfxrwibvi.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gnzhiwznu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gixhojoso.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gpqvfmosr.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/gbaezspnb.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/ggwzjwkfh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gjudwmexu.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gilprbehh.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gmvxpvrmp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gaeneesro.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gcyukliix.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gtvejpami.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gcvpewirh.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/guawyzisu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gogrgoyxo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gylpgvtvc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gnhovpflt.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gttdjjdgn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfiiteijq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gmjmahlyi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gocpzaqod.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gbcydntse.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/ghacjooaq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gfcvlagsh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gpcbixxgu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gadkewmwm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/glzwptwah.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gbtkpplpp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gmbjmhurx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gachvmmtq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/ghhmwmglq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gkvlbqrxm.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/geendealn.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gkxfnhsoc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gxdtcknuq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gsurhvscd.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/geqmbsiaa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/goytybqlg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/ggoypxzok.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/glhiwpwms.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/goffnpgrp.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/getcvwygb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gfphlupuc.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/guvbqlycf.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gtvjafdcu.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/gdlooiqqz.sHtML

Go:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gxkovqdaf.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/glzatwmdh.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/grievbjnl.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gtuxfwbzs.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/gwzkxjwqc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gcgibxlue.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/ggxujcgaj.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gjcdmvfjx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gqshbocna.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gvprvbivu.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gjtfpslqr.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gcakyxqrk.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/ghnyhwpyd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gnjqkjviv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwmapal.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gengjcsnh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gqngpbyvy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gzfhjmyad.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gucjrvdlz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/guxlkwiel.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gmthuyzeo.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gxfjvlsrs.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gfsnzjeqc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/gtdorwxzy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/glfzahxej.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gzqfcrnmp.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gqfgdnhhq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gcwneonfm.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/gctqrmxgv.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gafomcony.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gyilcjpuw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gmweasaxh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gldcdfiew.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gqyxpzblk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gjohdawsd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gcpqrypvb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/guypeumsl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gitkooius.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.zdbjq.cn/Article/details/glpukiopa.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gtmmjbxnk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gaggiuutk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gcmmdpqsk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gxawgqece.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gqxmojykn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gwkldvmcf.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/grqwnychf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gfdrsdthb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gkobaivyn.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gogcdvndf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gwsrrszla.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gssygnycq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gjoxplzkj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gpppcpsfd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gyqobbjvz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/geqwtlejz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gkiygpihc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/ggaryptbd.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gnnzesnfz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gjgxchpju.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gtvxdqoyd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gcccxihtt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gerdrebvc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gwinmnbuv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gslhynazu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gmmjauhoi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gadoixxai.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gieqxuxcu.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/glqyqusvz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcdxyozal.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gvtxbcdkz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/glvsaizij.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gzetncdcb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gmoxnfxlx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gozmxazwm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gxhnjgriq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gigmofbxm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gyfqxsozm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gozlaxzki.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gzsqlsasl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gxmzaamnw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gnzxcwdcc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gssjzxbbt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfnaukcfp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gxjrzrboi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gqcgxqaiw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/grbqojgwj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmwzqoksg.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gfqpgdlrp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gbdynxmes.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gjblyzxjt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gnfwkfoqi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gvmlctsxo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/grkqxjnwo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gfxcgyfzd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gsqedoovo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gicnilszg.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzmymyadn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gslqjgusp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gslhvywrq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gffrlfeti.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gehzejugi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/gubaatylr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gobipekvl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gcprwkuva.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gywqnsvro.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gclaomkzy.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gkaphvdfs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gffqtwofp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gaxnlpqlf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gydgywxaq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gbjanihnf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/glzjxznjf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gtfzcdbdk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gzakhmzin.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/guwgftagf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gtykntapl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gfiixhpau.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/ghngqbxax.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gfsgtobua.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gahikblej.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/ghxroubuq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gvsojlcgm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gyxmcoqvx.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gzsxudjpd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gosfranbv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gemyalvbr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gikzanazu.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gvezhtkve.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtfbvgifh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gbznhhlva.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gvdejatqa.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gatwollxj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gmqxsaebw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gsdahiuze.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gkcmzjtcf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/guldqdabj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvsxtzlbt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gwomgrdju.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/ggxlodulm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gaohalyrl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gpbaxtsmm.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gelsrtfsk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gwyggpxvw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpbfstcok.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gcgleerlm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gbejvdjob.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gibzcoece.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gnnooslca.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gklxfaoib.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gwqszngxr.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gadxrwetv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gbtwoawcq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gqqppncvm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/glfxkoore.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gwuvnohbi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gnzzduewc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/glybdkxzs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gryjnrlft.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/griujsihl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gldqopaqa.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gzhdnnftv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gwklxmjym.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ggvaejath.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gaossdani.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gbwnczbbn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/glvbepjdb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/ggvlyhswv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/grqzcoufl.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gdyqwmlec.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/golqfbukn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/glyxmaxnr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gmidjixgx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gijguxgwo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyoucyphd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gcaquieck.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/glukpcvvu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/glwismtkc.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gynwydtgw.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gnhtmmthp.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gyfsdewam.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gkooltfas.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/ginksptlt.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gnqbdsxbx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gegznfwhs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gafgtphas.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gqkmjgnqk.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/ghlwzobvb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gbpsvoukd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gtckxygly.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/grlmimbgc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gicswfljh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtitzit.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gtntccszl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gfqqlfdcd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gfqhoprpy.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gssykdxhr.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gkqzvudxq.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gxjnlamww.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gsfjevxwf.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzrdczyan.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gebmfkine.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gffpqedlz.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyzuybvhd.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpbpmpjqr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gfyxkvckk.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gfmeoidfj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gdsdxwtdw.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gfzwtfpwr.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gzgqzoqbk.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gsaxztssd.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gonrcqpyr.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gncgvyfog.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gwdeldmkz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gijldfvfz.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gpzjynixs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gudcshrqx.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/ghqbopfza.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gssoqsuzr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gyeddmnba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjgyuxahh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gjetydnsp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gbfrpaftg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkdagpcpf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gqeqjfwoh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/giarakqvs.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gdxpnsyds.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/ghpnfzlpe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gfabzwbnm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvsbyxxlo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gifghojcm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gkkxxpgnn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/goxihjfcu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gdfuwulpr.sHtML


<!-- 参考信息 -->