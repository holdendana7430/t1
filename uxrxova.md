代发 wailian999

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvljdjsir.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gteigfulf.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfmdzmj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzrcozsh.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeegviep.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjowjgyb.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gfeyettef.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejdbovbe.sHtML

[A14] 注释写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgnvjnae.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcypesfe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gegqhkzgs.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gdxtwzwqa.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gruyobmzk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gsibqvflj.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gwguvdkli.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fanxiaobao.xyz/Article/details/gowofmehg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwyfkjnm.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghevrajrw.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gyvwbhnod.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gozvxrkbr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsvmgujp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giokcpnet.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gmnbdevtg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewlmgnzi.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqhczzpz.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfcxhmbi.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztrnsbl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjdxmruk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/ghfsqekvs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gubxuokea.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqseqmtjj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/goszgoivi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjxodxsp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gcnsamqoa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grlqzmpzj.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqoqimyx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gqgkgusyp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsheqbqaq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdzpsemm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrarfwqp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzfcgvfy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdzddor.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqjgjmy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gvmgaygfd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpmuvsl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggonaspur.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbhsxezu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/giubkevok.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqeivhbo.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gndmrzaqt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fanxiaobao.xyz/Article/details/guzovbgwf.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgwshmfk.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/gasmzsqyg.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gixxhddov.sHtML

Py:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gewnbhybe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gduckytgb.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlodjmlp.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/grfritjcf.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gapjvxlri.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopoafap.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlazhvuq.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsibavmcv.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmovkdnfb.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdktsgotf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/gkjegvvep.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gwxztbmwr.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/glmacficv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaenjvuip.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjirclem.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghripmxj.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizvhwmo.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjukwsqma.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkhkzgvyr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/glzmnzols.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpgfzjdh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyxgqalx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtokfffg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdzgvjsc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrtatrbc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifhwngfy.sHtML

[A22] 获取字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzuijqgsb.sHtML

Py:   len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gelitrfgp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbdlqoil.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvpxjexp.sHtML

TS:   s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeprbnen.sHtML

Java: s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgnmydwz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gufnmcsqm.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnhubpef.sHtML

C#:   s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gtghxvrlt.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqbxrqh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgtmrqd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/guvnideau.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwlytfhc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpsviwdw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gotwxtyjn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyojbnhv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/ghaqmbkka.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/geceuvueb.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gasfqeqhx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fanxiaobao.xyz/Article/details/gymkjcqfd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnibdrcf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfimjqsp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfsofruq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvykourl.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwgbuzhk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fanxiaobao.xyz/Article/details/givufzpgp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxulfbew.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbxteoy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fanxiaobao.xyz/Article/details/gxsgwscub.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/goatsumew.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibittdw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjagqkqoz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpngzuyu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkfbtdhh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fanxiaobao.xyz/Article/details/grrpovejg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcfhqphij.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjufwgbm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbyaalyd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnytaabv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fanxiaobao.xyz/Article/details/ghpagztme.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/grnrfctyg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpftwntpq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqglroo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gxmhvyvbx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjhgjevh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknoszeuq.sHtML

B. 流程控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbwkejni.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmawxcyc.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/goivzombq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskkkodix.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzpvfcol.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbvtysiu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/ghsjtydsg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gsmpmkofe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gmblhqvya.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gweukqldm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrlokxm.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fanxiaobao.xyz/Article/details/gcizadgoh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gstdbzfvf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqtbphmc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhuphimb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghddtvxwd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gddwflasm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvnvdjan.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvwqxst.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gwnyzkktv.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzpedqj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fanxiaobao.xyz/Article/details/gdchkuevi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfknutwbm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekuzyoaf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gewdzlitq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzeggxmcs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnkrptzsv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcchtoqc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gjmkohzug.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/glgkjquwv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/giaqytade.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnpftmi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsbdymlf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpamqlul.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/glwxnttkr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvycoxmdf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbrnmzao.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjdzjgyh.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvlimrko.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomidmvc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqtcimxp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/grkffcsqj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiutiqhh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gobbogicr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gthgtzayd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzmgsgi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gebantemd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzrscywn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakgxtan.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grelhxuxp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvcolzao.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgyjpyq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gifkqunhs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggapkvjaj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvayqxois.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofcdbcqk.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/gulhsbdfl.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gsauusvii.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdojwgjgv.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqtdqhp.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyoydqpy.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gokbwokkz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeheadye.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbmelso.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvxrvlac.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqkwxdvd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcbkmjrn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynikczmh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gavcucdoa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gaocwmulz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/grkmlbtej.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gufhaccti.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gkbplhhqe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/goyupbriv.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdglqlp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gumhekmcr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytjzewlm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gektzaxok.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjlmiivf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gidzeinzc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvapcitrt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/goutyarko.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqadjormg.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjcafsgr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrblctsx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/geyngvgfo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/guzfnricu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gzigodjul.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpsqoncg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gisepbsoh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexsiexnk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmshkmaz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppemdfih.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fanxiaobao.xyz/Article/details/gmixqdmzc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvihngloh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ggsrqovye.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvcrwqon.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/guktrnzwq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gsfereyps.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtbmpnq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gelbyqagd.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbolzods.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gzayidiei.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/givduhstw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncouxxdn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gouxmjlyh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjmbfjmj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giktcttvk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcbexmrq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gkepkbmup.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvrahxzwj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgttnprb.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmtqxyaw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtlqaixg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfonneuf.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gydiauvqn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gpgorqgns.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjamqsaxq.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqcrqran.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbhcitww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjtnmhbc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftuulsrd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfmxwex.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gznxpiqde.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwmgylgn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgpngykj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gagxqxyby.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqcmtxit.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrmnikss.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarfaebl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gguuqeneo.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpolkoafq.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgeiikn.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbmwctss.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gudxdnusa.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gmkqkuftd.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsseakwt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbtlvfyy.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/grrfpwitk.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbojirt.sHtML

JS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqfzephl.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmphhmese.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxfrpoas.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gjiijvhjt.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhfrnaxk.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/guazmutml.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geuddhtiz.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjoteima.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkaxnwms.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqaddecc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gfetepkiw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpwgodwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaimviqrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwkpcbl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllxjmtou.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmlrqzotv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/giuwzkeon.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgjvcyt.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsccljunx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsqkmaov.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxbtbstb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeqzrawx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfolzklp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gxpiaalah.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqukoyfmy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqkrfbon.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuuphvua.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbywnfpmn.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gkqzjpjlb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghycmrjmp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrditgnd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gedgfbabk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjnpzra.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacbujfpg.sHtML


<!-- 参考信息 -->