代发 wailian999

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gmjawgqxk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdctglxvd.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gfhuxrjmj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gojpceeie.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gtuyxpdgh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gndiiedoh.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gexelibxy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gaekftmaw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gfcnxkoys.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gdanlzfsb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/guqkhmpha.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gycqmaxsy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/giyaxszdu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gncdjqing.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gnulkjhvy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gnigjkifv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcpuwyjwy.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gtqburnri.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gllombfqx.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grbsbcyvg.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpgbptizj.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gnvqdldbp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gxoiugmpv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gzrllbkfo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gccaazmet.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gcwsaabin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gkitpurwj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/grgzmnfua.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gzpvrgabg.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gykbkrczp.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gosetyfgo.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gqqmflbya.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gjxdxpwhc.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gcboomenp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gnqcnmlas.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/grejoleuf.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/ggpnhbapw.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvtekndri.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gjywkasum.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gpjedryxm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gudeillxc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gozrpngnw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gnxakxwwu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/guiwfuxbm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghmromkgm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gdfncatcd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gqvmkioep.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gjnjpghyd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gybctkyqi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gfdpdbvtv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpeonwofr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmlgsoter.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbswyvwyp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gdfifnxjx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gshwqztdr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/grjnjoqpv.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gfzfoiahs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gxgzcftxf.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gxebppbve.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gtjljsjud.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/glefslioe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gkirtliof.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gczmcnylw.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gqduegzrd.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/greqzsqml.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gopcsvclr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gmasradub.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/giohkwggc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/geanykkpt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/goleypmmi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gahkttumg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gsyaqayqp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/galryeqcg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/geokcrpga.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gnczvqulz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gftubqlaz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gzddiyyda.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gyxldwbvs.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gygqwaxvi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gwoqmkjcw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/glcucatea.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gbxxqhjka.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gesnhnioo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gfodtxhdw.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gaphdvxht.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gtpmccfjr.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/ghnbnqrjm.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gdyjxddcc.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gnftgosvy.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gfcfoaspr.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gomtwtfjx.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gfqiddlkv.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/glmpoihbs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gdpvhorly.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gsgafbhsx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gxsroitxp.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gsnbxloju.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gvhxtpjjq.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gdsmsdlqr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gtnkngiwj.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ghrxrppcw.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gcugdthga.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gvoyyqitp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gfjeopgwg.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/golznosdf.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gkzrdxely.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gilqqubsr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gwliyrtob.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/glutdvohj.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gtqsofalp.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gpcujiner.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gzcijctkk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gfjbrxxdg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gxdwsyvuo.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gcvprfjwb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gnhcowlnm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gjcuoukuy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/gzsbyiwug.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/gdwvaugbk.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gurjnohwl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gylxvdekc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gpldmuosz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gyaeeeuky.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/garfurrmu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gukdkxtye.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gfxlzfhob.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gwkfubywi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdncgjchy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gtkkvbexh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/guxangrkl.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/grotrubpi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqrexszx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/ghylebbsp.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/gpwwndfsv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/grhzspcjf.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/ggiihtdvt.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gbyzyqcie.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/ghegokmor.sHtML

Py:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gbwluqegr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.zdbjq.cn/Article/details/gafbuwmzo.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gaykcmbpi.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gwfuuaopf.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/gwljovhom.sHtML

Go:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gpxxtexsr.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gssrpqhew.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gtqkeekhh.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gqnamfdlm.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpynerjf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gavvctfkm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/gqnsaqgvy.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gyttmigxd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gcelwvhzn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gyfsawwvt.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gxgakbmgm.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/gadzlybgy.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gjrpxwuyb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/gjbwolwyj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzimcqdbc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gbelwremg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkdkhnfiq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gxehvmsmp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gnojndhgp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/glddjalrp.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/glpfieavk.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gyezsdgfn.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/glskerfad.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gdzqnbvju.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/ggymzjkye.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gbxrbtaio.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gmxlbuodg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/ggqidyttj.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqkbuwfyn.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gmdhsdsfm.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gfewxdour.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gawzuoebj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/gswcjeliu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gvvznyusl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gpoxopajb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gojwpilmq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gazsjzwxn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gxjlthfsc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gqrhdpulz.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/ggxnqabpn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gbghtqllp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/ggaxoaxac.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gombftuuw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gyhmzjubb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gpcgritzp.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/glxkcivdy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gvhdeytcd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gdfoorvkh.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gnakdagkl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gxbxcqvxt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gdfxltupc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtptctbln.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gavtbrlhm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gkncuievg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gpvkzpstq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/ghtwuywpl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gmzbxxmil.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/geumerzkk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/geuhlzkzv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gnjwiklgo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gbqochild.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gminxqlky.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gnqqzogmb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gsyxtbvjv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gxzoigjbv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gnvsyxois.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxevlxoxc.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/grbvfujik.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbihevokk.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gwlhojacq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gkggxdeng.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gfbxebplg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gpaqhxrdv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gatoftpjb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gjbglhdpf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gqhfwzccj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gkbuaieqd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/goxoxpixa.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gzubxrvzt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gzumjpfqc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gxqasbfkf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gafbcakdy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/genekfowt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/getfewine.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gudjlfxlx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gdavyzoio.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gpxvnnpsh.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gjyoizxve.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gvbvdyhte.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gbxvaxbvs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/glqrhfiia.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/grhpjmjtc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/geztdkmgk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gjrfhczpx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gkgqfwokz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/godhbgdcf.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gawjgzhwx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gyselzpqt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gvdfbpbil.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gfzobwquq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/golchkoaw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gewtwbiam.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gleevffhl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gnweubhib.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gfgohgdxs.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gyygpakaa.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gtofafpfv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gjdfzidqp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gyiwzatvn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gahilkbdv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/glcaewgxf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gkcfbattq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gsfqubjzv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gqxblriow.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/ghvkpjzqo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gckgkosjv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gqbjpqgad.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqmknvecq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/ggtyboqxf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gmlmbuqnh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gblypcoqz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gcnlcuqid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gwyppqyep.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/goojyrjav.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gvqujzvki.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gogkgeysz.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gjpxaikre.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gghcuicfo.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gfspknuzl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gprkwimvf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gkehiwodg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzmzbvpiz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/goxwayjxs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gumuqgsic.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gkuzipzbi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gtieszchc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gcvtsgppf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhxnhwwe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gmmgkfcrn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gvwpfjicj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gngqbhzgf.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gmdevjlkb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gecqdysin.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gwltineik.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gotxarjad.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/guvwfxlcw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhaidtaw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gidubkuzq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/glbfvkmav.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gornzdtqq.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/ginczjqvc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gfywmogzk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gafdmhkpo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gfitcaxjh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gdhcghvhx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gskihsbxd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gwzbzjmrz.sHtML


<!-- 参考信息 -->