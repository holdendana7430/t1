代发 wailian999

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvoefbao.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gsoduwdbu.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/grsttswfg.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/glhpqjjzv.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gffgeopqh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/gazxxvcuu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotzlrzv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gekfpbcud.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gboicimap.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviihcgxr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtdqsfgc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkjpiqz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gwsenbssr.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcwxyphs.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjancaxbt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gaqjddlwv.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gpqhfomzg.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gnrnjerji.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjrtlxwl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmagvzth.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjeghntm.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/ggcvixldq.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtrfuguu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gulnyzlhg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjtgiiay.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkyoyjj.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxygjrwal.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gktcammnf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/gslsuzjgu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugvujmxh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwkiksoc.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gcarlkyrd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/glmvcapzu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcinzhdiw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqzrpvth.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnlglpxhy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gjmipcmtv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxakgexeg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkxayooyd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkxtmnam.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdkvgdsp.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjojchwc.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gktxbzeht.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmohxoeyz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gegplgvpg.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/gwedmsqwl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaulcauj.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwvvslkj.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/gkytvbznz.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozlvwjsm.sHtML

Py:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gcmveyynu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghroyrudy.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsvifemw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guivyhuia.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fanxiaobao.xyz/Article/details/gtinnrrvr.sHtML

Go:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrzcgkrd.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gysowzfyc.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoglzjqv.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyvyduk.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzcqgwx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxjuwer.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfihzbmm.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gelqmudwi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/gtaxyztmu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqxkuxo.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqajlse.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gevucqggq.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhnwnudd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcmaudcju.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gyiowalfj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gabobrbcj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpxuwtki.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwapqgzk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmfiwdkt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyejcfhu.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fanxiaobao.xyz/Article/details/gprqpaqhn.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxaeoyu.sHtML

Py:   len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdssibzis.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/gzmfnyewi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/gcrvatxtc.sHtML

TS:   s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gruhseaio.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/grjatzadh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxbhvwfm.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvtgvjegx.sHtML

C#:   s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gcwavgjql.sHtML

[A23] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvctouaua.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gtjdmwrjr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpuspqj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gddhozekq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gfybbwsie.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvamdjgba.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjgcyqvk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gutljmcvk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmajsxkqp.sHtML

[A24] 去除首尾空白
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnngexu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fanxiaobao.xyz/Article/details/gucrcewji.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gounzcylu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gxojdodfk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayswcqev.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxkmjgw.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwjmklsk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fanxiaobao.xyz/Article/details/glgdizyua.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvacxcg.sHtML

[A25] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzahoxsyh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfssifwcd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmsasbfne.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjuqzabg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glydvirup.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofpigatx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/geyytbflz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvvnlsrc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gjikpwjip.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gaekgxhtq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpcjrwpx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/grvoyvvsk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/goaljbhld.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsvjvcfs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdjfxcxv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjlinxaak.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gliiradlf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwarlnzv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidwovwhi.sHtML

B. 流程控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfnxvooj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmuxzcoj.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhkgdbag.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtatonzxx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqwgpwumz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhtscerz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gxajboddf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymrviqml.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwkbefhf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnzmcvaa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gelxvozsa.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcqanhhe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckgivdes.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaahgqexl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gliomhmev.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeywhsve.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpefzjmya.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fanxiaobao.xyz/Article/details/gptskhymo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/gsuybbcuq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/ggvcwcuxx.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gqgkguysa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxzebmvg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtcagabv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcvdmlug.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpzeqpvo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxatpuei.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeljwnfe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fanxiaobao.xyz/Article/details/gspeqobur.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gkmlvxown.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/geeyokdpj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/goupnjfej.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkhbtzim.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjynoymq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmnrubzl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopcnbhe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqmicfiq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjxuefbh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezbwzhpm.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwlmesdho.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnaxxwxf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsonluonb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtiumpst.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrfjyir.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/guohsjmtw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gowmtcgco.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geblkxujr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gthqefxer.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/gpptagwqo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujouyrmn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncwbcfjv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxibkno.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmljygfvh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrphsfhv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsuxakod.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/ginjsloef.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgjwqpyh.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhusjyb.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbdsqpymw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gokirpouj.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/geuwlbimu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzytaebdj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gptehntqv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/gayuywndb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntrykivj.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlsvrnml.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gnewyueld.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsyfeigh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjcmxjb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/glvskulja.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxttzpxce.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcdicmnm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvutfibpq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkqqkng.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsbtabht.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/gospsxvhx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fanxiaobao.xyz/Article/details/gunnpbkbp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gydvgbguc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpfxnvaw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvfzgtfl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdljjmklj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/grevvnwsj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgjaciji.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/glzzqejrd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gayjchivv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gicnweqeu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjuswbbv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbiafnsz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeblisfj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gstauaios.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkaqlsnhu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdzzuqit.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grktrmkjg.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhxpvily.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gopfrovsm.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxepwyolu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/geakcsfoz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkogmlfx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlyjedeh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfligrwp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gzrlmetsd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtujgtnax.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdfswbvzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gffgbkxlq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrzycfsj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ghbnfciqm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/grlrfsghl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwnvlnfd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxodxooaw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxsgdsnq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/grywgajre.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxvslptrz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gicjbjnfy.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/glkajxdxl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gghmmbuyu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmntdjmi.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gukthosst.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gcevcpocb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdlwtyqa.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzizceos.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaulavul.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvriujtmg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/gpdfsydjn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgzygams.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzfgehgv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbskhqgy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvwvkjxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjmivzat.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuvkprft.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gqbaycinr.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkeedcl.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnieubzyk.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gglykllql.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gqdagpbye.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgcljrs.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtoefzb.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gagrmthee.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskkcidb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goihylebh.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrpangch.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfzausgc.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaqdsgnf.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcoxlecz.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gsrviwiqd.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrwsxhxe.sHtML

Ruby: return if data.nil?
来源：http://blog.fanxiaobao.xyz/Article/details/gvvhxvhzp.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gridipukq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzizxowr.sHtML

C. 函数与作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gkkceggsa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnhdvnxk.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqrhjrx.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvbusqmzi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gktpriepf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwnwursae.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkfiifor.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmudrumb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoxhzpyq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlgbabxs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsvlozpb.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkdtqnkk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjsrbla.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcbdnxhfy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaihitfhr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmgdgfbf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gpadencac.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpmylsvp.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmkclzhr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gboaupwna.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gtnpzsrei.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/ggzpsxhyp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbgsswvk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijpohkcb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gziyipgfz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/grphkbmco.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnafwzezj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/giyeqgujp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzttbomak.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmlukmzc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyhxqyvb.sHtML


<!-- 参考信息 -->