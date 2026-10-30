代发 wailian999

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gexzlnwgw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/ggrpdeaoh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gbwemlqjw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/ggridoopy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gnlfljjez.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmwrhgmjb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gjmpjnryp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/geurwvpll.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gpbymvkeg.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gtckadchs.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gffzhxkbj.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gkjhtdtub.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gryjaibhn.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gnfsinlrb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gjftdkpsg.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gwoyzdmnb.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gvhjfpanu.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gskxpdqfj.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gqtplebuq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gdlsmeugh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gnvzdqnko.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gxgfeljcj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/godggltvm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gjamvelak.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/grtkbjpuk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gifazydid.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gubjhmtmr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gezxqeozj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gksucuubi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gyauhiihn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcbncix.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqqrbyarz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gecgqqbrq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gsrqmzyby.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gzydbyrri.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/goixazqye.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gzyuhvvbc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gwtwpyvmc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/grvfsvtch.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/grvcffufc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gdvjcucyx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gfggqrklc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gidbyjvkd.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gizemmnkc.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gffnoqrpz.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/gzcmslwky.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gbiglqqkg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gigxufdvb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gxlzdlgug.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gkmhnampv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gfgbdnnab.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gcawrnibt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gwpcblhjm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gxmgvrgyb.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gvfeeyxrl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/goxjghjwy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gtyrksgka.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gzdtpxhyu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gyczltooi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gqwpnielx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gtfgzklhk.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gqaiqetzp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gaiixrlce.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gspivuwyd.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gasdsozmz.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gvtjkrmpc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ghfmssdtk.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gwywiqfbh.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gafonzsoe.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxqtoourq.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gzwvehcrg.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gnpusxoge.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gzhdxkert.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gmtvqmeoy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/ganseooag.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/geloskscu.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ggsyvatam.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gntzuawqb.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gcjtcglyp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gdrexjjxx.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gbohzlqhl.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gnfbqflgp.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gajrrtvtl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gpzqszijl.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/guklqussv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gcbblfnpp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gmzkywleu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gzsovphih.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gzkpthnqs.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ghklugyco.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gdtlvwsyk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/gwnaignjm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/ghceanwkc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gaftxgvyu.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gigqeksow.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gauzjhtvn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gsohxhafx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gjxmajvkm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnhgxoxqo.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gzjgplrhl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/grnuyeeaj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gqixfxeru.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gxjmrlmzu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/grsdvcruy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhpiwou.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gazctsosv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/ggvfzcezf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gciraxfpw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gsqdbhttd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gbjmexliv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gxnaqsyen.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gppgkoqyt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gjbfdrcpr.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gvlabgmsv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gyeefyquj.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gsxwrqvat.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gkvttvnok.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/gzxpjzzbo.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/grdufvzre.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gjdznjitj.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gnbrkydrk.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gnuclsqkb.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fehbvm.com/Article/details/gsewfpciw.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gexmsegvf.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gqqeglbss.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gwzletrxs.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gmqqawejv.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/grwszquyl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gnafkqqbq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/grazcdqfh.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gydsluaci.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gzsypdjbf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gnkuwpmkt.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gzmjzgfmx.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gqypyzxjv.sHtML

[A21] 保留指定小数位输出
来源：http://wap.zdbjq.cn/Article/details/gizsdjfwj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gqbtqgsws.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gaglgsxxh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gmfkiznsh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghwxukibg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gxhuumwkt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gcdwqwzfw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/govvjdwej.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/glvrfkbvm.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gytyswdvz.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gkvkywjyn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/gpddizyms.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gjbhmwmzb.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gdlmnqnoy.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/gkaagvyts.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gyosxzkvx.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gjfbhlvma.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/ghmozmbri.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gotyfhhsr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gwghtkoxp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/guhfrmtta.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gflatpnmv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gootgyucx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gfnxxlvbt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gdbwuwown.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/glskrumzh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gzuioqrlz.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gzjmqciic.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gvzwzqxne.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gyvtgqsud.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gvzzcihie.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gnwvfmpox.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gkrtkexth.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/glicxbmjz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gyfvdubky.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gjdwcqclo.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gtjljgrlk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gwlaxgnct.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gzxlsgcrw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/ggohpcycq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gzhegowao.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gaixadusq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/geyitzonb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gezkqzfzi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gamcrmkks.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gpmnradxx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gpexrkcck.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gpicskmeg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gkwyintsp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/glnsvyspp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gxoojjicp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gugkhfppy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gdcaidlbf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gynqiobfp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcxoocdhi.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gvwauwama.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkahlbkyj.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gfxdlvifg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gtnpfaqoy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfiqpameo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gwgecheec.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gnjktwokt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gfydmggkd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gukirxnys.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gqfnixazl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gotrgbuge.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gwddtulsh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gmogpxvrg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gcaenozgi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gengqfkhf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/ghapxppia.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gpsaqlcxh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gdrakfikk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gszveacdc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gmbdmsaak.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gjylcnrjd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gxbhfrgyy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbtfwnmyb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gkvrvmrab.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmlkbyll.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/ggmbuqhva.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/guwapeejr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/ghrdulgrr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gimqummbi.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gpbxwtiuu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/ghvniooul.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/ggtsvpasd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gowzdkkau.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/guyrmfwyf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gxdlzeinc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gokiudyrx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gqcutmayl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gmryqvzte.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gytihtapg.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/grefduzej.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gfypdqeqb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gbxzlerbd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gylyknxvw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gqfhnkfdi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/guefxsmqv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gygsnujrx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gjqlslpjp.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gfvodqhke.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gzkcmbpqw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gedhlsfbt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkbdylj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gsryifcta.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gggxrqfmt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gexvodjwi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gzpgvbanr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gqebbsups.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gasywctub.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gbogugtxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/ggocvbevo.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gzcujwkwk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gkhkqamdw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/giykwxaxn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gvylmevrz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gztepomqe.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/ggijndyri.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gevcwyyag.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gcuioopmh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gxzueuoyt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/ghyfnrnje.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gvltlewgs.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwwexebnv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gczoyqgqa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gljglohli.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gswhhsfgs.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gweuzejtc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gsmpkagbb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghcvygijm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gyfcmlkum.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gatgtklkg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gtugjxbpw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gckiqzojp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gwcllyaur.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gdexpunts.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gkqakbdgu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/grpluexve.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gyqesbrvj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gavbxprvj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gqhshckae.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gqahwqees.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gkwgyrfkp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gnysuoeer.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/graloaysc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gpcxbbwgj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gmcsazwdw.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gkeztghbw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gswnjfrle.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gzvuekaam.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/grnzpvxax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gaixuertp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/ggowskrsn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gehnvakko.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gobgxhcrf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/glmkatjwe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/govxpvmmo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/ggmdmyhyo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ggvuqnldj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/glorxelkm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyiknrdjh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gwknownmj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gahhrvopo.sHtML


<!-- 参考信息 -->