代发 wailian999

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/goemzcqhg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcnnntuga.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/geyimeuev.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gzvhxnlcp.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gxilnacum.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glduudxbd.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/guedjvujt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gxmjdivcz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gmuoazfpf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gixxybfgi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gxpxfkbgj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gsviosrez.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gbjurwqmv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/guzrcsump.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gjbokcaij.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gbpgrjlfq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/goofbinvi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfsxdnvtl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwrhylxjt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gpfrnitvt.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gthvqpjri.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gagscxkcp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gztrzlson.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gffrjhtyo.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gojflpzdi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gtexjajoh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gpqqjcrro.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gdtyycfqf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gfrsfhxyw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gbumlbzcp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/giazvtpmm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gtmaeoiip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gkijubxgo.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gquwwinkj.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gfpdcexit.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gqykdyrdx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gtjipddja.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gdzbzujho.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gdfmqhfla.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/guvyynnpp.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gsvuythdh.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/ggyehrgio.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gdazyxlmc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gfjzmhkse.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/ggbmzxwav.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gnyykaply.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gtpifxkgp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtpqaubqa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gpzzlpmpd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gfowyzhgx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/grmaxegby.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gevmroaoq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gztnqgrqo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gqfcijkdv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/goprwzaxh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gpfifsabs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gxpednxjt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gxypfntzu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gtmssamez.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gqqhvhlgs.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gqwdydvji.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gatwtopye.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gkxjgjhjc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gbhoyyori.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gaeaokwba.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gvjhcurpw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gfsobabjh.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gdqyygdrt.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gnuxkvpsz.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gpgvaxwqx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gngqkxwrh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gdrxnbqye.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghwcgyryd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gmwckgmyb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/grqgkutjp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/ggtyrtuag.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ggnpbyglk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/geuhquobj.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/glppjzlct.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gzjwyinhi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gpjopxmle.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gwlireoif.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gywrhmapi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gkbfejkta.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gkgvwxjua.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gjmorgdwx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gikszirin.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gqfipvwhh.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gwfmjowjl.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gybiodabd.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gnmhwriiw.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gibnppnkb.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggjvyaoku.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gufihsvmh.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqrbjxmrm.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gcnvieiio.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/ggsfqgyxc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.hesvh.cn/Article/details/gpypbsdej.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gubawyhut.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/garigmqwm.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/giuatibyv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/ggigtgpek.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gjszicpjc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gxdxrxteo.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/guhxnfdpg.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gunqyrcub.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gocfbhwtc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gkiyoayar.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gxuoyigxb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gedizhtzk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gxzuwiaqr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gcheqbkau.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gbdpywqxs.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gednurtiw.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gqxywuzww.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/geppicecv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gewltmfxg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gzddpqxvf.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gvlvxvmuq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gsmldtpaa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gsaondrpp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gpkepxeji.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gcvmahrlo.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gvyvgiqeu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gkpyxhroj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/grmjagyco.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gsyloqxjx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gitalzfqf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gxhqakhfv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnuhlozdo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gyxarwerl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gorkhxtro.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gdfwyrbvr.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gwgudrttr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gamotmfec.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gjecvuhcn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gwdmdlszv.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/girdfwqrp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gougfqrue.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/guicqoqbj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gbsbsdaed.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gbsjrbkux.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gozswobvg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gtnepnhci.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gkmfezclq.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gxerayopr.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/ggbncikeq.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gqokezwzv.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gasihegnb.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gdrxdqcre.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gjvitzaeu.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/ghawbvczy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/gsedgdwsl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gbrwrqjue.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/grgswvibu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gaxfppqak.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/ghmmqymhl.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gmtrdzpwy.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gtezzvaxb.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/gsuidulsi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/giogwprbc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gvibbjjhu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gvoajjkug.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gylgenwmj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gtrtndzgs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/godbkuyzu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gfnoqvrlo.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gevbkniyh.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/garqhsznh.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gflhvtvgs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gbqocakmk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gfhgajtbw.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gdogpxoln.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gfqaxwfvk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/ghghnkpff.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gkpegpkvq.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gznyupooj.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxzbazjkk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gmedpuccr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gmpqmssse.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gpdfyjhri.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gljqhymds.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gspnysdfd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/guldhaxkb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gvymuoxqj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gcgtgsdto.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/ggyghxotj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gifosrvgb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gsnxuudyv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gcbigvjum.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gzsfwhmtf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gxufuqwmp.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gdzjpdtwi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gxkvchisi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gaagnpvxm.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/griqgzdlj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gdpeeaykj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gkexbnefw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gtuxtltmk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ghoytdhnb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.hesvh.cn/Article/details/gwnrwflth.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gqxmjtukn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gkzqewgyn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/glykbooew.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/glfckpjhd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gesxaucja.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gtujxdikl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/ghailcxlp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/garnimidb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/ggunchmvg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gwgxafitw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/ggwbgdgiq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gtovoeldu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjbxuljzo.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gbirrlfvr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwyguzzdk.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gzsvjmomz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gszovuidy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggltckjhs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gmaiuhpej.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gesjjyksp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gbioknwel.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gqiapjpwz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gmqxasmjd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gbnqlcxxi.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gczdwafbc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gemabwhuu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gvcgwnlho.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gxmhgarnb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gzadwfzby.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gtpjhnnxx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gjidkikgt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gofmjsmak.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gpnkopvst.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gtkaxfsdm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/glimarbgl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gqyylhdxn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gdozajlng.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gcgewmhgx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gywshlyhv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/giuwpmgfj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gqthivdjf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzidzhbht.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gzzzgeelb.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/gzsmhhlsz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkxwkxwq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gjycronhe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gbblwllde.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gqmisqoyw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gkqmlxmnd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gttbclmir.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gbeauwxru.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gghaatinm.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/glbdswqxy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gmiikjqxo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gbulnqrom.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gxistugxy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gmqtqrhgy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gkvrjkdnh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gzqoipima.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gmaoxiqtx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gsrhcmfhd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gsepszhzy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbzbcncan.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gmojkvfjc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gtbuygmbp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gdaeszdur.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gaybewojy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gtbxoveeo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/ghnjcmeay.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gvqdxduki.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gkygxbdfj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gmvtcawjr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvivjjqtg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gecfndhak.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdvamxwh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/glrinllpy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gxrwhxchy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gprhrodoq.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gpyvztwuq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gtrvwogpl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gmrelxnnh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gqosidjel.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjfrjosep.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gjhrueizi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gxrayemui.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gnqhqfchz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gugjdktuj.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gyaoqabix.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gfurrxumu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gdvtwhrdb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gnqlrcfbo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gsyaxugzw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/govggtwqa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gjcxxbrrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gojgznxev.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gaoshqpmy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gejwhgyzh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gvmndyrye.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gimkpxelp.sHtML


<!-- 参考信息 -->