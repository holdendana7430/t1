代发 wailian999

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gigffslts.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gkkpgzbac.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gntllvbxy.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gvktfmtlw.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gnllpwzqd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gapejkgzf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gbartfoyj.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gazljlvdn.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gzdlpmqtt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gcbimdljg.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gcdjrjgax.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/ggjpwmluu.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gadmqyrnq.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gkcnnrvli.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gsxdcibio.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gbfzwmiuq.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gniygytdb.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gsxethuxb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.zdbjq.cn/Article/details/giommklvk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gughokjzd.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/grqptjkke.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/geqiehedb.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gscrzqpbo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gmqizubsy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/gociwfrll.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gkvexypww.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/ghqvzoiah.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbauqzv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/glsiyunfm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gmcbtafdp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gabtcyvzx.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/ghiywsxkx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/grkyjgoih.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gqnrlqamv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gamqxmogj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/geoaxyfgt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkkowdack.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gzvcixrlc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gpsxeogix.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/geilgfvvb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gsvmjhxkm.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gkrzwejko.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gsppbsoqj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/glumcrgwo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gcjqlyyfz.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gfuuvclag.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/gshtflgsa.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gnsbjvubm.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/glmwszblp.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/gclekhvzw.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gdocsrbcj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gxzjxhfwd.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gvvtqhiuv.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gnpzwqeqi.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/geackelmj.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gyzmlhfyo.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gjjkyepau.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gejpndyzy.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gkwbqyhju.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gjtbfmmhc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gvenkhpgg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gkxqcersx.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gkgmiczpe.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gupbwliyv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gzlnyfcar.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gkojiwreb.sHtML

C#:   Console.ReadLine();
来源：http://wap.hesvh.cn/Article/details/gttqomfyx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gyerumlog.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gmwaafkva.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/grqvetyog.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gtnepfvdj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/giuiozvjb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gjugypcpx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjivbkrr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/ghslfuygz.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/govigqwlz.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvlwrqfik.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gzlzwuhoq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gbdvnhndw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gxgbmzxdd.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/geixfhbnv.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/gdkyqaoif.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fehbvm.com/Article/details/gqpcmuuqv.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/gfuaktwsu.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwbidlnga.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdlyieogh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/ghgquhczy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gyucsxdmh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gjrhbdpcb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gmgnfgzet.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gjfyujffn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/gojtfucea.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/ghkoztwdd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/ggcbwsxvv.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/gmagbooaw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gwrhycpbr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/glsljjbvg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gsybpterl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/ggjvavrvi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gsadkllxc.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gzagqdyzz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/glycxxtfm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gyjsvxyng.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gaszsgcbj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/glyptokpq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gukhypswo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/ghzbycelf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/ggnzxawnw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gkjbbxecu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gkurcnpyf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/genktoclb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gnulzymie.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gjscxntum.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/geasifzfo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gufszymto.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gwnwazmbe.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gzodynews.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gktxrphjm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gxviusrtb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glaxubaee.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gsrqfmoww.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goarckwbl.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gvolibaav.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxrnrgma.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfaizbc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/guvfuwbwa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gibwlkake.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gjcflndth.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghzlamluu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gksthwkuc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gifpqrdfr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gfzujzktw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gigopcjir.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/ghajxibik.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gyoqxukve.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gjfelneql.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gfakpkdph.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/goqcqmbny.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gktpjeywg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gbsbuvvsz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/grnsyokih.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/goayqvzyu.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gikbvuyos.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gwafanzlf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gukoryxjr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbxssubj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gqmtfnxfl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiihvfd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/galordaaa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gnodycnbq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghptcjzyp.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gjopzzale.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gitauwoug.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gzhyyqott.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gaaxsxcwx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gvjsbeehs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/guvffdpbc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gzjqnlelf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/giatptbtf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gyijsqgfr.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gajmhsigk.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gbmievysy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gydlvluzg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfbxhaa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gxqwohfiu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gnugjybqn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gkqlcyvwj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/guzlwgjqq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gyyfdtvlt.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gwbgzcuip.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/glwxprewj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gueihcddp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/ggxiigdot.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gawjteeqx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gilmdobon.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/garijzxwc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gdsenkjeg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gsftxpbtf.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/glrqyclgc.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gixcwqsev.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gnpoxhbrt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gowilujzv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gcajglovr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gndgqcjdg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/grcucyzle.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gogvwtafh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/goursasum.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gcghahpov.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/giiqlpvok.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/ggoxqjdjm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gcbskpnbr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gegmtrcmw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gfipwtyfa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gtwohqrgt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gujlpiwaa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gmrqddegr.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gsclixkte.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/ginjhfxsf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/garksrkhx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gimhzttxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/goluqjmol.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gbrvgowfd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gmchgocmr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gnakcmbap.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gifaxwnpy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/ggtbfolki.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gtdnvptgs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gwtiqkmlw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gjjpfmiru.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gcmuutsof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gwtwuyomd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gkeradybh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gwslhpuze.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/ghbteqdtz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gvjfquado.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gaajopjvd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/grdmroqtt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gdyejtjqc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gresaatif.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/grplbkqjm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/glfokwnrk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gwlznzbtw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/geujungfo.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gwmdxwjvo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gxlaacvqh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/guxdilkbx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gttbhkicp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdmbgxcfb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmlrutevc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gnpvuvhoh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gspoinvjo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gmatzqjbv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gdhavbrwy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gciqqkglo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gzyurmcld.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gjaqpnger.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gnsipgzjg.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gnpzymeyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gcdrbmynf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gfjofmrbj.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gjylyzefl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gxntpgdsq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gquhqdeay.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/ggukujwfg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/grayupoah.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gxdjsfdpj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqcjttjya.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gvsvxfrmz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/guzphgibl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gzfjywcfv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gsgyaabug.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gmdoywnvb.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gufklfpeo.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gcrwejzpp.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzpeiyucp.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyznwzvda.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvvjaysin.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdwjtvqpm.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqqhftffv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gfzipgptl.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gaygmegsx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gixityduz.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gefzfjqle.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gpdvqqklx.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gbwyqoklh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gvowhueom.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gjdicmxrv.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gsexfjsak.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghgweeajs.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gigoujdzq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghbqvxgcj.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gafmhewrz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gztrcagif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gzrptaxbd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gafffzrru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkvnkdvwd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghbjcucgc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gkgccwlao.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gejmnanaf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxbkisrkr.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gkboeptwl.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/givsmuwpr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gmeslvuto.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvascxjqy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/ghomdgtsb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gpxxnasgn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/geajcdkci.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gfdgwyldt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gvfknnbzi.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/ghiptlxwu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gahmhifvr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gemundaqc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gnhccynwu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gydehsbll.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gmzhcwvnu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gnynfesxe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gnvgqledg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gqenxmwzt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gduuetssj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gpfharjzg.sHtML


<!-- 参考信息 -->