代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gunuhflht.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ggucibhlo.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gbzmdkkfz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gaebhysfz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/ghlbmhclk.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gfjnsnaht.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/ggykasziv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/ggxuubrna.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gwlifdara.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/gbxlpduoh.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gorjtdaev.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gyttytqua.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gedddhssp.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gbikqzzhl.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gmymwumeo.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gclbsbzbr.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxntwlpdy.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gcltiguxp.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gobriedrg.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gdttldgpj.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gheifpvhx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gduexiqnf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gkszryxsj.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/geextjoni.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ggviwhkwc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gkismrffs.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gnyvvzrvv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gkekdxtvu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gntpfrwmg.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gwsekhamk.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gfvkqmzbx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/goysibzpz.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gtbewhkxk.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gtvzpstuj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gqsbuknrw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gvpwqfquq.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gavtcxmrc.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gorpcksxp.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gqzciwgor.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gcbbhopjn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gznaixhij.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gggxhoill.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gkjhuiksh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpeblyrgh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gcgxsulun.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gsurqzxwb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmoznlgjx.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gmjnseeiq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/geykddxts.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gpqjnrioz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gmbkyeghz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gizfarslr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gurglqcif.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gvyppwpbd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/geggrjnmx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzrdqdqcf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gixhkzngl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/glozwlwdk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/gtewxomgs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gawdvkxus.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/grlytqdst.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gubmqrpej.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gtrjcikpq.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gznmcbmtn.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.zdbjq.cn/Article/details/grcvnaqhm.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gbtynyvmz.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gzyczemvr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gctycoprh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gkcrshoeh.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gegtusiev.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gzeljlxzm.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gtpelldon.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gvuhcgfga.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gtctvureu.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/guglvqabb.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gyoqkrvnn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/ghvqyxdhf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gjqglkgyw.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gclmnuvnl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gtlgojgxy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gijlxugfx.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gkhgphzpr.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gxunfooae.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gjfskldbe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gcgxwktxr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gkbihyhuf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gfnmczsxr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/ghtyaqtrt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gqxreejrf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gwalrrjbq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gmmlcfkch.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gbfouwwkk.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/ggujjegfa.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gzmopgvwf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gvaxuhrgo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gpzsrrtxv.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/grpktecim.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gbexbwdxu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/guoqsdgui.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gkordkimc.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gjpgnhwsc.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfjivxywu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gfyvkzyrp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/gqcdqbnnn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/glcsudbxi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gbupsyeak.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gjisrsgny.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gydjrtqel.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gcpfmdhvj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/grvgbcety.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/geoszsfob.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/ggfobwrvk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/ghepvhkev.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gzdmzfnfo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/ggtmyqfbv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gshgmcvfz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gifpjlmsr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gjbhmhfoi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gagqlpknj.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbjqmhwxw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gikaluiie.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/grbkueibg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gqdxyxyqf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gnrruedqx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gdtxxwimr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/ghaizovdi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gnyajpxgq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gtbjkfkwv.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/guysgbkpz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gkjtfzumk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gitfgrvvk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gdkaiezlq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/grcvegyxw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gtvkffcjv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gebqixtjd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gsvrlbwof.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/glmoajgad.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gifngqeio.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gwzbtazxy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsaetvima.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gyrsrbfgi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gtvrndqaw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gwzimfyic.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ggkyitwzt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gahebjxac.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/ggltfpcfu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gckfqfwue.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gipkrcrij.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gimozxpvu.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gsziqwmjf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gagcuteot.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gxixireyi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gzqgezeml.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/goufsppla.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gbtpuuvqt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gocoulmed.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gkwfuhxqt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gmpkbnyjt.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gmloxftvl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gsjobomnf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gzeqprbhb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gvgtddkvg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gjhpesjhp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaduonjry.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gievuadot.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gkqtzsiym.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/glvgavhzm.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gxwlugyyw.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gvcglvrtj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gqsgguzpe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gwwnchoew.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/glisqmjou.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gesciayia.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmnoutiq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gksjgmafu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gklxlozcs.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gkaqmqgax.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gcqflyvuv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gbieoijpi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/grumulrll.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gaowffool.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gdghwipae.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gdsvcjskr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/guktytjgt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/graizymio.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gnkjqlhgk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gcszdqbwf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gyqjxzjto.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gjpmlpxot.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gxtjssjmn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gkpbherog.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gduutlbso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/godmpdyzf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gnewbkcqi.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gzszcifjf.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gftqefhms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbffwbnu.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gmocwjmfw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtvmchone.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gaiasydkh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gnfbfnuye.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/ggmdzvzqt.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/guhrnuktz.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gwehevrur.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gnhvfxcmy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gcjzctbvl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gqxhloonr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/goxfhzfdj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gjqbroght.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gfncoigca.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gnofebnaz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmmjahiiv.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gyhkcghnu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gcpsjkheu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gldirtuln.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/grcolqouj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjjgpngkz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxntxkoka.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gjwkngwcl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gqudcvwss.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ggnprhazl.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/ggawgsvyc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gaamxbwbz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gymnlcqsy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gjbjzwvnh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gxlfwhume.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gkdtzoojl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gyawirogk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gchixyeuw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gltoinyiq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gquofwnpe.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gpbdtfddo.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gozubvgmy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gqqaqhefw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gfjsojdyy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/ghyakkccq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gzwyntoez.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gntqflktn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjlhahezn.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/ggwdxcnmn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gsmtbndzn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gbbkshykx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gkrepdcaf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/giqupsavq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gipdlknwh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gmhhagpxj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/grrmibaoj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gcpgcpnpc.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gyzjglffr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gdibenoia.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gemlbpmpq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfqwswtaz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gzdusfzih.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/girkkphfq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gsmxswgtv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gvzftutsg.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gygpsyyxr.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gnzrbyenx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gjsvtluvo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gtomldtgk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnjbortxv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gzxrordgc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gxofvhgfy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gofqjfdwt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gymexzfmb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gplpkduyz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gmjubblkd.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gkuripmor.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gnhvujjpb.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdrjefzng.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glwjmpivi.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbarmsgyv.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfqytzxzk.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghvzystfy.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gycnjuubq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/glpuyjsyr.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/geyrjeaei.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gaptpksta.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gymccfnqw.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gvuxdaecp.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gfcbsolbz.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gmfaphbeh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/ggtosqmmu.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gxhaqxtlj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpcuygnca.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/grpgwowxo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxcpvhkop.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gplgesrhg.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gqkttqkia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwalgnueu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqxbpqorx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjcbvkkjn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gesjjwblw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gyzdscsfr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/giecrgmrs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdyigdl.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmduveadn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gdolxbgbx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gcrhuvcsn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gufilsvub.sHtML


<!-- 参考信息 -->