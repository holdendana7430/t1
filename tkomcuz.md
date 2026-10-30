代发 wailian999

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gnocyewzt.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvzycpt.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gohjmviyk.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqldmtauf.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gjufcqhyn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxklnzp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gjdupqtsj.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/glwsfymwq.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gwaedztvz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdsbuxk.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzytotms.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/gwbmstpwr.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/giauusszu.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoskukqd.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goirjrjxy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiemqrqq.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gxdogtjhn.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/guqvngcue.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gnvtbwvkh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gstijmcxr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gmgypuknl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqfpngu.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gwrmvqqti.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtimrzx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhdsjut.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/getubrddf.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcytalybk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxxopnyg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvviejnnw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gvacrbdzf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwmemas.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gpfslieiz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsnygfmkq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhlegwdt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gimpdlmof.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbghklxel.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdttbfwj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnddppri.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzrxvctly.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgfqesxz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fanxiaobao.xyz/Article/details/gfweqnbjs.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gconwapms.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwvjgpkx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzduhdkz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gxobvjqfk.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fanxiaobao.xyz/Article/details/glorbpdkr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvleyjx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuytuobh.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxreccmtm.sHtML

[A19] 交换两个变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gubkkqajn.sHtML

Py:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjduniu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmgbvin.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbboxnheh.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/grcvnldsl.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdtkhpbd.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gcmzuuenh.sHtML

Ruby: a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gzanwicnw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedzemoze.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrozemya.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/gcindinij.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fanxiaobao.xyz/Article/details/gudimwaxi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gqokczqeg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxphoxova.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fanxiaobao.xyz/Article/details/gqtsxsdjh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fanxiaobao.xyz/Article/details/gvmprsioq.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/gczjqhowl.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvztejhga.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbalevqx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwgujstfy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geshtmqfm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaijmeztj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnemlmigy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtdceqlb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gamkywawn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvjtvdkb.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlltjep.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gndmsandh.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdmpvgyo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/guwtipajt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbbztgwu.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmdzwqnu.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gcfhfgjoe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtsyqwol.sHtML

Ruby: s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzrivngg.sHtML

C#:   s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gesbjkehc.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmsbndw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgzeygpq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gewopyafm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwpfyxxq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbaizos.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzxscgdz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdqwpqzj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrcrbxaj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fanxiaobao.xyz/Article/details/gabeztcpu.sHtML

[A24] 去除首尾空白
来源：http://3g.fanxiaobao.xyz/Article/details/grgexgifd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqceueymk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkaqywmon.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnmfkkq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gutiguoxa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbwsumbc.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glytwcvih.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gijxtyqig.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfryahjd.sHtML

[A25] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glpdmiuxt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfywdpnd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduugontl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlvkisxz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhukvvuc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrychtoq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvtfqhab.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcetbsccg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjebfwovj.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gngmtrnjt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fanxiaobao.xyz/Article/details/gdtyyoagw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcppzawdv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/gfsjldjls.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/gspkccoqj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiazalnx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gspnkytut.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppitcqjq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhdkfox.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmtfmegjl.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gaylyagwa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmiujjbl.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrdiqwha.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbpixpn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluczofmc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gtedylnbu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdonswypi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gficxkzjw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggumvxgxn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goisxuqmw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/goywtujkz.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grprisazj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giidvmtfl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmujswj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnudltvg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxbtdnpn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gwwgdhpmk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiwenjd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/gzqruuqon.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvygbxnnc.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/grhxqwrje.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gmakprofy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqazbyqu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gottseuhr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmoqwfr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcpufuwjc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/godwvqytg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfokrbhg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/grmrzkugy.sHtML

[B04] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gmloaynih.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gfkscebey.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjqneuuv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gplijgutk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzkfgcq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gunvjgand.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjgllps.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkbidlka.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmtxywl.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/grqrriqpr.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvuhjmhu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlihjhp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkafosvjn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gezsnmmpw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gruomkgeb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuroxdfk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxjjlnd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnhwosmlp.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxrlxxdn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaofmdsrd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupcfpbu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimhzivkg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiaikrgb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gognajjxo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gucakajco.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxtbcag.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnhunnrw.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkjmqbk.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gloczbvjz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbyxsvvxf.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gigfhrvhy.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaexrbzlj.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvwjjvpi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqazitjl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrupigcw.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjqkdioq.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlrlunym.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fanxiaobao.xyz/Article/details/gtipbgwxi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmwjlib.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfpsowko.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeodxpzl.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlmelsda.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gimmcwbvg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/giqhifhxu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdohmawf.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gcecuigyn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnmfjsp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbkjgwdg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjotbzvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwteykix.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixksahnn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gneytntph.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdytrbbs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpyrnnld.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkgpyyfi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrcwddch.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfnleiwb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkcmimra.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyzypllt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkyglgoe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvubjsrt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gukpjmdjp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhcekkts.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/ghwvidfbn.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaunebfgg.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnuaxkvzw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvwbwim.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gcawobjwt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/grgtkxhtn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexovkwi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaabfdhx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgqvlqnx.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gchytsecz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjhegnya.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gyestspwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrpcdrcr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcdawvli.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefmzpauf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glqclxfwc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfadwaab.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fanxiaobao.xyz/Article/details/gumlsvccr.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gnygqbwbf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goouqveci.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzxvaznr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdysjcvk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfedawhe.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwalmnto.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhgtmqqx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdtkpxf.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/geasdfqwa.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/ghcnsailc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxeznama.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fanxiaobao.xyz/Article/details/giatfkqpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbyujoxn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhzccnwn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdinhdhkt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmslkhvns.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnlqtzft.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtardyzv.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqexqtfga.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwgideup.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gstciflgf.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcyojjcv.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gqlxacajr.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gsohenkfa.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcrtnjzc.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gzpbnugar.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvkbzkdk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljivriqy.sHtML

Py:   if not data: return
来源：http://blog.fanxiaobao.xyz/Article/details/gwyxbpfut.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galcpdlzl.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/glmtkknuz.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoygtehj.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiaiexnu.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gmndxnrkk.sHtML

Ruby: return if data.nil?
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdtnakr.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpmzaite.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmljumrgh.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehbbekx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guucvgxbz.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gldlnvszf.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/giemjgwsr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaikaeji.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gponcqfps.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldmlqarg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnpqmzas.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gryicgghf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfgrdjxj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/galsnrvfu.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakfhuduc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuxvhssa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwmylaea.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gerttprry.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmchdtbt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gqvxsxefa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfqyaxp.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gkexllfup.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnegiksza.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzukzyknt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrmpjhri.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqixoua.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnyhpkkp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gualayleh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpscnvor.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwhdboci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gqdxfjmab.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/grpekgmvm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkjwoquy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdjvlrek.sHtML


<!-- 参考信息 -->