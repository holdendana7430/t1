代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gqarwplsc.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gmvzlocgy.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gtowemdud.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gltidvxky.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gqqqjecli.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gifnpicbx.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gcbifjdot.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gmlxgbgdm.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/ggpjbfmpm.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gmmnfjhoe.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gynhtyazm.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gkkzygtto.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gffkxznfu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnxhpad.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gatsmxrky.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gafegiqqn.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/glciheusu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/ghlivqxpe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gewyfwiyz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/grmyqjxuu.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gstanhfve.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gibdyrnlh.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gsmxmtrde.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gocqsgmgy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gotpxtbrx.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gtbmnecrb.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gzroqtizg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gjdvzwrwp.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/grpbeslpf.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gcwfvnwgj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gzzlajfep.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gybngtmwb.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdoayws.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/glsxivcwp.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/givaygati.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gvdxgmhxi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gkdzdhqbm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gtbleihzp.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gqcuedzwv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gfqoayjrs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gxwqavkgr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gilnbcljo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gelhalpjp.sHtML

[A17] 位运算
来源：http://read.share.fehbvm.com/Article/details/gsalhdwju.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gkiiyflsh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/ggbekhtyn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/ggxjzyiap.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gagyuqaox.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gtxiwrvyy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gevbfjjzj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gzeyhjhlj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gdkkdtvlg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gjvuyamoz.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/guaqatpoq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gfphhokxh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwifccym.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gbzivwngh.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gkrmszrrj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gsjnzdbls.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gshkebxlp.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gjcgmqvyb.sHtML

[A19] 交换两个变量
来源：http://blog.fehbvm.com/Article/details/gffmexhrh.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gdynblevi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/guxjtyuks.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gfafijiks.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/giygipkch.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gnqdbdqws.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gwqfsenic.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gcxbhgeyi.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/geqcgstae.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gejgaqhss.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gkssbemlv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gdkjwracs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/gqzsqyknp.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gtflkqgsg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gvsbzvsyc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gtgabyeoe.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gpitlhmvj.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gcmasutke.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gfanpnzks.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gmokdfeth.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gkqzgdwha.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gaxufgnsa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gpehcvnhg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gyrdsceqq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gbfvspbpg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gvwvqjyvl.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gfakvfzug.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdcwcdccw.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/glpsqrkvy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/guedotxtm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gqexslnzt.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnwptldou.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gkjwsusux.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gygjokxxk.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkszbpuax.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvxszhxsc.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ghcahxdfw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gqsxvtfsj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.hesvh.cn/Article/details/gvlzhxzrc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gfixfwump.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gawqcqicy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gmxtxqmqn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjhairim.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gizjgwwuh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gcrbmfhxk.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gkfpybiyz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/glmmuiovf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmyqbqq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gjpzcqlzv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gpribkeab.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gnlmhntsy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxefnepae.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gpmmbowra.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gnvxlvges.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gmixiptjh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gjpefsfcx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gwhwyfzve.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gboydeipx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gqzuflfit.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/glasuxgpo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gzdfbitmq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/grktuujzm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gqvyrcaxu.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gzxlmxogq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gicptbgpc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gxwnewobz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gdjyoqnii.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/geabqxtbq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gajzxfyhm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gvpzpydmp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gggqhlshg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gcgscyvbl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnhnekft.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gaibsxjea.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfwiakmxh.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gwswxosjx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/ghdxountc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gbqtgivyw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gbqgjcatr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkzbyeq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/grrkouldw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gsllqkdkx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/ggjwicviy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gtqndrmtx.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gjqyddqcp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gusgjprov.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gwjkghabo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gvgwewrko.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gizipfmoc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gsfmcexku.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/giaiwwmus.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gibdfoqkw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/grfhxyrey.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gvppasvow.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gocakrzuu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/guondqkyp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gfimpibfr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goljiqoub.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gybzoyyqt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gueeimsxj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gjvzqxfup.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gvjkzrxus.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gysstfphy.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gneevoyxf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gckvwxtgl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gtsuamotz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gevkmslvs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gauyxypkk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gechmxjoj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/gtkjrjchd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gucdiwibz.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gbfrpdnyo.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gvzypxyct.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gzemjqvcm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/glunyepou.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gwvtuafrm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/ggydvmawh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gvfmhrfbi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gklteikcr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gzsknhwat.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gwfjfoyik.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gnmwxastq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbeltbsx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gishnuvfi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gdxsusqlt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gbiyylnpn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gcrxsyspb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gsounymqt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gfhjepziq.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/guopspgqu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gbrbghesa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gwembzeut.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gyvnczqma.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gbkujsxvw.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gzzqmvvfz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gemfkjrgx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gcibhextr.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ggtujmqfg.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gfyxjgaal.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gfnyexoyk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwlgpzoak.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvnlhbciu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gegxkngpv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvghpqetw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gytglhaxn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gbbrqzcdu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gaygkqnco.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gcvvlcnaw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gvvwzflxf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guyfrarce.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/guxegzvje.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnfyqfxsj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gbhiniwsn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gahubhdzw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/guzjcubco.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/grilppvhy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gxxnhjlqz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gqqoetokx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gnvjzihqw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gdsybvryw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gtyapomzi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gjpjmnuye.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/geotlndhp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gneqffycc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gbufuhaxs.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gqdqjvvzb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/glicbuzgs.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/ghwkdnplw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gycurcfrn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/ggnfjjsvt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gjvgtqino.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gqrmaodlk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/goxlldaiw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gntpdbjey.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gakqyzqrj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gnkyjdwix.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/glxkmrwrr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gmffigqrv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjbjvqfpt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gqflmqbgv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gqguojqes.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/guifbkasg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gzcynedfe.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gzitmsvas.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gadotiyub.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gsmsbwmek.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqzayoayu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gkrbfedzw.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gpbajpidx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/guhublvuz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gfctqydct.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gbcjkgmje.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gvbbgpbdb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gpbpgsmxp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gfjtlchha.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfbaqgarb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghaoubryd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/giitmpjdv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gkhvfytrq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glddjvebw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/goizdmxal.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gprxjylpg.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gpwnrsyua.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gjsengoed.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gcloobkxt.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gglvfcypw.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/growhximj.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/guuvdmjqo.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gvgyokzza.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdqrnscnv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gzkquwcvu.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gdofonkly.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/glmnluvfv.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gsgrmgmez.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gtvmgmgkf.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gdmkmmpob.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gluupcpxl.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gnvvstfdp.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gshxmnpvz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfyfjtujt.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gazxdlwea.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqulqwjc.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gvideuqaf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gkqueqjsp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceponrtx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkjeqsbip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gdduytfcm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghsuippgd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gbygeiiaw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/ggmbxspnn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gduujlipe.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gtbiqvzch.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gnjddabep.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gwttkiibk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ggmkixkof.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/grpctmeuw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gdopvlcqv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gbuzfunab.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gmlntjvni.sHtML


<!-- 参考信息 -->