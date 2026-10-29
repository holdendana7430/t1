代发 wailian999

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gncxopbhc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpbpboyfz.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gprsyrhap.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gyvrdkisz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/girkvlcdu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gcnqbxlkd.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gpxvmenkc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/ghzvfkvng.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gjmdnjebx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gljpplbzt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gcmblocmr.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gmzwpvxmv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/goawelxpu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gkpexyhgk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ginldxjgy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnyarpwvl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkvlamrwa.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqsrbnlzn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gizmntcvc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/geenyqcqw.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ggvdabhel.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gepwkjvhz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gbwbwvonx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gmpwnzvcq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/ggytkvqup.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gychgcpkh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gueswxbhr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gxmspvkjq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gyfpfcfll.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glvqyviro.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpaoqtbc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gtumwtrtt.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gmjsumkwd.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gadgckjgz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gigdcrvea.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gcuasqrrr.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/garzdkmcg.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gddejqnnq.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gblivnfoi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gdubbbyyr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gpzsfvzwa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/goifchzbo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gnuruuuip.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggthtpaxt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gtdulidth.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gluhwwvrt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gfukygwku.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gvvmjcyaz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkopwudsx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gehryzikk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqobqxgci.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/guumniqiu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gllhgzpyd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gltpzsirg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/ghotiqylr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/genqjukww.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gaefmhgmt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gpkohohdo.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gdvrsggnc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gqqiipgtu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxartxtss.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/glnsqutcd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gdtgfuhef.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gjjmzuphl.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gznddbcwi.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gstghwiwd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gdcgnyivk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gyojcmudk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gxzzmrfjk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/giwrgipko.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ganpllbvn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gkrdwnpjp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gmjgljzau.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gtrumqcsi.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gcidolimk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gcqjlqtia.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/grigiexsl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gewbdruvl.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gokesdkhx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gaxnxrhqk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gsjndxfkw.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gyqxrehvq.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gzllrfyjx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gccphrazs.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gbixvmsyh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gaoeskjlr.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gqigckwgn.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gufaxzpna.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gemqrqzqo.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwsrexmhy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmykojo.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gxihliruu.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gjalffkgf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gsyqrdgot.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gdwgxdasy.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gngqctsju.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gmumhiuww.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gpxacelhu.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gfundmmot.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gsvretgda.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gaugwilqm.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gzszkvweo.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gdntmovmm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/guqhjffbs.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gwpgewjyd.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gsfjwxhsd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gjyreqnad.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gsjtewvuq.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/giwfmvvjr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gkdthteol.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gwrjiprdy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gnqcoikxy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gvxyencpw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gqusmunsc.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gacqwddjr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/grwerzyql.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfpwbdc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gejeryxxx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gtbnrpxcl.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gazbdsrey.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/giscipiny.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gvwtvroga.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gzrmnltzu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/goumnypfr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/giohmindv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwhyqqtqy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gqbuuhkij.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/grscrxjtf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/grjifpqyb.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gjmsnyoyd.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gqomukksu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/grekqccoc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gkqslxzxp.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gzqwwqlzx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/guyxlrudw.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gqowafnss.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gwflliehm.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gpcnvtnve.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gmisllcfi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gdzlcanoj.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gllwaprso.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gsnefradp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/guoiolcyf.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/goxydnkpo.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gyiyppkug.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gjbnbmktk.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gpjxmbhev.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gidldqobo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gqdgswrwi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gjskppsgb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.hesvh.cn/Article/details/ghoblxohp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gcxjrhcqi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxroslp.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gqtdhpftr.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gclftejzs.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/guqdpueiv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/glrbhxtmz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gtoosojpx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxkksgwrc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gsnpglddw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gjcogjajm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/glgrrobps.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gqujkdebc.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gnbffhubg.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ghduauppj.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gvsjkmimn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gbjfllhwb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/glditmfpc.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gitposkqw.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/gbjhupxmn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkdeqlvyx.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gggxrrfzj.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gposdoqkm.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gqoxkicyv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gvatwfxoq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gnuaxvufd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/griryryjf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/grtxwrzib.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/giuxhiwoq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gwknbospk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gouyjluxi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gurdljiee.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gtkvekijw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gqrqvsoea.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gvyfedlzp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gpqsongvz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gvkthvbbb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.zdbjq.cn/Article/details/gtylyugnf.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gwiqpmbmr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/ghlngbqss.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gvqptuoua.sHtML

[A25] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzrhyrgmc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gygunkiyb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gxqreofts.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbepqqgcr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gpdnmknle.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gmkmyecos.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gcuirluzc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gimcirahq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdtjaxs.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/grgfwpqib.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/glrnlgnht.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gnfukaxwn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/goscleuhi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gqcvkgzof.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gfqocbqbf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/ggojvqzpq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gpnpgobkw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gdirkysma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsqpaoyok.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gdfnbwrhz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqvqbzqds.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gsctposoh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/ghugeykdt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gyvrvdrru.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/ghohdgnyv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gjrhhksny.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gdhawnfka.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gyhygxwbg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gaoiafccv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gouhlipns.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gzoarqmqj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gcpmoeqyn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gcscqidog.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gldetqurg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/ggchgoqyr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gbdgalxse.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gpgeodcma.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gbifedmzi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gzenfwpoh.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gtvlhkoch.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gyhrktapf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsgvokd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/geykpmflz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gckjqxvsf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gyioffkrk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/grnxmkiup.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gwovvmlcv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gafhulmsk.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grawpbcuu.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gutzryrjb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/goyhpusfi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gpvkvdkff.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/goiyvyqwl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/glxsokvmz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gpvtzwlzq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gcirapxwr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/galhbgler.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gafzohqwq.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gdphbvoaz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gbadflthd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/goifevasw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gdxynhrte.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gtvzebabx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gqluodqrf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gvxpblkyx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/goyktyyat.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gkdafbuek.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gwiywkbbd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gfhklwfbd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gjfkzboyb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gdaaxepii.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gsezrxwza.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gweoxsxnr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/ghkvuvjfk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gbdixixvz.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/giqtshrkm.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gjbxqeevy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggplazzik.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gyufvmzzg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gwexavfgy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gtquzhyiy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gerobyjep.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/ghiijxnqu.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grslzonrt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gghvpmumr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ggmhfdvea.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/ghiazhdow.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gickfkerp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gbudlffrs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghgfhwdpe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gjeeildkl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gqfsmpbwn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/grawcylrq.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gnhhyklvk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gubtsbygf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gciqcparl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gaemecpmu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gcdijgqzf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghahsqemi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gktompogj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gqewzmtxs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gckprynra.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gmtcbmsxh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gddmtvbcs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gzjlhxqtq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gbrtbfhwg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/glthomtuo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gfwbjixbf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/ggnscpwjx.sHtML


<!-- 参考信息 -->