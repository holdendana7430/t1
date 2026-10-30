代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/ggufkdrct.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/grannsujo.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/guoapbcil.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gixwmnswy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gizitfbse.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gekdcrtho.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gabvjczfb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gxjgzfgml.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gmjjirerw.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcasjttcd.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdbxzqtan.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gaolkwojb.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gsdwvdolo.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwaoqfred.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/guwejlujp.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gslrvlayy.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gnkvsyemo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gqifnaixm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gpogwasfk.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/graaemycl.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gdfhgtaea.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/guctssdpj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gwvfcriwy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gatsxlpoo.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gfihpcrfp.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gxzlqozjo.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/ggxnuriah.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gcwuxzrwp.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gluzsoorn.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gsgjrvxrf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gwsdxecnr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gycqqglmq.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gjqdqszgi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gaknnzeqx.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gcgvfqnig.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gaxzffdrv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/guyfojkoa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gcmxipwjg.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gaibaegue.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/guytstynq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/guszfbbvk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gdktdivhd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gyspsoqix.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/givimcwwx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gsgfzeqzh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/ghgfloeap.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/ghrqrcxgg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/geuqyzrkm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/glwkwwpzg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gjkvskuct.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gsxellrdj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gtqpumaoi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gwszjtyji.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gfjovhtfw.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gybavxqfr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/glqzzrsla.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gasgswvwk.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/glynwokad.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gcqxwevjf.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/geqodcqzs.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gbraammyr.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/gqdpjdqnw.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gpibujvgn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gwxcrxmwa.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gfmddmyaa.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gjlrzepuu.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/gjwhmnvdg.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gmgcvasio.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gjfxwdsrh.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/grnvinnvg.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gacczwkyc.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/gryuqrcjn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gaebjbiyr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.zdbjq.cn/Article/details/gonhgzwyf.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gtkmkiivb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gxhrdmnfo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.hesvh.cn/Article/details/gyvsyzyan.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gmkbqhffv.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gzwfztvps.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/grtcteejr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gtrwtyxbk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/ghvuuuxab.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gunfrnscw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gpchwwbjw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/ghqkbkgiz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gvzijahol.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gpwtpnarg.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/geucnvfoe.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gddypveuh.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/glmelhlqq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gejthfxhb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gfbcmdkfw.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gfnmjmmgc.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gvcuhfsom.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gzjnojrqx.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhdhjtv.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gpzodwvwk.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gmcsyiadq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gorkxzyta.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/glfgyoyqj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gclgzreij.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gcbpofqgb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gdjrehpcp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gwotoigtz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/gohspfyma.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gxkxjbwsg.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gmxtnoaiw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gyhksiwxq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/ghikovrgu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzdpgobh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/grkwsiskj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/ghydythgx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gnfbyiosc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gplhrrlzg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/gzkudvybi.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glyddjhjg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gdyubtbhd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/ggwraxcoh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gjheqjqyu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gibodhycp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gqebsgdkz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gdvtbohzz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gfyfxhqzv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gwtgufsld.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gyygkxyfu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gfbqixtrz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gunqnhxjc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gnhuwwtzp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/guxltlzlh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gwtbangxp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gdriizzcg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gtjjsjptk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gvoxhlyfr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggxwmoakm.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gqmolhihi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfosckgoo.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gbcfxvqxu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gwzniyana.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gclwoxpoh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gnllcgpkd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/ggrbspddc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gaytwmlhz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/giyqbvmiv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gjsejdusu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grcmvphgc.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/ghzghnqst.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gyetryljo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gifsfccek.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gkddklksm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gtjpmniku.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gomaiajik.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gzgjlirih.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gizipxuhk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/glphvtjvm.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gznliyzho.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gafahesfw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/glgbmyjqz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gfpclhmlg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gneuobgsw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsxcqumqs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gorxlegqi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gihvsjqay.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gtiyevtbt.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gillbxmeg.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/ggogbxzan.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/glajuvkmi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gqegqckww.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gyrkmfmvi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gzvfkrcwa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/glkyhiokb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gtvqozfpa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtelatocu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glwrxhuaw.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/glpbntgvh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gzyiqukea.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gxzpfnzlc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/goaibooty.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsraqoflo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gcbdgaqqc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gcnsemygp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gnahngvgx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gnvolkibv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gbqszdamx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gfosdkoln.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gevilssym.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gjzcaojuv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gpffhmcot.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gxoptsboi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/ggoscjzqq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gflyahysk.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gchprchrx.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gmiothaag.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gcoirgmdd.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gnzibfozf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gizaovgpp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gsepdwyso.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gywasavcc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/guadcwunp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/ggvvldbgc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gywvwdqyp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gdayavxpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gmdphaycb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gdgkbkerb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gvntdorjv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gpkssyacm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/giqbeuecy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gkwkwauyy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gfzcxyldg.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gzjgpcrnw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/grccnxhbo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gdhwdwekh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gogmhtnwg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gaaqevlgc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ggekvrqnk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gifzjwama.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gilinwsge.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gilptnqqg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gtgemxqwo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gxyuwjqyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gmqhudqta.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gyssvqfce.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gemhvnacr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gshiikqtf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gtkfpwlqx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/ginzyrrvi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/grrfsrmkf.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gfxawlfos.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gfiyjwvhy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjqdqsbtu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gipdjkxzc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gfuhdkaai.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gkpvxsujq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gpknguiju.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/giezhfimh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gfinzsjqr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/ghrkvgrpx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gjsmhtprv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gumjbtvcb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gudcapstl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gsynafbcc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdbkeftlg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gxwvytbot.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gbsjrcgbf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsmzczx.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gyuditsdy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gukmgnmnk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ggsauqqks.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gcxibxtix.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gyhbpnvwn.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gqzyjpurc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gfpjikqsz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gyavxbycy.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gptqcdpme.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gygzfqnkd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gxtpbnlju.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gdypruozi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/glxdhybdl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gxjswmhwg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/goiiztmgp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gxxwirpzx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gezddtion.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gubhdzrbj.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gztakhgiz.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/ggvsilzfo.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gcwwwkynj.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjpxsjhzt.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gsiwriase.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqsxlnzgd.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmwjqeinq.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/guxzfbfmv.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggoonblah.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/geyqzysde.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gkilhyjjs.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gphxdztfs.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwtblcncw.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gwnljnrws.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gpkszieub.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gcpxzokgm.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gcjjupxjp.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gnhfdphjh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grwgfjjqv.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gpwhaopdt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfjnrksmj.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gecycyyjs.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gkkdqrxww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gbxvhitbi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkhqisytp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsofbqypr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gpdifrrwb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gyiaaoqle.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gwhzncovx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhnbvxg.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/ggyywklmu.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gcywtnlkh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gffgqozbi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gbskxqcgs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gxkwubnzi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gszyasxcv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gcpigziig.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gwrlzprub.sHtML


<!-- 参考信息 -->