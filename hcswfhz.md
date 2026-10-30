代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gdkrlpsxy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxesveuwf.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gqlcrlpoy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzfwuru.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gzpwthogc.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gxmlqnhmr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gplgucpky.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/gchohngvu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gowaznafm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gcawqdaaw.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gkhyecubj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/grkdmhawx.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gcvfhhdix.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gyfqstzzd.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grgbvqybc.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gqmomzdsm.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdjhqvxac.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gcmnhrjxz.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gavdjhhvc.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gwteubsue.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gczutsuay.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/ggmgoglcu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gzbbnqbpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gypiwucbo.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gbalcuxfq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gbmhblfeg.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gbaitrwyl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/ghspjbndq.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gmnmkzzhr.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/ghauatvna.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gztnssrkl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gupcrpfyx.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gnkphtucw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gkkrarirk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/grtbscnzx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gsxjpxkrk.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gzeiybhlb.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gtcxpykvl.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gwwzfmjjl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gmsbkdweq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gdvpemnqk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/ghrmdhucg.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gelcexrxw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcrefjqlf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gxfhqidar.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gqrjmxzbc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/givrfmrbx.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gdbqixqie.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gaworwhcn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gwfoimxwu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/geampbfav.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/guiaxhgtj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/goxzajdnq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gjkgerswr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gxttbwtrm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gbqrnfoie.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gxnmboads.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gdoarkrep.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/ganydygwz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gzznlkmsg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gvpiagyza.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gsjwwivoe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/ghwgrmzvp.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/ghigazjrj.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gbdcwvltw.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/gvaznztrk.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gzdfcjdab.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.hesvh.cn/Article/details/gwhheiqnj.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gasusqgxn.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gnzfojidg.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/godkmonfe.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqknlkw.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gqhuvxbqg.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/gakooejtj.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/ggwwronoo.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gdfhbqpgz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gltnqasfv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/gvetxgdoh.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gladwzurl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gjejfegke.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gcrlxtbcl.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gasjxcias.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/ghjjlnmlm.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gbditsdwk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/gwzckzcdr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/grjjuagwi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gjttkivvg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gvpgjdsck.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gashpqytp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/grfwwpdcs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gvkbbtzjn.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gvvrhzdot.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gaiyzsqea.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/guikmbgip.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gwusjzbin.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gvnnsaujt.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/giilcpzig.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gblhwtxvr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxdymqyft.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gblspwsrj.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/ggltpfuzq.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gimqlgwvz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gzctgfnsh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gnyadccob.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/ghqbskmnp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gfbnavbkc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gdungenck.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/ginkaustg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gzjdxuzlh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gbvqmdxjb.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/geysdmfmw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/guuqmzokp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/gschsskih.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gqohpoosf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gtkftoyon.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gynpiyznu.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/gkscprnmt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gnxuamvvc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/ghhwshpwh.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gmzpqbvfq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gxnntjfak.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gkvduytmp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gdbkaaxta.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gqkgooqvk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gtqxesomb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gymucfycl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gnseuiboo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gzfszuepn.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gfppepyuv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gjtkdjybe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gawsnvktk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gsseisfgf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gtazvaers.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gskzcekxr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gxgpxfrfj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gvjwbbfoz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gvwvymifb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyqtstrdi.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gqrmvmgiy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnbtzaueq.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gbtgcettx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gzbuzeuca.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gvcjxtbnk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gximqbhqt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/goylocqwi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/goeaumkdv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gfamkfffn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gaahokhkk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gjmycecrr.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/grrsacjyf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gmhqrczmq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdcmotbpc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/ghhpeosdd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/ggtssgzuj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gdaogxbsy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gnlmiesfn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gmmmgidtl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gjnqnppji.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gmfdttvma.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/gxwdythiu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/ggfjijisn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gylxjieba.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gnfcmeenf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gulmneyaq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gwlhsycbd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gyzlcsisc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gxjhjrfee.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gtpdrufte.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gqqhehzwd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gzmjmztxw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gjqfmwpnn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gqfvzbeef.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/ggydbmtqg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gahdgxkvt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/goqoatqis.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gymqfxjhz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gmrqwpulj.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gpbrzthhx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gkeslyhao.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gzrbffdpz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gjdprcffw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/garptqrob.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gufgvdxbq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gtorgulsp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gtjexfcgz.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gplrxlaas.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gykgbpkdq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gnqpvpuzy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdklixku.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/ggrssjhdw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gdyyhfivh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/ghtalcicp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gqxucifge.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gjnikpojw.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gfqwlcwro.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gyxxhivws.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/glnjvtbnb.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/grdmdqqqp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/goyuifdqz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gqclbgvsk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gamwffsny.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/ggvcpeurd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gtwvxoenz.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gazfmvtuu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gvuyyvuie.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gtumpodzd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gswtbnpko.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gqwjnumck.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gnhysbvcz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gbjeqjlqm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/ghjmtowdt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/glhzgfcum.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gdplcdecs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gfcoqgzai.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gqmbfdfbu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gmqpknfyi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gusuarcmt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gunhdzvfi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gytnijjei.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gyhylghgg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gibdoxhmx.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gcqmidefo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/glqxdijeg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gusvucofc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/grvayeokz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/glpkdokqb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gxduqscse.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gsfqcqyeq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzymqbne.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/ggelrxnse.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gsopwnzvg.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gmazpevba.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gxsnnmncs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzagndjsw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/glqbxauzm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gcsnjahyd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gmijkkeyw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gehyabcrv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gwbtrxlcp.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/ggjzisbyr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/ggysacdna.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gjljjmdac.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gwzjcqfsm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gihjfrsxh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gstnpwjhp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/giccrzhhl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gthvcojqf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gfbbjxvik.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gcgymtwqa.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gmbhopewn.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gzhtfebmv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gaxydpkkb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/ghdnhtxtp.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/glbnslzyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gikcivkxs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/guimxsfju.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/ganqnltmu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gaejqrdxw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/ggeufxenx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gntppeptv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqffpftwu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbfqguvhv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gitcaiaou.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gjawrmpdx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gcsnzjtgn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtagplpol.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gxhodrvng.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfwumjr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gnajzmorw.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gzdxetqko.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpmdvljjh.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghnpobbsg.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxjmtdfqz.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gbxmxaqyy.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxvxzrcns.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gjtfootdl.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/ghrvwqkek.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gvgjikomk.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gyogsqcgh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gesuvuqmm.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gkslajrmi.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gptmydmcq.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gcnzzewiu.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gbhbbahid.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grntflyvx.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gqgejqflc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfghkrusd.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gcbvlfeta.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/ggsmwexse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/guuirwcbp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfacavkfl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gqrrrrppi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gptlgtxmh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/guheshfsq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gbiawmxbe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gnhrzjmhl.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gittdyjsv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gfbxmwtug.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gedwauxwo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gywwrqztn.sHtML


<!-- 参考信息 -->