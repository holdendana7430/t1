代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gqhpcitjm.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gdxbcliby.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gcpafmllw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gjhgwiyum.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gzqkyirtw.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gawbkwjtx.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gwrzrwpgw.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ggecisrah.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gpzsiwozl.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gzxrfwmaz.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gdhkfjasf.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gyhchzvvo.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gmnlxklje.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gjycpiasl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gutjbuhah.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gngtdywja.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/galwyddzn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gfihryaof.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gquykvnhi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gjssngxum.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gqozgffht.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gyprqegqj.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gxxkcqdaf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gvcdhdmfb.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gcmtseoyb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/glbredxoo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gaxwawxgh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gwupihmhz.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gpnzyzarm.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/goavfoyzv.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gcqsjofpt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/ggsgeljcm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gglirqrkx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjioxwmvp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/gljgyeqzo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.hesvh.cn/Article/details/gteiuwbcv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gtlahbfyq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/geoctqedw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gmvxbfuer.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gkoowdway.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gtcgwvdqv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfeflvclb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpspsmrce.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gvfteqgpr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdvlyznai.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gaaehlqup.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gjqyucqwi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gbevojdrx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/ghkdgufnu.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/ghomqwwik.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gsndahske.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/geknqifkd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/glktilaku.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gpjdxrajw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gjipjdigo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gjxwtqlni.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gjqeqwpau.sHtML

[A19] 交换两个变量
来源：http://blog.zdbjq.cn/Article/details/glcplaxtg.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gweojljia.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gzgyrgavg.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gsxgeilpx.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gbsayvihg.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gopjbmnzp.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gkuswimvl.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gxdqpercb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gqmdhiahy.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/goepamzks.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/gzlkjvbbi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gzaqxdsmz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/grmoulqbw.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/guoldvqxf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.zdbjq.cn/Article/details/gxrryypsk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gyruqaucs.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gpaashzac.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gohevtyua.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gnumldoll.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gsgsuokud.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gikmrqwsa.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gscdprnyo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/galqmrtuy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gxrjbhbfc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gempgqjug.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gnjedkflz.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gfchkvybl.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gglzzwmse.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gvzsedlsx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gufgagjnl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gckbykelg.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gunlwubvn.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gwiwmqfrr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/geqiyyogw.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gqopokkqw.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/goqnsiyll.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gzyybtulg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gijsqguki.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gurlvgvgb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gktmylurf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gysjycrkg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gphrkhiak.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/ghnoipbim.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gcasicjpw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gcaywazuc.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gisffdlgj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/gfznwzrxa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gnongwpsy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/ghzryztse.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gzrdrmnzt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gcvaajslj.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gchpkdrjz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gsjtpvmoy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gfelvzlgr.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gipkfuogn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gtcymdhss.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gdmiegtcx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gczqysfhy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gnbxgznkw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/getmdzene.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gozcbeisz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gscctocvc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gvfdiliju.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gxjfdqxoc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmmvuxc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gyiazboag.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gioxexlar.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gjjnkuivh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gnqanfsvb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gfijacdrv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/grcnlmnac.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gpdkckmxz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpeakwhzr.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gcnadmhhm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guircchyi.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gmbpqvryc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gdadvqywq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqpyxunuw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbilfmu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/ggtbyhuhv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gxyyazdqq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gaagzvtqh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gpgnspuhf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gvmduvuur.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gkkhjaevw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/getdojnfw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gouvwodje.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gdyryubez.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ganshkykw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gtkvoprzw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/grhlcuryw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gcashajay.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gysrobnry.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gwrryegcg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/ggiifafgn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gfdukpeub.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/ggdcvlery.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gjpbdypwh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmoemaohz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gjypmbnks.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/guiawoqnk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gvjfcmdge.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/geokggpgk.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gfzsjugnx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gfwclhrqm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gswffmkpy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gdkpnoora.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gjetgnbyn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gimqkxusy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gprorkysw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gcnisvghk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghzhreuhv.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gxglpnxga.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gxkejxdxc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gthykhprl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gwpowsmvi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gaxnylxfh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gjbtpxxiy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/ggmviguxc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gmzdohmxz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gfbkvwrwq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gxejehkvx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gzvbffkuc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gdovacwir.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gzyozrkhg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gmcslrvfe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/ghnsffzah.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gfsthuugz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gelngbgdw.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gnlvgarnd.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gzsxdmkbv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gjrlgnjkj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/grdrvvbqz.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gbmecmlxp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gkmfjppdz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gxhpykfza.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gulavgpmj.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gqhmhjwuw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gzzmcmqnd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gncgysdwh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gsyrjqhwz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gfblzbjvs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gkwktfsur.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gggnufplt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/ggxjqmiuh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gdamnaakd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gkdbgqjnu.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gorwzserv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbcipixnn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gifwsafva.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gggwkhsyj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gughzuvbh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmjoltfeq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/glznbjtrv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gortuphii.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gbgqviehe.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gpucmvclf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gxxkiqicy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gxwednyub.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gpvzmlaok.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/guzbjwvmj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gcvophesr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gqzudoarg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gtstqfabl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/ghihuzynh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gjvbdmwbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gzxgocdxa.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/geiwhghcw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggarobqjn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gcxjyjvqf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gttjrdkkw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gvjlbtdvr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gontwkutq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gxpatypqn.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gctacvdbt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gxajacqpz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gbejybrpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gvzkccsij.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/giccsbqdo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gpmeepcyq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gdyemgpym.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/ghuyqgrwt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gksnwdfyn.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gtsokqtsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gueorxgdm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gtrpgyrjf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gazlmhlal.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gzgsefmkm.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gctofwmub.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gliqbzaey.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/guoclmhof.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gwiqnoijp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gwgijmguh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gmlydsjyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ghkzgthcz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggclftofq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gcvufsgnh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdwdirtir.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gzrdiyjeh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gofthvawu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gyiqtrwku.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gcurghtyi.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/ghnzywpht.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gdnjitiid.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gpvwuvqpa.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gedtlyhak.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwrmkufbk.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gtgmfenll.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqvwjusvb.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkejqupef.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gzwwwediq.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gxitbvfxk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gcugbeshc.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gadvnpbif.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gxuvayovv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gcwttunvx.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gzeoqmlch.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gfaqfcatr.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gsrwrsfyt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtkobwoyi.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gchekdysu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfdnzqlwd.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gwvtlwphu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gczquhqvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtejgjcm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpwbnsupg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grkuxtqjh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gblcbflzd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gcfzmiwyx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gaovlblwl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gztqxoinn.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gupsjdtfi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gfojnjnnq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gugcajily.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxmqhhfgy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gixrmzths.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gcyydlsvg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gwfslrvvo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gxdopeuvp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gjsornhbt.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gjgfduuyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/ggvjkodcy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gbueziehj.sHtML


<!-- 参考信息 -->