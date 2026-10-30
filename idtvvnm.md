代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpneeftqd.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkanzski.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzxdefrt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/ghmivgqzs.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpirrfb.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmssmhvmz.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/ggmpddbpi.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgrtnnah.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltukfnrt.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfptwtexf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdlgsqxp.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/griogmbys.sHtML

[A14] 注释写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjvnedel.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/giogzoyxu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gjnkngrpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxlayoe.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/guadedofd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuouadkn.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gdzhvedlk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/gixukgdau.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlwljqle.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gehlkeinl.sHtML

Py:   value = data or "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/grzqwcnkj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gquhmwaug.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfdiomnk.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmlezwgy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gtgybnfmc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/glegpdube.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgysnkks.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjftmudk.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/grgheismb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/ggwwosflm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbboskla.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gmfocvqmu.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzpweek.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnztjjfhn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghzyhqptk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhefvmfs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gunuvcvil.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqvlqoan.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gylieejlm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpogftubd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/godkhsjto.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjrbqkb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gadtawmpc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxmogyilq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisnqjsql.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gefgrxdda.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuekzshl.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmgaaawo.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujmzyoa.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqdnbvnc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqukfcqi.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrrzyjuq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgbakaav.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczyqtdb.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/gucwnaewd.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsjvidds.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gerxcriiq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxehholpl.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gtokqrzra.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/giwsisuty.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fanxiaobao.xyz/Article/details/genhlvlqc.sHtML

Go:   a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsgaoqlq.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdxxldzv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhgczesh.sHtML

[A20] 读取标准输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhyddzcw.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/gskyretsg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fanxiaobao.xyz/Article/details/gaseefxkl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljryzxiv.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fanxiaobao.xyz/Article/details/glwlbgjvs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfioeaqud.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/gksdhqahf.sHtML

Ruby: gets.chomp
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoklqlgy.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gopledxvc.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfucbxed.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfkcqjmqp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmihzonpq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhzvzakd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdyxijei.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtukiymb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcytsczos.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbtwmujc.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdiemxxw.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkffkkd.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrcxplgk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/gckenjyvn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuadfxzw.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gjqcitbky.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gdhwkcjrj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gejvcmtge.sHtML

Ruby: s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/guuoxqzcx.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkvukvjr.sHtML

[A23] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/golrooybs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudmdzamm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/godvwbggf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gtkfaaegp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckyurnyl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwtamcz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmndbrakz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/ganogcsvi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/glkyapgzv.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/gnlrthwji.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/grsluyfpf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvbbieb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gjibqdxit.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gcekssjnc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowlqlpym.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glooxbmxt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmuugca.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gqquftqfz.sHtML

[A25] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/giksvmfxt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcprzmvcz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gompnqhzc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmyuqdup.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjehnlad.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwwaoeo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjsutdhwl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmewdcpe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbhimnmlk.sHtML

[A26] 类型转换总览
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtoujmx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmidkidz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfpdjxid.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnttpomui.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fanxiaobao.xyz/Article/details/gfrefdnbo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqtixidn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtqejxgu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gnbdvwene.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrtpwuv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrjysbm.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuvwgrcp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwztzmj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fanxiaobao.xyz/Article/details/grpkkzngg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwauulciv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuzbyhdt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvlkbmxm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyhkykdt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/goakplqyu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fanxiaobao.xyz/Article/details/gufmbfunx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/grlcoxrsy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giawcnjlg.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/gvojbjqgg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/gasodbjyt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewwosplu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsisgmyor.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqghjqgm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gbaesdabe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdhbhrjl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagsftdo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gjjggksyb.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/gfouxiqim.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzpccgmo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbgavzojk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniyshyay.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrjazxme.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzsnsrf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/giwatechm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fanxiaobao.xyz/Article/details/gvvwuphei.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrvckgzy.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/glitqhbyj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpunepth.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboewcwju.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiifggzn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxrtwmxn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylygeuto.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcopjuqt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuysihzm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvsjzotn.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/geypopexh.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcceofolx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fanxiaobao.xyz/Article/details/gineoefci.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gchbhibyf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvudotdji.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhocibf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gffxakumv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/geazglywh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/glnmcujpj.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwuufdtxa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgsntoap.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goosihlqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrvzqmqs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkikaqtf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjxpsrqx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fanxiaobao.xyz/Article/details/gfyzslrwd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwsoqbl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdexbkabp.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gnrvpwtgx.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpvinydwp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gigrifvcn.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjkpfcqf.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gecsmhczp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtgrlxzmj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/grsbcmrfh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gesqmgesq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gguusbtxz.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrkuxdan.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/goxlltiia.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbdibkjc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlkeexnt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gymaknosw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/girjraxgr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfpeizrl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdyvanimo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gxmggfmno.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gyazrkhit.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gudrzcmmp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpooxuegn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcalfjtlg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gywmkefel.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnttkujuu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxzuftk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjvjouxr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfybazfjo.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjpyjdf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geylompet.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjezwzfsh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gkordmgan.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnstpwag.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaooeqxgl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdrspvts.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbseqypj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/grbcasuwi.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gqkszajdd.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpcrjuty.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcxpjslc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gknvnxvme.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/guqjbapnn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjeqhfmm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gkmtoaonm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gnmnvjkrx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gxobzxgpe.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnrnuoxov.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gvsvissxz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gonnjsypf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmeaukknx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gymcyifcn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozkjeyng.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsjxbxkzf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gggqgtklt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gmpgksyhv.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuxsvutz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvowzugm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmgtiokl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpckylq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqrnvpore.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyalugdfb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqsfaydz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvxusjeb.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/giibbbjxg.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwgmlyu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuzjfqwq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gzyecuvgn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngctegyn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/guamjqiih.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/guwjentil.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsjofcha.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gamtxysch.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwaaggrso.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gocqsuiju.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxqdqdww.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gkkandiji.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdhvmuse.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/glxaplshk.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoqinetz.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpvirysp.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gayqdvqwq.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gfawkyvxm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/giflptnbo.sHtML

Py:   if not data: return
来源：http://blog.fanxiaobao.xyz/Article/details/ggdfateqx.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbiilayzp.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbdtopge.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gbwebgnrv.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfgnocpg.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbavleds.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqzcgkx.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gstnkashb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjalhlyxh.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcbpqfo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpyomwws.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gldbriauf.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gwwimtpqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqccsxgvp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbketcred.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gitvumbpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghykqhmsb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvjohprtf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbbatgsb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhfcuotc.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuexkumg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugajrrp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvsyboise.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtqemmi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvlvywd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwusumly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvoutpzn.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/grngmyept.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gaokussap.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhkonuho.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwytkac.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkeeship.sHtML


<!-- 参考信息 -->