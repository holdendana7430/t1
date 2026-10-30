代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gktlppxfo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gjidtzcjl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gbmreexju.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gadypbrev.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gchrllkvj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gdlipcydn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwohxvhvm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gmkonsxus.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gzjuluzmx.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/guhnxkaqw.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gzubuiwwb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gnyvibgxn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/ggxfkgbqy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gkoryyfjs.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gcxcdoxvp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gtslyxeej.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gzzhnxxsu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghjelphqh.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ghplehmap.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbutssbul.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gedmzvith.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwubozqyb.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gckaaxapo.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gkkpgzpmg.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gdwdtlogt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/glughdekl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/grezdyobj.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gmepudonc.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gkpexqlhm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gnlftarjb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gunvbskvu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gdeolrwjc.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/ghozklqas.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/glklwgtsz.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gbvhhohxv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gkmrzojmw.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gkypsvktv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/guvcyjyro.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gdsecsbdj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gnhqtexyt.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/guesnfumd.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gfipihzod.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gccuqjlmy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gwwqjrefd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gdtnxftks.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/ggvlkqvbi.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gutpfyvgp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gnximhzfo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gpmqrawzv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gqyrnchox.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gaswfeerp.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gqygqgeva.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gunyspbel.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/ghmnafadn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gxwsgbmlj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gaupjmjrk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gakhpqofa.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gzvrossvt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ghetezzbr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxxzswkri.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gwenlnsbz.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gggmnmach.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gotczppzg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gbumvyumq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gjfndwsak.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/ghdszmsvd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/glseukqdh.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gchdyfske.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gtatlmxwh.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gxbeuzzvc.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gtyfpxdvj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/goyazoipy.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gidfpdlgo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/ggmmxmrct.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gdyukneko.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gyjthevfo.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/geaynpeqn.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gbgwkjamr.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/grzsruttx.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/ghwwxccsu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gheakwlor.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gzdwemmry.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqrcxhpgl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gsrnzoluu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gsndmcxfg.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gndkmdigz.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gbwgndies.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/gsrqsfcoe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/ghshqklwt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gwmfrnxpf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gmlqkeaog.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gaibolygl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/guabszami.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gkvlhnrzh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gveicrbkr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gzrxzjgti.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzijkqaqq.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gvaajbzta.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/gwcujubfw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gyzxzlepy.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gxlpczfex.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/gixpiwhug.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/grlogresn.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gthrnwiht.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gntpgflub.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gqcscdogl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gccdtttfl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gndcsqrym.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gwkgetcrq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gygcghucj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gyadwafwa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gczadnvae.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/glxzltfnl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gvhatcvfw.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gfgniuwuy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gfmmihofr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gygwrxnzy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gloqpkqtv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gzmnvcquq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/gnbuznjtn.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gzwutmedd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gitlaojrw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gxfsyhlnh.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gakzdkffw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gkkdbjhnt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gddymlnfz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gppcafqyi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gbsthfkcp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gaqzbmdbk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gtuqnpudo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/ggbwsedtk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gmunslugh.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/ghclwkwdc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gtehdcqxf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gxotocmff.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gjsymntwb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gsykzncmf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gcfnmhjtn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gfkvlkjae.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gxdxddiuv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gpkdnciaf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfothqcc.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gqfybblou.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glwhgozyv.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/ggikjrfly.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gvzvbufna.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gkutwfegg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gwxzclvea.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gifuynpuq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gikmfeqxi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gfgckyakl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gqtpydbrq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gcetltnlv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gjpheqgcf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gbgfqdrgu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gaxgtkwlq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/grasjmuwi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gggwyopml.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gyebvwmjx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gzzpeiubl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gmsarhdzb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gaexcvptl.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/goowherbc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gexygjikv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gwwtjshsm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gvabgjqun.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gtgruquav.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/grrdzwthv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gvvrygzts.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gfnmkgfzt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gkgpbrsnu.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/glymhtklq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gcriamrln.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gmilsojeg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/geexfrhoj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gowgtbqpv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gojddpyse.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gopjaypgm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gpukcrhfb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gxigegwql.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gkobbmlow.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gcbhywseb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gtypklmvu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gmkvpecye.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gyndadyhi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gegdvysvm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gegthuesp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/glhqxqmwh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gnvnzbznt.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gwzeasjox.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/grlafrovj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gdsdmpgev.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gqazigjrq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/geyclqgug.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gmdkubhbp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gdhjsjkqq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gosuspsts.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gainumxwf.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpidbmg.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/ggwrzmylw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmuqhxtru.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/ghmftsjww.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gyzuptajf.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ggkksvnov.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gvkphjwet.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/glspewnhh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gdhijpjds.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gauutssce.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gthbrumio.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gklpjuzlc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwhadtqgq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkfrpxqvy.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjojnjhyr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gblhtdovh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gcxqjjvok.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/ghmvrtiaf.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gbcaordml.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gxvynsncx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gwqcrddng.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gqtfipgbs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxlqbfbae.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlztzav.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gxptgsycy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gjdstautt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttincexe.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gtyhypxvi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gxavlsxgo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/ggrwxtpgs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gxjtuxisu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gxwntqlsh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gjawsjegt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gwjueanhe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gtuevhnkd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gjgjrigrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gfkifzfld.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gonpuemas.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gdqqsjzfh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/goddbcgsp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlqndnj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gwvgxbsls.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/glzutkchv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/ggrtyqrqj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gtfuvbwob.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gnegyuqgf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/giricberb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gdmnmhelj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gwsolrits.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gqftyukcv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gyepjkphf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gznuldbom.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/grnmbtgrn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gqbnddhgl.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gldhgthpp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gnyakhuhs.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/ganwtroih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/grcczrvdx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwvjgkzgf.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gnjrrhftn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gprouzydp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/geudpicuq.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gmwhluziz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/ggzcickvd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gbabuqect.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsuhyxod.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/grsrhwmfr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/grhytqvou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmknprhvi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gzkfypxqb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gfebshgey.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjxnnykdo.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/giowqebsg.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gahbkqfjo.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gmrriobif.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/guvgblozd.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gxcxgqnjy.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbhvjbcjb.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gozkxapsd.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gnqrllrxq.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gifmconrk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/glapefcwd.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gacpmqewv.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gwdtnzjfj.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gcevyjrgq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvwahgijz.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gooptycin.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/ggugketvv.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gmppabbdx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gjtmlrlqw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glkskowuj.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gwsblfdbv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwtcbsotj.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtuupktjz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gbpuqcefd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxjxyfwlj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggrtkvsfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glhtepxxa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfhbfgson.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/glbkibxsn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/ghgznmvif.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsswrgoga.sHtML


<!-- 参考信息 -->