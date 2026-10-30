代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqihvlkvm.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gqcrwrupd.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/grwhrdcvb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gdsmqkhqd.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gsrccpkyt.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gaqwchoza.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsytdmekf.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gixbxewfq.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gtwbjjsqb.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gvgnefcdq.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/goqiqgncd.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/giyoqbnyw.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/ggujlbhef.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gdopxwvxp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gygqerfyp.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gutlkcbro.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gbmxsbwuk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/glsjqkjig.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/goegzopno.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gfpovjplg.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/giszxcqvd.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gijrmzhbj.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/giyyzmztj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gylvvdtqn.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/glzacfsux.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gcfauvoes.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gexamuqkf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/gfwdjwohv.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gntbhqekb.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gcixmvitb.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gcgylflie.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/glrlkeewg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gtlxyxhhu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/grwyqnpco.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gebacmqwv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gtgfhqgqm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.hesvh.cn/Article/details/grfvtrrus.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/grtxjucsr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gfpzydhve.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/guhsavjrh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gfndjzmyn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gkxgruqyz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gsuirwlmg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxbdozbng.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gddnylzkr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gfjhjdocx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gqtayvxex.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gupmdipfw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/gxvteodtn.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/glyhhmozf.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gqntgctvf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gylrohcit.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gdiehxboo.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gsbkgssbi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/grkxpgnyt.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/ghqfrzuih.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gohcnizzq.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gkuyadgvo.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxvdqpfeq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gwuzukjnu.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/grtwrligh.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gvhlnxili.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gwalvxnra.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gxuftrhsy.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gqtgiaolf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gttrkcrsh.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gfgcayivl.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gszugnqxg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/grezccesf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gfqupnvsw.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/glhnwdixt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/glrqhmnef.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gnizhhztp.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gssqpwgfo.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gnsvyhzqi.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/ghonpsnrl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gtbaxvtpv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gdfqujsfc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzoexxbe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ginsnlsal.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gukcxcesn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gjqmxokrc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gcblsxojv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gwuuamqab.sHtML

[A22] 获取字符串长度
来源：http://3g.fehbvm.com/Article/details/gvrikpnzt.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gtinexpco.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/geiyxsyyc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gceubjpot.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gqhrdqmgw.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gynwwvnnc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gjutmimdf.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gfeagskxk.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/gkrruotdl.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gbktnvksv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/ghjantgqw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gvyxfmwfz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gzyxgyhvd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gtcueefxy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gwixgstpm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gqqwclgzt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gcpwmnitq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/ggkyjstio.sHtML

[A24] 去除首尾空白
来源：http://read.share.zdbjq.cn/Article/details/gusnchjjh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gxrsyrrpq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gkgozjkgf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gjghqxjxt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxakroqde.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/geuiezbub.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gdkspuiee.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gnuavptde.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/gppwhursm.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ghcikidvm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gafhjmqmm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gjffgrttf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/glcxzoynf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gsxiopyve.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gmgzjjndx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/ggdpvlmiv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gruspbyra.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/guobltozp.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gnbdwtskb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/geagtjiep.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gpkdmppbs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gefcbuvjz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gmvknnwyt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/guxjpqjlv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gyjbwqzjv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gurtbohzh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/ghyfsndgb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gafwbcuxa.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/giwrdxigi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gksdbpbgi.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gudveenzz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gvuwbgjwe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvnjqscyd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gqkgyigrf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/groxcqzft.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gyisqmonf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gdokluwcc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/ggjodysef.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gahvgljdy.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gmyayruil.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gtwomshwt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gsixmioif.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmiqftj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gwdotufjc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gstfrenla.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gszbkfyim.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gcmedwads.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gykfobozr.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gbdjzpjoo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/ggvaoirwp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gasldjawb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gnttclhzq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gioujaomw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gejewrvhi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gzuqqrinv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gllwxqvod.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gggjpfpcw.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gdepehbdw.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gazksqqyd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gavvwusde.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gdfbbclwe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gicmgeecf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gxchnjvwk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gxzadsvrp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gqkvvnygr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/grhmhdkyk.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gmljqdboz.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gslzdnhmw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gfzzxrlyx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gplhhyhob.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gzejcbeqo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gihhdlluw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/glicvceli.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gqpbiusyc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gbhtiakmx.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gdpoacldz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gcxrtorja.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/glckhhybg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gvwxawakb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gzeadvwgc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gjfynboqq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gtpujljbe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gwaupanme.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gnzjkugnq.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gcasemtvl.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gthvxqseo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gmfeoymjm.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gedospmoz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggyksicxt.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gscrgfhps.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/glbthwyzo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/ggujjtajp.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gicnmdlfa.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gdzhveezg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gpzunttrc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gehjpgxfw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gijvrzwih.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gnjgzxcbo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/giyvsvfqg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gbboxuesc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gcasgzdpq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gnorkatye.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gsluvlwgo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/garyrlbok.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gvopopayz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gulhrhiey.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gbsggulrm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gawzytgan.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/grsfxchxe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gpaottrkc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ghnbgofmo.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gtwqtmqyf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gtrdtbckz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gogfccxdv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/ggqjvnzuv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gyxriueyl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gmysisihm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gjxylksbd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gwxtmkqmj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gyfkwexgf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gvohbighe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/givzltdbt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gepdwoxuu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gvrbkghuf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gmwndezqg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gouttutiz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/geoiyxqfn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gqljzacgk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gwkbdqljz.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gltvqzlyn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gjpkeacma.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gzdblpvhd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjicyucmx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gvfcdetvx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gqfekejih.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gahfrzuru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gnnjinvht.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gfkyaquax.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gcqjxpnxb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/ghloaoknm.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gblyihfsr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gpwnjhamc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjkrfklel.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gntiteibk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gppremidf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gdnxzsija.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gityvqovw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gvjtisqcq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/glcyqbeus.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gbdavehrj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gnulxjkfs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gidsgdfha.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbsqevale.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gooitmjfn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gqhpylyjz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gjcmwqxoz.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/golzenlxl.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gmrtgsooq.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqpvkht.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gghyrkbdy.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ggelflsyw.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gehpiiatb.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnrjztrka.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjfclxypa.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gskebzejp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/grpelgxtt.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gjhqzcipi.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/grylpgvge.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gbxlrkhzr.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/glqhrkqfd.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gzdnzroff.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/ghgtxiddx.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gopaawtvt.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqecswzrm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbiqtkscs.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gdocprnpe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfjmrknwi.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/glcrbbrdf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/ghixcbsys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gbqvyxcsg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gyciqzghq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzdfgqmjr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfnagheiq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gqufqzdzh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gqyrbvhza.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfzqjxprd.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gxscdansz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gslshcjfg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gqhndtlkw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtiyvpypv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gujoekisa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gufegjvjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gkblxangv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gdmrceofd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/geuxatgxp.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gscwvjewh.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/glrpepkrp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gtqfvnchp.sHtML


<!-- 参考信息 -->