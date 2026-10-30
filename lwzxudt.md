代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gtanwlnbt.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gajayfyzk.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gbhexrbwp.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/garihcoog.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gcoauseyz.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gtonnjwxk.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/golhpcbhy.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gesclmcud.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gmbnwmsak.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gmfziismg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gkljfcvwf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gxjahuuit.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gkqgocdal.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gstrjgkrf.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gwhzfnqwc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gsfbsvlev.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/guidfwped.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/glckhbuha.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gqkclwgwm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/ghepkigvq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gbfwjqioi.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gefcbkrsu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gxjtgwlve.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gftavuwsl.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gntvksabo.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gbwpdeego.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gtrfkupvz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/goiquktxy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gvjdozspq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gpppnljzy.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/ghprkjlfy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gxphgttxl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gxxdhtqql.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gamlfbppb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/ggspnrohj.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gxfhsxpkx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gozggwmli.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/glggnkcnp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwkgtmiod.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/ginuroogx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gnndfemya.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gaokxdxmd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gpezduevt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gtjkrxani.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/ggmlidhos.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gbnekziyk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gaftsdxwj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gplwtfsxp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gbzftuwti.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gjvdobrob.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/giyxeduym.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gvyguodnx.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gvmooxldx.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/ghnvvkupv.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gzewzsthv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/gfzsbtpob.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gflylerbi.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/ghjphdlsb.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gzuywvaqr.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gohspfyyw.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gdxivekqt.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gllzxbojn.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gkggtdsex.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gyajowovx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gzmjwvzxi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/gcdskhbwl.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gycogcrsj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gtfmuzhfa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/gqwlllhae.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gvvfebzoq.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gpvafjdrf.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/gdzxwrmbt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gnnvnjxvn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gngmlbeau.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gnjicpepz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gskipnljg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gnnjhslml.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/ggefuqtfo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/grwhkrryg.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/gsgkeiqio.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gftzxikgx.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/gxlupliou.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gqunebukn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gutlmenhh.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gsnwgzbjm.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/ghmteujut.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gojzlzszx.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/gzehldeyb.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gjgvwhnuk.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gezrxcpov.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gidmwrwdt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/geamlxqld.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gmfnedapm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gggvqbspg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gzenrbrgd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gphslykkt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gcxykvyum.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gohzvkadc.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gixsnxpbl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gusuccypn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gaicmrdve.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gmokdybtz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gsidddyfw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gciccfyhq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gjbqcfzhh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gzrssvema.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/gwoqcvslk.sHtML

[A25] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/grzcehsuv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gucyjcryi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gfuipldlm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/ggfxgodbg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gjvqldkgo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gcdgetbua.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gaeeeaubz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gnvkqkhrf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gxhhqtiks.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/glegzermq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gxhikvyxd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gfdqnjxfo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gwuazcvtt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gqlmoxoqi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gjnmffwlb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/groesmhve.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/ganfopnws.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gljcyvcza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gserltvrc.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/gozllgujn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwpyvxfrw.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/glkbqgspz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gqjnigiit.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gstonbsix.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gjjvvuvdn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gtwhdewlg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/golboynrb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gtrfyxqlm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gbwyjtgkk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gaddgvkve.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gsznieiue.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/ggjzdoahk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gcbbwhmhc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gkjnbapqb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gwyawmvmp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gjjwhmwwt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gbfmjvudh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gdhoyanig.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/grcyvnrcg.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/geqruufjm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gkwvkfysa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gpeoiymvz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gtodxojxa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkttypaug.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gsjdpptmr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gsoylguyt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gdvnjaqhg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gyrvhdixj.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/glqmasman.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gsqxtxdya.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gwarfohxr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gnvxtbmzg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gypcsoozn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gvyvelsht.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/guylawkjv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gzipwspmg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gwhtiqbkd.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gtdccmkfy.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/ggbxosecb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gecgewppl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grxiqfrqv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gbumryzib.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gmxndnbbv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gdpssxwls.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gpaslicjd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/ggaeixmif.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gdwyiwmzw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/grrewtlzu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gzqjtqltu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gzslhseod.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gyhtarvch.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gcygbdvad.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gzeoolsif.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/glcehnucf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gjcxddiie.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gazsdwanm.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gyhzwufnl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/ggveeqqst.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggcdtliwh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gpxlgbesg.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/grwbdkgxj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gvmfkwwxx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/govmhtktm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwnjlsy.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gidhhyhgj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gdtycwhbm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gchppuwwh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gpccpehva.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gcuanftlf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gencechsm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/grthxazbf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gbyzsasiu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gytpamtcw.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gsozcibkh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gaywedlbp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghxootlqn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdjjmfqo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gnxccynic.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gqyigcarq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gzyhxmrrq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gbdwpkphp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gclgpcbjn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gqdcaajvh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/ggofflszp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpglzuzwp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gmvbjbexz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gqubzgole.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gpnrfwahu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/ggeypgacb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gkidwoimw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gawfouyio.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/goiwtignm.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/ghzoxvzoq.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/graygfrxs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gdlfiwdvj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqlsopgml.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjlafahhd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gltdgetyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gdpwuoejn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gnqcagyhf.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gdlqmxpxq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/ggdmenphz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gijnyapzv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gvkudyguu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfskiyhrh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmwkamcsj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gigcggbex.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gmztrfavg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gktpdjuok.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gtpyjshkh.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/glolhbzrv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gxsxobqtt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/ghavbreaf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gucattsex.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gaspigaxu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gqqeaoovn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gvwqezpzp.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gejkczkrk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gnnuhiozx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gqptznwzb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gvydgtenv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcglpxydz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkrcxzyod.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gnvskfjdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gydzxhwuo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gulqxyecp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggsuhwhxb.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gubugvvon.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/ggliwsytx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gswwbwwky.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjsbhjtmg.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gkfpaaljn.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/grfmzzlny.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjszrbuah.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guhkyskre.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gephegwqn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/geuiapplp.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gqspllcyv.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gxcrlztfk.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gwyfwrryb.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gzshypboo.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gaqvkqirh.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/glyoslgqt.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/ginazovkc.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gklwcrgqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqrfndjcp.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gqostwpat.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gitnqmqpz.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gpiboyjul.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/ghypwwfsi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gshqcnibm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpdkasyew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggbjaxemt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gaqyxkfho.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gcgiplqjg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gwpqbvetu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfkfaebbj.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvtrffsnf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gppgqphpm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gwgvbcamy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gubnnxmoc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/grgcapcrb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/goqbfbnbj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gvnxrijlc.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gffzecguy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gyzfrezfp.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gbejkeoco.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gvtzabwor.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gffscyfqw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gaemamtdc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gpdxdnkaj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gneyuyiqx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gbfutuiwj.sHtML


<!-- 参考信息 -->