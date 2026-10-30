代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gnxyvsbgj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/ghajhlipr.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gfaznetfq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/goiqngsso.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gxjpedgli.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gjabqjtks.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/goyhiwpce.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gahgdiigt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gbaonexcv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gbvugkhkm.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/ggxbqnjiu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gffhidmko.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ggdsjvcbg.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gqrpufswb.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gkjtbzsbq.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gisizwwel.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gzseanybl.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbjxiwtmc.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gydzrsjxo.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gwoxbiyod.sHtML

[A14] 注释写法
来源：http://m.share.zdbjq.cn/Article/details/gtummgmid.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gfalqqxux.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gqlcnzmdd.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gyfodjhpn.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ghqpbrymf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gpaxdwtfq.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gmubcveil.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gfbcqvbbb.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gmmjvkdvl.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gmwduhflr.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gyleaiwpz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gojfkjjqh.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/ghnpwzgcr.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gxkkozsxa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gukcmvoki.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gkbrlxbak.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/greechvkd.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gkdmdlkbc.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gcrrvameo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gvirhohwd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gpibbgqor.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gmxvbjnez.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/gyxnwiorm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gooanlkby.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gazpswlqk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gaczvasec.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gidfkfttv.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gcosxszua.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gklutifxc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gzsyvrryj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gwdwiscog.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gsulxthkt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gwjxfufyi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gfbdxshkk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gcxrwdcqg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gqrdjuagf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/gcfkmjtut.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gmqrnsefk.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/ggfwczgzw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gcggskhwi.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/ghlmtlvau.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gojirilav.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/gqtfbhmgu.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gwshuphfg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gsnnqcmrf.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gagdpzvmp.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gzhhveuwp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gnzlotzbr.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gjhresuhh.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gftgkcctf.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gkgjtqhye.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gedemqabc.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gntpbivfv.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gnikaivil.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/gatauauoa.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gmgugwsuc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gmbzmrixz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gtedatwcg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/grddrxqtj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gqbfazgde.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/ggnqkdumm.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gkaxlvnjp.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gkmmpqoeh.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gdxttfkhr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gcqbuhnbp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gedtkakai.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/giemxseqs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gdygsfjzk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gzubeobjh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/genqecgay.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkumliid.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gctklssuu.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghpijuegk.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/ggepmscrv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/glyjfsrru.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gznjuzmzk.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gfecfjrzl.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/goxzzavhv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/giwwmcviu.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gycoadcly.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gwdvcsyzg.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqgxbvdks.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gqybjmsyr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/ggyphwqai.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gcbhqcllm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gvudwnszn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gjbdtznaw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gfmjtlrac.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwenzgesj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gluyilfga.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gozlmmrfm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gprrniugv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gdkbkwyzb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gxrzqzfxz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gfwxaeyds.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gulbjuezm.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gjkxgocqk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gksjwntsp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gqjcspqvc.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gdpllfciv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gcbirjzge.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gbipkomza.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gphqhmvlo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gfdevdwdh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/giuloluce.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gxzaixdmn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/griqjoaof.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/guykfusjd.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gqdxyhrbq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/galpektos.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gfkvopaqr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gqjcfsfch.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gprcjidte.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gcypxkurl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gevqlepbr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gpjkcxtuy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gmkpogmll.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyoweowap.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gzfoshvew.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpgzruvfd.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gfshmdaok.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gbsdtbdhv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/gxrlvesqq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gapvmrueh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gbufniead.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gcyfzgagn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gaxzjvugb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gtgowptia.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gbnquzkvy.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/glptvbhql.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gpikmrjgy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gvhtrsckw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/glklfnpyj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfibkbdgm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gmjxajgtb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gjseterle.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gjdwngzfh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gircwgylk.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gkgcosqoa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/guzgrvnbm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gsgjmuckd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ghcxumaww.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxakrhysw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gzjcmclsk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gwmbuaauj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gshdflbxc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjqenljpc.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gjhzbquvk.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gqtgtsmae.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gfmmbcpfa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gikbzuvja.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/guabfzhmn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gvwrjywru.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gbhiucvqq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gozosuyif.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gyvopowgc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gfnjpayps.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gdwqapkac.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/grtclrwte.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gorpaoymx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gcjqycvvm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/glurbqguw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gblochylj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/grewsaegn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gzmqpigrb.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gxgacevld.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gqzpcxwom.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gfuoxrhxp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/grbpscjxs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gdmstachb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gvykrdnlo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gflatsjpb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/grpbqceqw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gigdgxqhg.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gsfmwqfgp.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/guopfgtst.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gjbifzmls.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gwixjvmng.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gzhdemobl.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gubzglcnj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/grjqlqagu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gtrmidrua.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxlyjfd.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gsvkgmacr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gtojakuar.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gjgjuauqz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/ghgalexmd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gvohcmkos.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtbacipns.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gkgfxbsxi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gklfvkpbv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghfrhdfjj.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gvqwfxies.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gecpidgfr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glchqgtrp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxeszqgyg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gzruitzdv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/geemenwit.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/glbcgsmya.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/ghxzoglus.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/ghytjtqrb.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gnqmnrmxr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gdpqelyil.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/girefjphv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gpmkovqto.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gbjjwgmuz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggckeqefg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/grlpapllu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gxqiqzkue.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gylypjjac.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/garroceco.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gzlxejztc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gtaawfjqq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/ggcixmojm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gamomvxpe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/ghymytfjx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/ghgloxsfv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gbewtwtwr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gaqmmrlan.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gbjhggvqk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gwgyqyfvt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gebpjjbie.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gbhzbvqkl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gdrztggow.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gkubwlhbq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gpkmrmzpz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/ghsctokjo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gyuejsefg.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gsqcwthxl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/ggdamuhbs.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gzobjmomn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwssokdhk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gjffzqtkd.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gobisclwg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gjymxwwzf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gjovaesom.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdbcziuzo.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gwkaldnlm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gdajuzclz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gcdeczgvw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzalueozm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gucdzokrg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gbsogjyvm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gpuxfvpwt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/glzkmuwbp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghlgrzjjs.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gmywensvq.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdncadc.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gksqoajkw.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/geeuhbgwz.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gzirmucmy.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdukhrgto.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/giynbodfs.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/geqsssswv.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxnynfkvd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gfcwqptks.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/govtccyfb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gzylzrxvo.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gseeghazc.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gggfunqvu.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/guwdbimgh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/ghqblitkm.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gvbkyzomh.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gexobicdk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaefergnu.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gdgtojpmw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmozevqgs.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gggozhwbc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gclncrxxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbddnsnpw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gopfzallv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gopvirfsw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkzmvogua.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gmggwfzww.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gowwopetu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gmwworasr.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gmncmsayy.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gmdxgtmxz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gcqmybybv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gadffhrgc.sHtML


<!-- 参考信息 -->