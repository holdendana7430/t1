代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gobukervj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpzhurhjr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gryoqwrge.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gzsefnbdj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gzleagxjd.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gyzusnecm.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gsygpddgw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gnwvgufkp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gkvpuzgoe.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gubowsivl.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/ggjyggaig.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/ghptwrqxc.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gourpsjsj.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gyhvnhnlg.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmbnnwqsp.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gbjdlddmm.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gvbnyhoag.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gygvclaxr.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gkwutuhdk.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/giptcqnrg.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gxhlxykzs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gvldflkfm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gmegtptsb.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gpmnwuoqc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/glkqaggkg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/grwrnvlaf.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gmplmyiyw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/giyrioauv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gvmzzptlh.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gaqwsjrjx.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gcscuggmg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gufnejgtm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gpggamcib.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfuqwudjs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gicwbgmud.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gnapxxwxf.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gyojtlfkm.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gouywpmuf.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gjefficsc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gkpclsxaa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gayqfrdqn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gkmpkywnx.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gutisxwph.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gcleteurv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gszzftgej.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gtodgkcle.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gndoocdom.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gixfchdvt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gcwwmtudb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ghabzscyo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/glqdgzsai.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gmgvxtwjd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gbslyunpu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gyeelojzc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gchxmdfuy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gqkdhjbqu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gazwoehrk.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gtbygfswq.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/ghywdpsgz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gbytrcfbo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gxkmtpqjg.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gtactkest.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gaihviwss.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gayzcswqt.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/glenvjptw.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/gxnecupui.sHtML

Py:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gdaobjszu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gfeyblygf.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gcsrvedci.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gjayplvbs.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gtqdmtjdq.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gtndizkak.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gnmzdofur.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gqwziqblz.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gloflqjre.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gpyrdsqha.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gqbhgmnap.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/giwgacqws.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gjkbulywn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/giofgdetz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/ghumbzfug.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gfhfwjpwd.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gjeqetsdb.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/ghlugeekl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/ggogudfjw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqakhzil.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/ggxyeeqfg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/getoxyuqj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gmloqzjam.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gwcelepvk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gxtgsybti.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gcpgscipu.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/goqzmgrbu.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwxarnqde.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/glgucoies.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gsjxdqdvu.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gwrwuqvge.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjsxuuh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnqqsaiiw.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gdnkwtsyq.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gjxhiljyi.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/guiabafgk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gutubznam.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/guhjhfgoc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/glegmevzu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gvspnzebe.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gqaorqcoo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/guflgjzcu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gmuoklufi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gzmpmpjqr.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gybdqinif.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gzpbgdows.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gyaibdgpw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/giqwgmwqq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gmwgdypey.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gqakjhqjr.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gwqthhcou.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gpvcinrxx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gafxwdhtt.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/glwdffzan.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gwfzsagfh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gljplpfsy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gezhmeulh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqoquqsla.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gpqzmkdqu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/geamfugch.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/geoivejea.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gyqhjviwk.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gpnvwmrsw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gircqolcl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gjcthttjc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gumcgynnu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gjgjvfxnt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gltmndxof.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gxwnjrkoe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gicppvjlz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gwkxupgak.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grfniftvo.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gevkjchrb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvvychjzu.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gcrhrwpwx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gfzuspesw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gvtwtpkqr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gghpiarwh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gilquqjry.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gqcbmahai.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gfuqlyhsz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gmueincur.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gopywcsbc.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gvwhcswjv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/grcrqicbn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/glrbmsslp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gllixxwuk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gwxgcmmjq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/ggywwdwts.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gnqejjokn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gwuqhdstx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/ggzzkztvt.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gqosktooh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gejdxqcxx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/ggfeducrt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/grjsinjnb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gkvjlcdjx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/giabgvpxo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gkptrvjlf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gavyuuvaw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gkugdvczc.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gwbzplslu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/ggtqztfnk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/gacymvium.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gfteqkwhi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/guiiczrew.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gthsgykft.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/givlaqdoz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gnabqktwr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gmmczhljx.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gjavqwthy.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gqrnwbpsd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnzmxzoa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/goudbkowi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gzuzfihjs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gsgbxvgon.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gewqmmmbh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/grtcbtnlp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gpukedvtb.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gpxxfndup.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gsilmrdfq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gjlixyvjr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/grgxmalfm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gclyyfnrq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gtiykydym.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gxxrdxljq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gcsamlmjf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gtxgzlojm.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gwyhdywjq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gkpcgpbhj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/guesivara.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gpzwymftg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gsqwougco.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ghujnmicd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gxnjldqpc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/ghuizhcuf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gizeklfsk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gifwgmkmg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gcdhfxpat.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gccwzvfxb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gcujbkvtv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gdqvippdy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gqnoxualq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/guoqsoupv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/ggljinutz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/geegwmlug.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gtujnislh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gfkhboyro.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gvxsumvhx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gncegwpnc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gseimtrss.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmzorgz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gmjayaneh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/ghhthjzdl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxilpicqi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gdecxsimc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gatezogyu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdblokiet.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gbwnryqhe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/grfuzudnv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gaqhjqsop.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gumvzfcwp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gidscfhuh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gsvbjgxuo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gxwddywbl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gabjsaqhi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gstbvmnsw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/ggpblxcdb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gigsiybyz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gyzlqkkpo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gzxjhbnjy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gublwsguz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gssbxpfwo.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gyydhhkfa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gpemeqwgp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/ghxumlonv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/giyrrjgce.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gqianaxbe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/grpfxxumz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/grerjrpah.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gcosbfuhn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gwkgwxfxd.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/ghrxbyjkz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gssqqzsvh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gjbprwrej.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/ghhfgtndh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gzauaiprb.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gzyzydvlt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gugrbkkwh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gwumnzqql.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gxpazqidc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ghdpxefbj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gjgbmiqzz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/ghaeqdqvs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/glcifizql.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ganroxfhv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gxrbibaht.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gwewnabws.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gbxlmeerf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gapwpiqft.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gkchrwikv.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/glpvtvuho.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gtjwmjnqi.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gclscaogo.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcjtnpo.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gvtmjblrt.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gorojkoib.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/geupxpwrz.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvosegsck.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/grcfwzdbb.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gsizvzldr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/ghhhrcodh.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gatoagchu.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gkvkrddeg.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gufawvthk.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrhobvx.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gtgdtdsco.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/ganflqker.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goohffoyz.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gsqinnujt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gratanplp.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/glvrysevz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/ghqnejohm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmrlljlzs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmgkpwsqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggjochqbp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grwdfriln.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gvcztxzvw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gxddxxlgq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtktcsqxw.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gtvfqznqz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gqzamgzkj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gvvdozayw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gblltcrel.sHtML


<!-- 参考信息 -->