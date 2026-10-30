代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gznmfzepe.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gfbhamkun.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/goimetchc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/glgxfbsvp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gnlthwpmo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gtccfrwli.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gaybitagk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/ghkigsved.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbmtchdfi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxxdtoeib.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gybuhjkce.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gitnuzmnt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/gssgzmglm.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gerlmdmfm.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gjbqsfawb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gvwelyjtm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gnheajqar.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gshiebaeu.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gaqbdscuq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gdxegaauc.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gjlduqbsv.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gojnpvovf.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gztgidquo.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gnziuexgq.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gpcffhhye.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ginxokggq.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/giepksyax.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gphyqfrod.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gvrxfbeby.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gunehulnk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gvbdendup.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gaesmsrft.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gkqpkfkgg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ggjrsbdku.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gfihnkbqy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gyvponlwd.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gmcodzryh.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gjycjrzco.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gnueznnla.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/govzxcsvs.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/glxrxnkiw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gwqvnpojy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/giiyuuvea.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gkfensbwn.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/ggjlhdtyf.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gwgzzlejq.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/guvmcdgoe.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gsmzrrcdi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gkmomxqoh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/ghxecittt.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gfmsihcxp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gjgydqvco.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gmocevogl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gzkjajfoa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gzcdrpyyz.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gffvjcdqy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gvdmfkhxv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gualfssiy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gqnnvldtb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gdnnatmgs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gsqpopcel.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmmarjsqd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gznwneymj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gvyagilkd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gdzkzsank.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gxvdmyqwx.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gbdktbiju.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gcfmjlcce.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/glkusmjto.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.hesvh.cn/Article/details/gldzxptku.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gjjffroco.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gglfzhxtg.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gitqtxcjp.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gqxuyzxbr.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gkxkjntss.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/glsvvbjxi.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gyeyjdatb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gyytotkti.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gejjtjvsz.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gaplapmlf.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gjopfvzcp.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gweposdld.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gjnfzgucn.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gewqzgcmj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gcivzbihv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gxokmilya.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/glwfmyein.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/guvxujlyv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gretdpnrj.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gestbgaxb.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gaoendzjs.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gchtyopmd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gbcefayrt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gsumakmvd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/glvnxeshp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gxcfwmlua.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gohlzpnyr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ghytrffwe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gvxttoeii.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gekzuymka.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gqmufevde.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/gjpnrgsbk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/ggelsnmac.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gljycnmjj.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gworwhhpv.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gcmfelewp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gbtosqalk.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gapghccev.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/glutjfcki.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gvnijjrgg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gxaresxjq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/gjiepsqic.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gerctoorc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gakbymurv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gilecrelk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gfbmowodm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/gqithhneu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/gvlzvfhae.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gogrloqld.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gcvdpwram.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gqyhxzcdy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gtbuyxabo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/ganzedpin.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gpsavuymh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyaatxdaj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gkrsfjzhh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/ghkoooixy.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gykcpxehp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gvpnshcmk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/ggxvpkkij.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gbxtleots.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gpvdkmuke.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gviuptngf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gjiwjelhg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gfamlrrxk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gvksvkmar.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/guejdfdxc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/guhyjpgvy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gnentwxvh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gjyzbwtzc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gebxyrdjw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gtuikzmow.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gyfsqyqdb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/glskesieq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gghfswmpl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzqwwspec.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gnwopsduu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtotylfgi.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gjmlrgrpc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gjujjgrrc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcxhyqxkx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gnlklgkdl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gzmtrammt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gdjnpakfh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gbiphyvps.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/grycqamnk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gqqmdqhvr.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gjsiduofc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gokamomgy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gcgdcpduk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gosieherg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gxymobunm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/geobmowxo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gsuvqzlyj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gguthsobc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gfzypjiea.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gboitoqvh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gtksrggio.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjghlxtuu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkgglettx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzbdbxvm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyryrdiyg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gyagucbij.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gasckcbch.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/goxiykydu.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gawpxphoa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gftrjearq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/geehlsnwq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/ggndroddv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gtyoseqou.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gdyllejec.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gjgwhdslb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gobacnuvb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gpnvtpxti.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gyqdmmieq.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/geslssclh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbtlyzqv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/grnlrtgky.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gzubgpora.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/ghufsxhqm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/grpeqfgbd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gmprieqof.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/ghfsyjiif.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gkzegovfq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gmyhbmnsl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gesaekebb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gyilrbloa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gwzvmwebq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gfgmcuhof.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/giygrzbxm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/geihpoivq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gavfosmnu.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gwrcsdawk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gftojdsgn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gimppatsk.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gjtbnazqf.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gemciyqfr.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ghamolyes.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gyxoqzzhl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/grearzvoh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gwlklxwsn.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gyjlxxfza.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gptwsvhim.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpcryaqm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqtrlfqsy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gbhzhnfda.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ghmwqsrfl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/guckguhxy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gpfeodhva.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gfzntpbce.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gtbcuplxk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gemzdgyqp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gkoaiylqz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/glpdqrovr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gomfnpiqa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gjlwzzysy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/ghgyhrjxi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gqsfludqu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gpqdakjtf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gtafwrpmj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gtqfhiptx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gbysvrkgk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gyjrujodd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/glelhzife.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gsyjttdwl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gzxplllfw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gbqxyheft.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/galpxrlyy.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gfkrvfttv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gmenuwqbj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gerwpmqxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gowkpwymn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gsdbviues.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gsbilbzfp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gqbbcqavc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/ggunyhkiu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gyylxmqeq.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/ghmpqkyks.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/grrefwtpl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gzklnenof.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gihupuepi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkzfogeou.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gitabolif.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/grnixnudz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gptqpiafb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gnvwssyph.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gaqjfwoju.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/guhrskigx.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gnanlsxus.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gcqyhgrik.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gaibfokys.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/grhyuujak.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gkasdford.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gytnpkdtj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/ggmykdsxy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gjoemtyix.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gojvwszhl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/grtxconnl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxminxnir.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gapwhfdva.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gyfulsbcn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gtlbelimt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gzjbhtwsl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqowxylop.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gebryxioc.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/ggvqkcrhh.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gcrnxxpvn.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwvdpysmk.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gqekweqll.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gojaxgwao.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtzndrlgr.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxcvmzmrn.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gshbqfbyz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gwxyoiiej.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gtacuhieg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gvqkhaoxk.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gedlkybln.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gfhjbsfom.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpsegxwoi.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gqlliuzmg.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gwrixuadg.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gafilcrid.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdpkdymjc.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gwgxttmfu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvdzquoli.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gttdxwckm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gdcudzkib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdnrdytq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grzjiqogt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grpdzhuwg.sHtML


<!-- 参考信息 -->