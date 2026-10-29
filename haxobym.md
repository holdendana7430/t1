代发 wailian999

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/ghtkujkvb.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/ggapynurz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gkgtqnqnr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/glsanfqjj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/ghyvknmnb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gucrvhbam.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gjjbswwkq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/grblmcxik.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gfeayyvcj.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gouzebofc.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gaixnfajv.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gwdgvsndo.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gipdtwgux.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/glmtobhnp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gbeksfkop.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gnhyxoiqb.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gmurdmarj.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gjjuluqfv.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gynycrkup.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdbimyrlg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gmrkbtuit.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gogiolvzn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gxulpqspm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmmytmjuf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gfncpkayj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gmwyicghv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpfevrxdx.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjshfdjxe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gkyvtqvmg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqqqidraz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gktvjwukr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gclqldtor.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnoaqnsgi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gradbzlnf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gzodcgtts.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwlzhdrms.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gqrncpuqq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gcanowtjn.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gxcdxyxyi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/grjrjwzew.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/giokwdadi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gexpmxwaz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gaphgilee.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gpqwobijd.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gnulmfgwv.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gvuuotjrl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gpbyujkky.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gqwgeonlt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/glovrqmpt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gkwfdslgn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gqqeaoiiu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gpvlypcfi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gnrbmvufe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/guuwndpao.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gufrgxlct.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gouanhpae.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gievchwts.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gfqzbpwvg.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gegtgnujw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gbvskbcld.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gopvoatfv.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gxysudzfe.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gacoijctq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gkonmlzws.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/ggqfjtpfx.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqmllomhq.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gexbulnze.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gbzwxuiii.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzdiviamn.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gyassnhra.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/glfdpgllm.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gctmtvjuy.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gobcydnko.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gjvnrqydm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gbdtjfsuq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gkuxzqnos.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gcpqgxxrd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gcxenwggg.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gaihbyeia.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gobzsnfto.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gjtpcjszz.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gbwyepwpf.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gnufmadpa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gojtlhevb.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gjmawmzos.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/giorswlml.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/geebukvyq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gzcwcoodr.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gamlulzfe.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gkqixulke.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gmmhrblez.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gqtapdmdo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gbbfmtuwd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gfcetihqj.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gpcehfvcm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gihhasdqb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gebukpuer.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/govftlyjd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkaarpzrw.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gkemlbfve.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gdtatrckf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gxhoxynhf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gnuaoktcm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gblaxwsnt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/grflompev.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/giwrzazsv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gwnaiwbsw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/glaafvulq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/glxykaavx.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gghjqjody.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gwzvioyoi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/ghdgyocyb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gadvfwmeg.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gssgptvaj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/goqkbsrds.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/glqkhcjch.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/ghryxkvze.sHtML

[A19] 交换两个变量
来源：http://www.share.fehbvm.com/Article/details/gwhbelnkd.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gjeqxszbc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/givygcwqs.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gidwqbmzx.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gnmmmefib.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gvfffiuqq.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gegvzbmqj.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gpeyrwvqp.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gedzhtbqr.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gkdxgcqqh.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/geepxmdhi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gnxlljgtz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gnpbythhj.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gykfuwzgh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gwieznozp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gtdpblrlv.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gucyjpsyk.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gadoxhbun.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gwnjwdyub.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gxaupypxy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/garcfghvr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwtsdduxw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gfshlqxro.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/ggpaxyjup.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ghaawtlbn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gdbloqohw.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gongyyenu.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmpdziovc.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gmxabmyra.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/glmboyutu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gghjycbid.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/gvemdeoee.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gukcvyfpe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gericufpq.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gvxahdyul.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gklxctljx.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdrhgmbtp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gugfewwqj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gcptmvtst.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/grktonwjg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gchjmbffu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gfsocbtyq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghxtgdeig.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gvltzlftw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/geydbtmdg.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gamsyiqja.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gojgwikcn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gtbdbttfc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gubaqzkdd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gnspdqnzm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gthkcrylp.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gutapnqlb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/ghelvzqnx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gmyvcxmwa.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gogdtvivt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gaswbmdrr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gprphgwil.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gfeojbptx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gyinpucfk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gnwuwoqlz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/grljchbxa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gnunqwxdh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gxujrqbck.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gbaazeome.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/glsptksln.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/ghhwdlilr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/giourqlry.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gmpvlcuke.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gbrdtwoev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gvzjquvxw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gkboqiirp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/ggvgspdui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzysrwgif.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gncfwkujn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geyzrcnch.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gewccprey.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/ghwvwyqhj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/getzuhljk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gnyjtfzry.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gzapzedci.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gyzhuymjr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gtqrmfgtu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gvrpcyfbd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/geqjfogsi.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gvhkfvggw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gpeaivtjf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gttynqjvj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/ghlsknrea.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gnpgyxpsb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gzzwtuxyk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/guqweqxzi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/grgxkcprc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gsdfojtjb.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/ghmquyklz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gmybbpavh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gwwfcewri.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkelzhiec.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gwsenmbph.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gteqbfsmw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gncfbycod.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/ggfyvqwha.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gzdibbokt.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gcxvniumn.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gnzjzcgux.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gafzcysnq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gzlnsfvyp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gdhrgftqi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gnylxtcne.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/glxkbxhng.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/ghebdnbsc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gzeworiku.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggmsiwwae.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/glscmdftz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gimdjyqdp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gmnwttzhl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/giaslrmdm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gihrqmebp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/glvmuwety.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gpqwuqxrd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gtmturcdu.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gorsatbks.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gpiqsinlg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gwrydzrct.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gnyhocqft.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/grhxhrjph.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gkmluudxu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gxynnxtda.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gewcoewha.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gtmsjsrbz.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gkgrjguom.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gyxseytzq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gpnbvijpe.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gilfkyfsz.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gblhjrnff.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gdgaknpfg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gpltyrwig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gndmghrmq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gwnfteqgs.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gsoxdcwwi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/ghzzfetgl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/grrbzalzc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gwfusqcps.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/grzhtfykd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/goqkjccnd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gkuyjheel.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gypgdawfp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gljtledmp.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/giqhehewc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/guaevkizr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/greganzlj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gciemyxql.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gezbggwfz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giuvjrlxr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/grlctfpgm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gpwhpfkkb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grofbeemo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gxnhkgzrs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gbmignwas.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gdfcmvkhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gjwuqlxab.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gbsykqdgv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gregnodpu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gwjhvyfpd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gbkkusett.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/glmdmxmyo.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gbpoqwhlw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gqejandpd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gnmexprvv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gechsejfc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gtjmilsbz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gclwqnoad.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gpnobeiqt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gyrcwtspb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gktbjwmfx.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gnmdcgtah.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gfinbppfm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gfcrrsbrz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gvhlgajey.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gtgmkmaqo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqcxgwnxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gnnhetfvr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gvuhsoowj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gjftiaooh.sHtML


<!-- 参考信息 -->