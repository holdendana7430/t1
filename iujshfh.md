代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gxkplgczr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzotfvq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxemmnw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgrairip.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkznkdwew.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gokabxwrj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknvpwayu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmfwhdck.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydekljl.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflxfzrlq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggeqfdirq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gybobfuof.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gargfukon.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gtqvvfqkq.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/grflvujvl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghotjsiho.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzptiqyva.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/ghnwdbwuv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtofoxlt.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmwhhsmb.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyatgbmi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fanxiaobao.xyz/Article/details/gbulqomog.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsyzxocb.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgfrbrxl.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gbnagibks.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/gfmtdlquy.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gdagnfqpr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/guwoyxgbj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gomqcevfe.sHtML

[A15] 空值判断与默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gdqunqkfy.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gcuwjwsit.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxyqqajd.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxbslwbe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkgwhcaj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqswtlwqh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkdcfru.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gumnsyrbm.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpktiiq.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gblzemymx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/goxcekzbb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gbxucqnhi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlzhyqmf.sHtML

TS:   if (!x) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxpswqrd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggyovspvi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqqcxgdbv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwaqhhbv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmlxylxeg.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttqjxlyv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsthuwa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfrbykrq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogfbtzmx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/grwcowkbq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gudktydpo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcxtcarnp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcmcqdla.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqewuet.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gvumaatlt.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkgecwee.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gdrtubpwk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gajtyaqqs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjedmvovz.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/gzuwznvmt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gupmmparx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpdrshup.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/gdniyllac.sHtML

[A19] 交换两个变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grfymxpii.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmtqnne.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbnrtdsv.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fanxiaobao.xyz/Article/details/gavyzoxog.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gjazmdfnj.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fanxiaobao.xyz/Article/details/gifbweqoo.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqnwbztl.sHtML

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/ggciywccs.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjnjidsmb.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoqhwrxm.sHtML

Py:   name = input("请输入：")
来源：http://wap.fanxiaobao.xyz/Article/details/gfibdzbzm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwoibhzt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fanxiaobao.xyz/Article/details/gfduwmkld.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gqtlmghfx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyfkmwkx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuvmjpub.sHtML

Ruby: gets.chomp
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaoamzbe.sHtML

C#:   Console.ReadLine();
来源：http://wap.fanxiaobao.xyz/Article/details/grvnnwokk.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fanxiaobao.xyz/Article/details/gohhqbxwu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtmjkps.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guveidbwe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfagato.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyzodso.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaogvbzqa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjwjaxsy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gtbfpxqns.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyseemylz.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/glagclqyg.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomzlxads.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fanxiaobao.xyz/Article/details/gnucwcufu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuwebjfq.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/giesexwma.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gccksktln.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgxsytmk.sHtML

Ruby: s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhjnwpft.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/guiaeccun.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grrxbwamw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmktwjr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhimaioe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwsljra.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjnyeca.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukmndjco.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gerpvcbtc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galprobko.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fanxiaobao.xyz/Article/details/gehixwjqz.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glajfesyz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtlakxak.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghfwogwnl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gpwcgjqnw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gjkkxhpgc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpavuwbr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwllenggo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fanxiaobao.xyz/Article/details/gazwazoif.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gflpnnsmt.sHtML

[A25] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodhkiau.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fanxiaobao.xyz/Article/details/gfbozbcuc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gztuuhqzl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiagqfxy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggiphtiue.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxuzyxkn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqgrumzw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/ghcbjgypw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gitvwpvbp.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmylkjv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcufipzyk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmarjokzs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fanxiaobao.xyz/Article/details/gbvmaodqm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/glinfhpzg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/grswaaaex.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvjwwausz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/glnokuimb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkzxotxv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhydtjz.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gdruevjpe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxygajin.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhgxnjv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gksvfczah.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpsrlezie.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gujwohboc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gfilkzpou.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/grxylkagw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjyauxwt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gecmmfsfr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzayvslvw.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsssdjipr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gyzimeeed.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmwrxzwnd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gqvuxbkll.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrsmnmhp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gzsgttpuy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgppqog.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjwjrjr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gvdvizlfl.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/ggfxnjfzc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/gnbxdmcfm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvxoqtrna.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggakshfhp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfovrzyie.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtazwgfnh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztebwixj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fanxiaobao.xyz/Article/details/grnnygeam.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnarrmgh.sHtML

[B04] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gpbechkvm.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fanxiaobao.xyz/Article/details/grekhccqd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbmijdae.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghynokebz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzehbypss.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbskgzxsn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gshmbogst.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fanxiaobao.xyz/Article/details/gekbrawji.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyldeplp.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfbkeego.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqpwrbsa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgzkwoqa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goylnlqkk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffwtxqyf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gexwvhuvk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyudnwgcb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gsprxxmay.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmjubxvt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaqrwuvl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjayajwh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtnlrfve.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbyysctu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsckvhbq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdrksxvt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvyqwyit.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gttqgjmhj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzouhohls.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/gppqnhzsv.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlckhlms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrylunfg.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbairsnt.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsxezhpl.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghtbsxuki.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gflvrppoj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmkksxdm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtyntwru.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixtysgxt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzusxks.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjrklxxv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gzumthyvb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmheygoi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzokfukrr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxvtngaa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdfmfdgeg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkamnvqra.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyrhanrh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/guclxqimx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpjlijpfx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gysdgmtmo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqcprrvat.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gumnhityz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gaespbojo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/ghyogpydp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlyslqff.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gikigtvmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypsfhttw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpxnzlkh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/glajzmnoi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gsowmvftq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykunlsgp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfidycgy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokfvhtv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/guuxisygg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gnynfvwyp.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghceexueo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gjloeeaek.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoohyqif.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gxbrbvngi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/goitebuey.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gajbmhpdg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gajuwwblt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhouugvt.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdypdhym.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrtvzsgv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/ghqxwgjie.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjpgkrxi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gculnnkdk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqwcdyrd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnswcvwzd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gmhldscpl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgrzxmmt.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwxlldygf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtuotfvj.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbmfnvbh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbeogfjt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghszantyb.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjehrvwy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/glmochwvw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjtdchjc.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gdritzapb.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gjesddquy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjwsfmzl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajfegqd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerrhdvmz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoftfqfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnvziwg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guumurxzg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqtglxbg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrgsquho.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/glbgxxuia.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzyhdret.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/glqxbpdtx.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gglqgencp.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grphvuykp.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gkmrxktsx.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdwqbdc.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaohfnfbp.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhpqfhpa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gcvhroubp.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/gokrbgrhz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grjoilruk.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gipogjrbj.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gterobymc.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzinqws.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvimowe.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcfsavan.sHtML

C#:   if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhshgxiq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxkdzltb.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeqmuqdy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghoucllml.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmutmfwz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gxwscvlbi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfatemhh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoylslht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxevqhbmg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyfdecjex.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/griqjxebt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/giasnbrbd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giplgqdoz.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpwocovly.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgxiqgsj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxnzvqn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtjuswy.sHtML


<!-- 参考信息 -->