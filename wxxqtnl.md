代发 wailian999

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gvnwpbdjt.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gphwxihvj.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtcmzthc.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gemsaaroa.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmfzwazd.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/ghksubkox.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnybphdms.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gebxdjgbe.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrzrthdu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gpbeclybn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gopdyyfiz.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gccrowawe.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gtusjfihw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gtckvtkzh.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gwgoavyws.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwrshcmh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpwmpjzn.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvevmpvyf.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcekqpduz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgpyigdz.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gfrlprfwv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzobridof.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gfvqbtdgj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfswizequ.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/gpnfyrird.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/grlndjuqi.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlbralt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmpjvte.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdowkldp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyibvylf.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaimythz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyywjqouf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfujljqjf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gktjzpxuz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfcntgopy.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmqyxhfa.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gljgtyitq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glswmbewi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdcdagia.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmyilmop.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/goccslmci.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqygqfknq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grdzpzacw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcahwbxah.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gngnacvax.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkywdgrrn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghagfakyb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuhfunsr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowyyafma.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gwepzbzsd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fanxiaobao.xyz/Article/details/gpnhdgjvq.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gvmlghkbl.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/gfucpfjtg.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtwhbrifq.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/glnnohxpn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fanxiaobao.xyz/Article/details/gouurdtnq.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpilftq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcvbmnru.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmhszzh.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/glyfdbgdd.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/goslkjjks.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpwvkbya.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyzshbap.sHtML

Py:   name = input("请输入：")
来源：http://baike.fanxiaobao.xyz/Article/details/gfjpuzelu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucfsyznr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/ghtguypyb.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gftzajpyp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/guhzwwkrp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fanxiaobao.xyz/Article/details/gooiykyfr.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngvenda.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fanxiaobao.xyz/Article/details/gruipxlyt.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfrvfotpx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/glcjrnmby.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtkxlbtb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbdfieum.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpxfhwpy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glthhgvxy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnwaavkj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gjxgcmdoz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwudvbdwv.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggeetkmcj.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwfiaybs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/grvypygxr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fanxiaobao.xyz/Article/details/gricghywz.sHtML

TS:   s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzcvzzyt.sHtML

Java: s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfauwpor.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkvxmgfv.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqahjnxwc.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcovmrag.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsqgnghum.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikmpumq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepssmzeu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjtzmqsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gdkgukmba.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/grdoyybha.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnxcdgek.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gkfrejrws.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gfteyiazv.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhyjmalz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gtadrzafb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmrbtyc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqexlznwx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngctezkt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/ggtrfqckg.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghfbfauby.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmujjynmi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/ggxjggidk.sHtML

[A25] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusdkgaar.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fanxiaobao.xyz/Article/details/gncygndhu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvduymlst.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeblcilf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswomxtge.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gihzmbahx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfoxfiro.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrvxrcx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggakcyvln.sHtML

[A26] 类型转换总览
来源：http://m.share.fanxiaobao.xyz/Article/details/glngjyadx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtrsmxgs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/gecscdpvr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/gplzuojza.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gjvhnneta.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfzorhhh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbfzgoydv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gnhloesty.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbqnypgs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbatwlomz.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbmdniqk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggdwoxftc.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gludyujsl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrqwlgyz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhwcanfz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkybctwop.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gpbkisavr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgyhotnt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnebuotkq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnowvvn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/giywfgjsb.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrbhjvsi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/glldatfuj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkjprdocb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gncijregz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/goafrzbgz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqldkpbxt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmhlqyv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/gsexqbsqw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhgvagn.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/geinxiutr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsnzptrn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gslvgzdjo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gztnevhih.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzjspiju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpzrhsng.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihiggtq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwlktcoy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gccykrpbf.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvkidhzbd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfafsfneq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlflnrjp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrslsatx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gccydhmjk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhjwmshm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fanxiaobao.xyz/Article/details/gnfyaucti.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqszstbj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsopqwln.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhvlnsby.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/gsztoyley.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gozsnkxbx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgnjiqcr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifogaerx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrmeunp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmihoyolu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fanxiaobao.xyz/Article/details/glombazwk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfudyqhju.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrwmmqam.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjjimzp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvospqe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyqwsbun.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvussjk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtkmyips.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fanxiaobao.xyz/Article/details/gekznfaha.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guchgyjfv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gounlxorl.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/grepgfqby.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpwslqwz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gauwfmkja.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstghdjn.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxgnnyfhw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuuaxbrk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gezydsrjv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/grppgamij.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdeznfgzr.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/gruoebvmy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypsqufti.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/glezuushe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqmpdjbn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdqfotkr.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gwpyhuexg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuuubryv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpirdertu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssmfdvdl.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqnjzntu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpoigsejz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdpyltlly.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyahkuvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmwdoyjn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzxwyzmf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsinemepl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/goceftucb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/glsvwjemr.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fanxiaobao.xyz/Article/details/guoocldlt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gngmhqoen.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkktcidrr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gvnudatic.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gictqudlw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmmcflxm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzlyhexd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnmziauv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/guwybfhec.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqswnequz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncfnsgle.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glsiuhrvn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthkzupq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwfhagge.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/guyfjkhqa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxbrbzcy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeigefoq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxecuqzoz.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gduqhprey.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/glkuomlaj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqjopexd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnpeikcn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/glmstxhgp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gipbxcnuj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvfrbdvy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezdumegu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaibehuk.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbnjdrhdj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcpmrggv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwelgvkax.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyqybow.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gpqkfutsq.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/glbqfcphr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxissyrhq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gzspswomd.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/gvsurrmdt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzkfmpb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fanxiaobao.xyz/Article/details/gsrjxxyjn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvigtbno.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gracqtxij.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxhqpjcb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdminjpkm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmaxdnsau.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdebdiaa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gorejzfsh.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gowncdpki.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gmdsqhvdw.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulapbwbo.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehulcmay.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gkustjuue.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gujnmuumu.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpuoubkij.sHtML

Ruby: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpzuhoxuf.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/giwsijozl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gdfftcxkf.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsnwkulf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyxnqiod.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gyknkiwbk.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyehsbvj.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfreqxne.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghddleipp.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gjqjrylky.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gcoqhtbde.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpfsfxbgm.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gzbaxkiny.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gexvlmiqr.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsijhqvtf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaoormzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggadofljp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxspegzlz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfntmglax.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcxcakck.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwstcoush.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfkgbgcs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyypcwjdc.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcewqcksv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrubqae.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gelfskezo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltllqmsi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gksoebwkn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gzgwunveg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/gonkqapdl.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gpomvewea.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gfbnsdwzl.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gplmonheb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfifenwl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdffntbo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprctodxl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvnknflr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjfmxdyci.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpgpaca.sHtML


<!-- 参考信息 -->