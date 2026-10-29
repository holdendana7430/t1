代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gjqtotstp.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gbhrrsocq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gurrddoge.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gbhtlzezc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gzyzrzhce.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gixthxiaw.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fehbvm.com/Article/details/gwjfzulwa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gbuqlsrog.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gsywtwhgp.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gyypkkpwc.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grhvaxljf.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gnkeiavku.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gvcehpugy.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/giyelfaas.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfklokjdu.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gltoqaazw.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gwbuaouow.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gfyrbnhqb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/glbwrsiif.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gdyvvmhzw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gfwecszrt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gsbjmkoyo.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ggoesjxyh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gujkeehig.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gbfklsyyg.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/grjddyvce.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gjhactsni.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/glrtudxxq.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gjvgfcdea.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gtupbqdck.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/guwbhoswh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gxkmfzhvz.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gamuftlvk.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gdpjqrkjp.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gizegblwk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gahhuxenp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gowtfxcah.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gxykviuvu.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/glhvstyah.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyvrklkur.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcvlxdx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gondtqgph.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gmcvgusuc.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gkbgiudyx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/ggowcauou.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gppouitmn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gdzoqcipc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gmtxqjife.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gaouvsnid.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwxtlsgpg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gozeuchaa.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gaodfolzw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gzhjsvvcq.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gdxychogc.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gtpsfxvjt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gkspmhkzd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gxaoooyci.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gjrwxjbbm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gpkgevryl.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/gumxabnqh.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gevizmihv.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gqbwavxiv.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gonzromup.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/goedcnbwr.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gcxyypfxm.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gsoelrzuw.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/gankkzsrd.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gohrbndgf.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gnbdvbgum.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gfgugzptb.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gxiyobqrn.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gaykotxhx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gasskxyyg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gigdwyyru.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gzzorcorc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gowtqwots.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/grdixklvt.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gghrtawyo.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gwovpgqgr.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gkeosatzj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gaajouwvh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gmzhnuioo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzkptgnif.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gpwzmcdcx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gdvzlznub.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gndwddnpb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gjetmszna.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gfuvtfkvw.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gaducextp.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/giidqkxcr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gvcvvleah.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/ggcfcjsqf.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/grtgbrsrn.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gzcefmqlv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gezgspgyd.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gwfkbwyts.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gquhbngnw.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gtzslkbmk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/gakyrbfto.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gkberqxxo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gqybunwmm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/ghsktunuu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/ghuqnnsir.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gedczxnuo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gcnisfbba.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gscnyzquz.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/glujvezli.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gfxzvmlis.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gxsdzncwu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gciqommvn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/ggdklkjdq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/grmjadqhr.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gzviaqmwn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gwntuvifg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/gtykanmti.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/giuwlmgvy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gbmufafsf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gkffymrex.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gfwkjyvrs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gvmvtleuh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gdpshymdb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gakvpools.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gsuafgpwo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/ggfgwwexb.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gmphqppwv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gzcbjdiag.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gyxmukona.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gzvjfauwm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gtefnilqc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gwrgexdsw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gtvotzmno.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gnhynirzo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/goirvyugr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwokbvnei.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gmskvtmrp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grnkkiwbs.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/ghrkwdfmc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gupekorma.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gbzhqmeyu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gmppzxduc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gqtcvzgdx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ggyetoxck.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gawkahbnw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gegfvytwl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gkgbmindo.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gtvkzcgvi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gxkfoxlof.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gczsgezxm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxrzpaoar.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/glkzgjech.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/guopgoqzx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gfgtebhyk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gysblzaao.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gpqsmoevb.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gxaypnwdd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gyaefpnmi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gymdqnfgt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gbzlekjoz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gqsubkceb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gtzxmggqq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gfqjcaqwc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gknlktltr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gskxhiqrt.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwoquqpyy.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/grfuuovbn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gnmnkbebw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/ggcxorpvg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gjrwqnjqi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gipltuzkr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/geudloktc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/geuwelexf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gjfshjtpg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsdrtsoza.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gcimjevuz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gzeauffln.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/glegaamzt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gpofoxqhv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/ghiabtynr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gatqqkegp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/ghndbycqo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gbnwtdyyp.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gevjomnih.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gmdtyykam.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gocnnfcoz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gjajwouiu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gyevsvrmx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gdgfilydr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gpsqspkpv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/galblgdhx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gabpfuqzm.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gueuympve.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gjsvpwdqe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gmnmtqkke.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqgsbsesu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gixkglcjb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gqxbiuvei.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gvzgxmlgj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gkckhrzgq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjesooh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/ghndtboxa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gozloobzh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gdvokempr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gifswzxfu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpsoixsws.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/giofyqvya.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gnbarsrsu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/grpfhydsu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ghwjofuix.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gksggzmje.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/genackdlp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzwrupfwt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/goapaqchw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqoiaesyk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnfytdztn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gcimtzldg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gcltwesfb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gcplfmvew.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gyivkrmya.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gsronwcnd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gpajkqebb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gxtiondqa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/grqctnigz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gggnnnyte.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/ghcnhrbwd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gtboyglgx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/garldjzfr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gybkacgxq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/giwhfaihn.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/ghotffnyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gwkmgwuno.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcxyyamlt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwcqpyxky.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gtrwinckp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gqhekfbkr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gqfnwkqui.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/grfnyilhn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gxitguxal.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gqiluuxyj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gbzhvwurj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/garfohkad.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gqzwpkcvm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/grbewosqw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/guujanysv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gmdgfjdgk.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gfxhvlhwx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gxhwskdfv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gjhiwtrdy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gbrkghdia.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/glovecybs.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gonwgafbg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gmwtwuihi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gnnjyzjju.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gnnnexhbq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gukhidajr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/ggypalxep.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gcdcxhezv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/giveqlsdu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gydpcubxv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gtzsnkkbn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gudhffsvj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gprunifyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/grnqvelwm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gnbrqfzxg.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gfepnnjdh.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gbjozdhfj.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjvrfpplg.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqrxaefbh.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gfxdjzbzw.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyeuullqt.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gamnytjuu.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzdgtkaka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gfnyjsvpv.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gbdhgwqlo.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/govksxrkw.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gseayljpi.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gsmngwhqr.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gjyrxgnar.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gqyncrdgg.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gwtodbyct.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/ginlbmfhu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyqvbiomc.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gocjpqylj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghssqgjzd.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gixrexkxt.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/glbhmeolu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmnzoxnzt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbefdvjpe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvfucjodc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyfonispx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gcnddqtif.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gdoatgyor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxgqmhni.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gqkctwkqa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gyiswctfm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gehlpkdyy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjcxiqszj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/glorkkqgc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gpywyeijo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gjuqrckbp.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gjyxynfck.sHtML


<!-- 参考信息 -->