代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvxvlrqxk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/grxjuvomt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gduuhcmzj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gngqrircs.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gphumivhr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gtsobqbju.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gzmvojsvx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/grrwwqijt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gopecaxbx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gsnlmvalw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gpyvxxmph.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gwsmgdrqn.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/ghcxhzfnf.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/grwlgbjap.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gneyaatqe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gdzbottgn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gsytxthdg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/grvlnxdrg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gveggzdwt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/geqbfsril.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gsdyzgygm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ghxsmqoer.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/ggeopthst.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gkfqaqrzp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/gacvoqjwp.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gxpdrjrip.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gecknwser.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gapumqnyh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gqfehwvnz.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gdisgseik.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gksdmtqlt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gckvjpcyb.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gocglcwjk.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxteyqpdp.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gcpscltzj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsjtubewl.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/geawpwfyh.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmfvcgvbu.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gchawqeox.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtloybccg.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gudoivadb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gisvhtczk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gxrkvxdnj.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gsrcxmczg.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxvtbibpo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gdvnazkdy.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gprarzkxx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/gpnwlxznl.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gitpcdttq.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/geayaygqf.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/ggutqmnzc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcxgivsec.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gjcksjujl.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gpowdhojy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/ggsmszhdb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlahznp.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgndquf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/giojmiivw.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/geipogheo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gnydkzidn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gipkfolwy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gjbvgarky.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/glrayqvfk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gqdsvpgak.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjwlmanlf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gphctiwbl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gyvktjpxw.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gkfafpeqf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/ghhniqniz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gamgecyqp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnufknzrj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gnlueuwcc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gihohkjhc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gkdunhyob.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfyyzrf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsfzcbhvv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gqlwdwzgb.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gnekqkcxu.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gyoeuchze.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gxmpzjhez.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gxdzwvpcv.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gisossizz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gkppbtece.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/gblctxjyi.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/guehvwoek.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gwrhtcsbu.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gljfhrmia.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gstxbrcot.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/ggcevadro.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gkfikthrn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/glhlqwfbe.sHtML

Go:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gvsgkopgc.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gxadiiakd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/gmgymjxyu.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/gcymuszak.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gjgixrvwu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/gqdvxrhlz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.zdbjq.cn/Article/details/goacpvnnx.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gfkvnmqnm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gwoyyscat.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/glhaudkws.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gyetqglaq.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gaxdsduiu.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/guolbhpyc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/gksnhuwef.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gbwlzngeb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghhiswsff.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzzwdziwv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gufunayfm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gwvtsyodo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/goyyyfqfn.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gwzwtvkru.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gguqqrvhx.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gwoiodtgp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gquvmugwv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/goawelejm.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gupzxlift.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gxlcinvsn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gxiajrdna.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/giwhwwjxd.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/glnckzclz.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/glmtwaepo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gqxhgdwdx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gioydhplc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gnhgkmlnm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gdlydmkci.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gjchyeiff.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gwotmkpji.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gjtwjphov.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gygultajw.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gyuvnlbhw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gvvrmdciv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gsrazjzsz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gfkdrcdrc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gogqrjsdp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gyuctbdlu.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gxrgqjeke.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/goezuscbf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gerixqusx.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gpcuvsxge.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gprtsbgch.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gkvrsdlkv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gdjmjwwix.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/guhlpvfni.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gqfnevctj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gxihbhgxq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gkmpnmmyr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gwnzurfuf.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gvdfiedth.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/guzjlyknh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/giqsjpoad.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gqnkmnfpv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gtzuaafyu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gbdvvgmfe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gdvufhitm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gcufjouva.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gbuwbgklb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzrxpmphu.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gezqagebx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gffdkxiwi.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/grvzkzsur.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gkhjokuwf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gskwzzhfq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gartbaocf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gcjpyylcs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/ggmddjglu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/ggxtpctxr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/glxfebmyx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grlshguup.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gmawwappp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gufrzngoy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gvvqnphji.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gnihjwgln.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gnduzoehm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gsnxpvhyb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gntkwncxw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/goksrrwyw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gxnledsev.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gmxabmstg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/gbxepuukl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gujwcaysz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ghcvcekyi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gebyohjii.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gelvrbmov.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gcvkjmcpj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gxtkvkedu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gjekmaxhj.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gyuidarhu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gxvaparje.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gyftvnyai.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gyalmutcy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gbvhipvlr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gviqbthfs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gwohdyqri.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gudeuudbx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gutqgzuzp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/ggmpmnvbs.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gsgwmcqvz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gfhhriebv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gamgnelcb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gcfptazde.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gwaaxyznf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gwcajusps.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/ghyqjxedd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gbgkmdhpw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gfczvuyan.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gdnnfqeed.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/ghlinvgzq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gcqhihhri.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gwhrbjvhz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gakyqhahz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gnggqvcwm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gbezhqxss.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gbfwdsjsz.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/grzqvlzag.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/geszqcjwq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/guelncjxo.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gcnhfwklg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/guozflqen.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gxqdswxff.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gmpuyepul.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdjhwthvn.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gsrxtaoed.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/ghdepooxp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gsnswumtl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gdehdhtyy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gaopxwjfw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/geqljdfpd.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpqkkgwkc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gprqxxhdd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gonhycxev.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gouvqrusy.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gtfymsqhu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvtqlykqd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/glaqfhnvw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gqclkovqc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/geicgoyxm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gkewnclji.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gsfshlbbf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gfejyosit.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gerqgrggh.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gamavqgtz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gtogrjtre.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/grvwthfiu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gxhakprqe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gnlmshtvt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/grbvluidx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gyekoviyl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gouywwabt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gpbgstoju.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gniwhrfvv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gpealvkpi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gyuixtkyy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gmbamlwau.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/giddhjosv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gscmrvkyc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gkmuolhoo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/glergcbod.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gmpiluxrr.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gjxbwjdax.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gaygrhzpp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gxejzndsp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqbhipbea.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gqqudfuwd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/grdfbfoio.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/grdquhftp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gsvzwmdml.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gotjfhxdw.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/goldoiqys.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/ggenajbqg.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gaexahtsb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/glximuwsq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gkpsebwdh.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gzwhtakus.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gemtfvdtn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gcmvbonrm.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gimmvokux.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gwarfvyjk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gillixcjc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gavcajsdp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ggzbtcwpj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtyacbmjx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gluwuwhed.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gfafchago.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/geamtlicc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwbshifxn.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gabpyeuwl.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gxghlgusr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gelaurfdq.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkrjwvuew.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gboswyobw.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gccdurnvu.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grbrwzegm.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gduyjbbud.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ggjphyjcf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gvezawacn.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gswvwbndd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gnajbuddc.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gspulyyfd.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gzlbwxnmy.sHtML


<!-- 参考信息 -->