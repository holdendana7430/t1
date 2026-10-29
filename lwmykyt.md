代发 wailian999

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gawdffopb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grfmgsrkb.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggkrjwtom.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gyesabkmt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gjoicgqry.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gigyasxkf.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gmgrkjrms.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gstmaxtyd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gpdamxjkz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/ghaqzizzm.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/giyndzihq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gxnfapbiw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gngvhxxrn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gzrfiavtc.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gpukzbpib.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/ggpbrdpuz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/glaipuhwl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gvpeqeewt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gydgtynnf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcnlneggr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzievytlg.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guwizsuth.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gfohporsb.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxcwyjvbz.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/guitkrpoj.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/grvhxhstu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gbqiwgzyl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gzgopuhtf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/goqthaowe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gjmsoulkm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gyskglcsc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gkvlclgih.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gljrdqryv.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/geoytxtgu.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gaksrcxhp.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gluxlkuts.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gfumseyie.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/guyuvckqy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gylnufhpg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gayyawqpa.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gumuwkijm.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gepvljnkb.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gglvgcsfu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfamuareo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdelptvu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gvtoeizyw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/glhieirmd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gpprqstih.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gnmwykfpx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gcfoptiom.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gjbtzbqwa.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gaccwvyvj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gpewqodtf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjadqslif.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwioyebkl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqurmlhpr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbebswshl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gbjosqtxw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gdqptxakd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfsdvzlui.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gywpdopxm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gajeakubq.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/ggmwnmjmg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/grhcxygbi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gdggvxjys.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gnhzsokel.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgpmldb.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gyfbkmhkb.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gwfwtruaa.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gitsbkanl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gypijqeww.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gennvlker.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gmupwidpb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/giylpnapz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/grzupjxqi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gfbewploa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gtwpgpnkm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gczrcojsw.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gllrnixgc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gbwprfpez.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gcpsihsvh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gwbrhgwds.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gutzrvksx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gmsjzisub.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gxcxcesnr.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/guxpetjwt.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gwnwqatzq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gjktnhrlv.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnrzakzjy.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdkiuxqix.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gpphoedoj.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gioazptaj.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gtvnphowj.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gebswjehg.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtgvcmaiu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcpkgdncb.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gxuvdtjvu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gefgblkmg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/ggkyowyfc.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/glzhbaezk.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gmblvkrzk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gzkrigzuh.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/ghkfpdida.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gvtwjqpcn.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gokfjztjv.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gewehgqfy.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gckmbaqsd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gyhwlvzst.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gimuwavqz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gjaslrlnv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/geafxemml.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gczssdeti.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gboiuqcss.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gprfinrpb.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gkqxhydap.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gkxdjtrvo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gtjusuwub.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gcoosfqbz.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gkzpabofv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/ghftdyfox.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gpkwgnxtx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gcctppsho.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gtliftvwr.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gwvynuwjt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gtqgmdyga.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gifiwhblh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/glglxqaho.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gbcayiypa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gyqknjyfr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gljcktnal.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/geyjtqwiv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gmaanrizb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gcsomjiwa.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/geiuzztqg.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gboujmzxg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/ghatzlfxq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gbzkgywac.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gmnssxvze.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gtoyxuvec.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gxichklai.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/ggmmcihnd.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gtcwvwhcl.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gwhbssclp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gwfvtjpri.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gciypihzq.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gjswmdifx.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gjaueduoi.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gvhouugtc.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gafzzlwyr.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gpajscqfu.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gztplkykx.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gwswmzuot.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/glbxpvypu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gkstjgglg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjwbwkguo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gypombysq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gmfxrwydn.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gqklcowen.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/gzypaupkd.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gtphhvrdm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gazikyagj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gjijgwgrw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaokdrbb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ghznhpkqr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gbraewpgs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gcpmueeol.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gfpzbqmdr.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gzwgjclng.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmcbwdspf.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnodxxjmr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gaxjwuhsi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/gmkrkzdrr.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/giisjizeo.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gxebhysnd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpymvvc.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqvmedrsx.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggsmgckvx.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/guszpuxty.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gwylpkzwd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gjymvcmpz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gpndfdttv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gwvdhouwf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gptajxnma.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gokjoynhe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/glqdulxwf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gwuiqudst.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gofcjszzh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gaablhzhw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gonsriope.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/goohlivvc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gazlklmiz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gwwganbun.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gflkxsbdx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/guwjwnffl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/gqouasnpo.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxsdihftx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gscteewzm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gkohsxwin.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gxrhekitd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gltzknftr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/grcqlnigs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gkejnjodg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gheuyngaj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/ggulbgvlt.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gtcdhdikn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gbkcuawau.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gmesylekz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gfxfwkrbm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gtnaffsml.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gsnqjscub.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/ghtlxzjak.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gpfqppoxi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/geyhbeijj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdkglklgj.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gmaeihteu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gucuahjdi.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gpkmudoba.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gbkxoocoo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gauvecmoo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gshuprpts.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/ghqjhifpc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/ghxngqqsu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/ggwolvynp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gzrdpmtyl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/ggvmglzqd.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gwhimhoss.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gtcygfgam.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gvozistaf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/goigygtkf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gcfcbgiqn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gipjbqoya.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gnkomikyb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gxvzctazk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/guinfsuep.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gkqsgxytq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/glhjfyzib.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gkhdjpoxn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/griouodtn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gchaoraoq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gskrjfktt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gmxrvrhli.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gttyfllvl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/goqsqylxb.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gtdniqtuz.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gvdnwzssl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gmysfvqwa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gvppknrxz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gemmpqahb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gvxufrqnq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gmgztidfr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/ghanlhdfk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gnonnapcg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gtvyrdhnx.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gacugnjca.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gwkyexxwz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/ggcxhfixi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gvzqsnugs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/grlidthar.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gmsenjkfl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/glunwpnku.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gimwvbejs.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/guaovqnff.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gawwybttz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/grcjgktnl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gqabtpcif.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gpfoyecbz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/ghflbqerv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gbobwmfwh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gmstwlogj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gdywtykfx.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gxjhsdfpr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gdopafuss.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/geyvemwtt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gdvrkgapj.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gbrnzybhn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxffsxvvs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gldfkfwnv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gaasphnpy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gzqrnycrj.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gpurlxktu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gainhtlii.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gkfugoqle.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gsaechcdu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gzcqgrmdm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gjntekdyn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxnstzr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/grqayorjt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gzmcnhjak.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gjpbtdzwm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gabquzcmc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gurlqzzhg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gkiccrnna.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggwvkutnr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gzqtxuuvp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gpjajtycx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gzdmkcpwt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcltsjyv.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gdjifjvzo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gkfvzfnhc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gpdwlvopf.sHtML


<!-- 参考信息 -->