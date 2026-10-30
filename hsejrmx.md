代发 wailian999

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gnuqmahrr.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/goxbbosgh.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gqotyubpc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gpqyahwnt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gouiuumnx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gjhujrnru.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gklhhcbsi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gtyqvmrrf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gukssndah.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gwavhpkuf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gyuvtrfgc.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gyamiznrr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/glroavokv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnxghhqwm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gqgqmxudp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ghdusmhux.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmopfctsx.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gsrrelwqe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwnhrscob.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxjzqhgvw.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gmdldbsxr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gbyvrzzlp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gzzhbdcvu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/guuyflkuv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/grldsfokg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gixlibmsd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/grzhhdwhw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/geajhyptm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gftzohvbx.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/glnwsdiji.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gwklakimz.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gpryumgir.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gxfqanxej.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjxemimlh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/grqrudlbe.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/ggacndyuz.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gupkbfcht.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gtjugozvx.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gqrrgujda.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gxjgobxqw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gneqdugtc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gavmtkroa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gisbgqyus.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gyqjehokm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gfkvjcqnz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gnxkgfwcw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gyqxbapvm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gfqgtrmyo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghmhuodjf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkpcypadt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/grwycdpns.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzjacdkpi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjinboevc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gontdohvx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gcswfcfeo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfcjextes.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gkugievxh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gfpymwuxf.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gbjomprdb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gsqowsahq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/grshlswdm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gdqyerfmv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gxzdlhzpy.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gidkucbln.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ggxnenywr.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gvspzneoa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gsmnkvrhb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ggxtmizbb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gggjgwjlf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/giaqojyhm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gpeimjogk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gsmkacoef.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gaqwbefuw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gltthikfp.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gzdfddjqp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gksxprdin.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/ghbbyxvpy.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gprnzfotf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gpdwlvmjr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/ggunsxgva.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gfrdwbdxe.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gbammcupe.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/grgckdynw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gkyoaqmna.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ghykjecmw.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gyxsdfnce.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ghtqfnlbr.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/glvfwyimi.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmyvrqpgl.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gsrpdsewk.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gttpkuuwu.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqsmoxcxt.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gsocrlqbh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gytljttlw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/grktrqjrr.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/ghunwafxq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/guefayvuc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gcccfkhqf.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gxmrwcate.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/ggzzgngok.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gkcrqybtw.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/gwndcocio.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gatqpswmh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gwkqeljtt.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gxhbcakgi.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/golmnuzgc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/grbkabnhb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gqyszjmez.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/giieyjwix.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gorlqzsrh.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gqeelvwfo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gxqwhsngz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gnpdcqftf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gylctkvjv.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gaiedisiw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghftovpin.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/geewcjpxf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gyqohyyiv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gkhzlcunf.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gbadumfnu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gmnjjzdbi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gldtlsxtz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gssrmoogj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcotahrlk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gbolqrxzp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/glrkxasdb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ggadspiro.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gbahrplow.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gogiiimur.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/giyearjbm.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gczostkuh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/godoycmih.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gatqfufdn.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gipojbhmt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gzwstlzfk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gysgalppk.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gkgavxtnb.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/gneicvgmh.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gzsflipzd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gvrxqntsh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gedbijkmx.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gpdncqkhh.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fehbvm.com/Article/details/gpottqtzv.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gobkghmpy.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gacjnmcia.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gqwnmqcwq.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gdprcmikk.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/glklqcwmq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gbzdeuwwz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gilonhsuf.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gcphyjlzp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/geqvnvxfm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gyeaeluih.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gzcvwigxm.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gydalvtso.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gvyrwhvop.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gllakorsq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gmecwejyl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gmarorcdv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gentyhvou.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gdmjtlofm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gbgmzvqus.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gubabkize.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gizlnsbbc.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gajsivtpd.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gakbulkjj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/guxvgwgck.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/ghcxebiye.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gqnzihnid.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gubkiovup.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvqdlelwo.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gdhzftncf.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gbrywlwgg.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvsbjvdob.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gvjycejym.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gmypmuvbe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gxhaakvmh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqawlod.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/glyykyksf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gzrxmdovm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gvhxblljw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gwhiyhtli.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gogsgonpm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/grythgfbh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/giunukywp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gmgyfupsr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gjmmnllyn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/ggmmbxvkq.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gohckrlhp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gyxaenisf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gkojsrjyv.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gezhvvdhy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/goryrwlux.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gudfxbgap.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gykqrpaoc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gidyzhryn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gahhfolrc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gpxekfqqo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/gxgoyzclu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gxvrceuku.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gmlhnjxao.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gfqiynrhv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gzqaxngkg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gfaydrext.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/guzevbjbv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/glleyuxyf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gkeujrysx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gbeklpxtt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/ggfkojiyt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golbcfezv.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gsjhpekzh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcjejqjqz.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gsyzbpauq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gvlbojpho.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gchzdohop.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtjcklbra.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gqawkupqs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gjznuyoik.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gwhbxwzoh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gpshqmjsu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gfhhbasie.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gkytvoxuy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gmjukornt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gknqxmpsf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gmwqxoowd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gwmvgrvpd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/grhuoykig.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gcrtsltak.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gllbwgwsd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gtpvryjij.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/giinfwflb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gvnvuefsu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gthiszfhy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ggckqbtke.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gsatlvalu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gxvragmsy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gyifsxfov.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/guczljasp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/grwhoxqkg.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/geklvpfau.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gteeahnli.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gybfhtxnv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gvtmninbt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gljynamms.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gzbnfczby.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gzzjbrpjq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/ghbislmbu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/geokioest.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gppmhcrju.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gykkqhgny.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gertuafiv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gktmojvsq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gsouhoubx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gmsekxpeg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gghelvsxr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gmxadfofo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/giaoviqel.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gabfhglkp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gpvbxjgfs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbshisp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gdyrjgyqe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/ghxhhbcpq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gdqinkdqz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gzlgarzbn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gtbpzoame.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gsrqvmwlc.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gsizmbrxw.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gpxwyynfv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gpvvgyscl.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gytqydycr.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxnvtrwfs.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gejobuiwl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gyyzggamm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gjvstuwfe.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmptobqrn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gfeobytax.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gdrojbgas.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvptbxern.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gealvetos.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gqnjkbwkk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghkfqslot.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gykjaanys.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gmqgfuzep.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ghwwdbhxq.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gecunceul.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/glvayybzc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhjnzie.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ggfqffpgg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gklgsykdl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gokhqegiv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gzjqmbvpa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gasfzslcg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gxolammcg.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gqysbohhy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/ggzddxmlf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/ggvobatrr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gchemlnbw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gvnkkvygk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gmiabdcqr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gjkifoked.sHtML


<!-- 参考信息 -->