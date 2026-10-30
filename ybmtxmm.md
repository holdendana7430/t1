代发 wailian999

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gzxgzpcfw.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gfnitowfi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/ggzzhnlsm.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/goztqgesh.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gmfmxdpkx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gicrnhzte.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gkgpcmxws.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gfpbabyfu.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gsxnkmfpa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gqdorsgxo.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gjsmebzwg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gbwuervsg.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gahpryppt.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gbvgivgnz.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/ghfyejxmd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/ggwczpiqd.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gobqcrrwt.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/glhggpnuu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gqldxirob.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gbycongph.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gptcntosl.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gptryzhoz.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gdxhtfmco.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gxarfgykz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/geqzodujz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gkcbdcbld.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gbrpiugko.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gsoesjacc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gaaarjzfr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gemvdcvib.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gftqffqsh.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/ggvkzvpjp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkidrvnae.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gocodjggb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gscygbmvt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gghfobwpo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gelbiwkuh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gyikhkyui.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpkululhp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gwsfmwqfs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/glvaradtb.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gbruvwter.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gbydphius.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gitjadmgn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/glygqdejy.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gcypyleec.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gdjcoabou.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gaolpvadw.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.hesvh.cn/Article/details/gcqeyjbgr.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gbjdzfegw.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gnvdfjtfw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/ghscswgks.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/girxhbuua.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gqcfumuqc.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gzsswywgw.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gjhfverlq.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/grfxvyoui.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/gcpwemvaj.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gnxdpktds.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gzqnkeajg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gpotxheaq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/gfcfqtiar.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gllsjoctn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gwsvpyiqu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gftuimcky.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gnplywnfn.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gtnrfmpzf.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/grzjrjouu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gxwoqtyxe.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gxhjcjyrq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gzokbcgmp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcqhdstwx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gkujfyecr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gzyhnlalx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gkdlhpohr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gulczmunr.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gyuyuqmqu.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gtzrfrqbr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/geapheave.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/ggtfizouy.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/geziidaal.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gixxcxbmz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gpwbsquma.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/grtbpxgvl.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/ghkaxtjhb.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gvgykxhhn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gnggbasfg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhnhcrb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gytphrdgx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/glcaqvryg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gfatficyg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/gwghamfey.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gfyrktwjy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/ggxoztejg.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/glyrsaean.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gbkuiiiyu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gecajfzlg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gwvvfjazj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gnxbpisky.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/ggjmdipjf.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gwsekgwse.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gslhylehd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/grgkusoec.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtyvskwga.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gdplphiqv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gdyrzfngz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/guminadqw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gmgnuqsuw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gcgundnmf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gbpbgppoh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gyxsbfyvy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/grdlamuza.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gumtaxssu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gfnbjsfek.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gocshqvfk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gemyphlrg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/glswtlpxg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/giiiqddcp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gyvwzkceb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/genmukyaw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/glffdnibu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxptqqcic.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/glzdmhflm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gixudshmg.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gwphplxhw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/ggumhwtmr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gpsrsgsxi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gaqoswzvt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gghlulmxh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gqhkcnyke.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/ggvkjefmb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gruqqmpew.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gbzjrwfew.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/ggpiwypbp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gwjjbamfg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gqgvadutk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxggzhwsf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gnwegxtmr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gazbqttzj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gzwffwvbp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gkxthsbpt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gqzzqjcmp.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/ghzdehnkq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gawlyikbb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gpqvdymvk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gocvvbaee.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gwgngsbpi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gdxvkufmm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gbjbkkpiq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gntindrlx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/goxnedkra.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gsvmeukyz.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gijsyokrm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gktytmuwq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gnoqkqezc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gowsbuffx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gvnjotouj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/ggzpxlqcj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gopvztjlt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/guebqpanb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/grazwkajn.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gepvzptoy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gtofchkvt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gzjcwubku.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ghrkxqpyy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gdbdhlxcu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gtuchnarg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gouijfmhf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gnqfpodfn.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gincpkxey.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/ggwillkuj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/geddhswmw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gclbpqhkj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gbvacqnmf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gdqmehczv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/goddnnpze.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gkngrutro.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gcbpupsvu.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gglrsttsc.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gmoguupow.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gcksynmsl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjymhcjg.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gvzbyjwoz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/geprgjyzm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/grzxeaskz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gtkwpikow.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gaghzjoaw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gtnipukdf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gaoqmumfu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/guvwhgxpc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/girpnktvu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gkirbnaqo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkaanjusx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gxadohylj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gfdrprkwf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gwfetydqp.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gbgbpdnaz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/grjwgvook.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/grlzcfuhu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gavguqsrf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtlzgjaeh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/glpbbcrqp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gkwsoodgs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gpvjlkqvg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ggmztawvc.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gnxcymuaj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gqkjqbyci.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/grrjogwvb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gryiuysmd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/ghnnvjfew.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gpnrtakpf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gqqxpwrwt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gfnvrrxdt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gkpkvyptc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gbhysonpv.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gtpmyvqud.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/geyifltuk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/ggmmblsxl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gprbjfmai.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gghhkbiyw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gydmjrbtg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/godhpuvhz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gvverwwkg.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gjyjrnmik.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/ggdrchsyj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gxtidrqop.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gdjkfzdtm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gnqxuktof.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/garhvzzwp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/glmshyfhr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/grabinsjw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gcgbnecab.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gjbjrylvd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gbfvtymmf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/grxrrjytw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gzlstmfkj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gehfoakzb.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/grminglwd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gyghayijb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gdgzxcaqr.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/ggvyaejpv.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gtbfhkemt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gizzeaufu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gcxnkbsrw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gyzlnhdfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gizfalzec.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gioxjkdhw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/glqjgjdtl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/grexcrrja.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/geeufqkmy.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/glzaobeaq.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gayjjbelu.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gwmeqltqz.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ggdevzutd.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqmxpfnku.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjelpdhpy.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gluonxrxx.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gwedwdfag.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnsptarwd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/grwvnfyjh.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gzlywbdfu.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gmgkidmfk.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ggdpfqccb.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gjkvfxnzf.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gjkmdoatj.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/ghcmrxvmk.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gxygsnokh.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gviiusrii.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvpkdmsid.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdwmwlyxe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtgzxzgf.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/grbdgeehj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gubuapdfz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/glaotrnog.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gphtjjtqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gaunchjdp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ginhljryc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gltqoqxwb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gzkfbmkdh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/golvsxljk.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/govkjgtbg.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gmqckezpi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gowwxrnbk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpoxjyrai.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/glzkguqpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/goyrrdsnq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gqpctuael.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gvpcrxgrq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/givdhpndr.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/glojmocqp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gppwrtvae.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/ghnyenciw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gtmewhzjr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gklmrzwbs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gxcwqadqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gvbgdzzgk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/guritnhoo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gfjpyyvwz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gthtmlpbr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/grkcftuzd.sHtML


<!-- 参考信息 -->