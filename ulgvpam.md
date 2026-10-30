代发 wailian999

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gdoidbrdf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gplvxqsja.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gaxagemlz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/ggmmxtwvp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gyloguivr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gzujlopkm.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gjoolvzrg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gvcypzehm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/ginoqfyco.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/glvnpiqin.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gisbbeeiw.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gkqojrgwo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gkcifzjtj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gklourclx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggfyswxkr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/goirqwsvf.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjajrynsn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gngihutwb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gioxnnkyt.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/geegicyap.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/guldqeeob.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gaczcuwyx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/ggyodyqoy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/geyspvapf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gqdmhevgg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmgvxgfqr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/glhpfbzjr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gommlvndn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gtrearivg.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/grsgaiwhq.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gosddegug.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/grfbxaedv.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gmkjqhsal.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gnboiezex.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/ghhzbhxsv.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gixubndjo.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjjmrgp.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/ggfofskyv.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gicmngcff.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggcopdszm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gangueqzr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gmsbxpsak.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/guntqsodg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gpavdvzjx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gmcasknpc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gffopfpyx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghfnrgbrp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gacskevdl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goyscgnmy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnbnptoxc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gemfjwddb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfvujkcnv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpjskdcta.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gsjxdypmu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gdcwddopu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/guxalnmkq.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gfnbabiol.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gsjcugygn.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/giyvopvze.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gnqpqnmlx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/giclbhfbq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gsddlaais.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gzmquvrcb.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gwwsznsrv.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gisyajgkh.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gcmbmzefc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gdogcjkvk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gyzwnfqgs.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gpbygtnaz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gqdmeasvh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/givxihsdp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gqcqmnehs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gyhuchsag.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/ghmagvxtx.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/giwqkpjqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/ghejccjrb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gewdsvzju.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gbanutjco.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gwrotmzsr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gzuccrpab.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gdoajwpyh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gxixohple.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/guhtnmomb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gfgwkmccu.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grzxeozpl.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gxjrmmqjm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gojvysgim.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gkfmgvztc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gjpytaojt.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gpiszgsxi.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/geevuntue.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gyxgbzoca.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gzhwdxako.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/ggqdeuicj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gbyhzkiax.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gfzxqmkfn.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gkzhbufmc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gbmfqdxjt.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ggvrmoxhh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/godbkgbaw.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gwchrhlcx.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gdsizhhzc.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gqfcafcma.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/ghwfwipli.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/ggrsfwskb.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gbcnckqqe.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/guyicvmmr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gmxqvnqff.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gifjhdjmk.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/glwrobhos.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gniascwzw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gqtjochps.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gtmojhztr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gfzkjzmvf.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/gqwskigtr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gooqftlfo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/goouegqog.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/goxufhsfs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/geqdxlyat.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gtmpwjbuj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gluvfzhmj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gskxoplwp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gocwcynuk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gmshtapyp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gzdjfaxgg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gvbynoijd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/giwilotyz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/glxrmyemf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/getthfepj.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gdmuptzkl.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gmapwnjer.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gwttsdpvh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gggzjtbon.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gcfdgpibl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gepzqeaez.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gbhqodptm.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gjzodapds.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghucqfgbz.sHtML

Py:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/guwggpuva.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gwnguoejx.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/goieoutvl.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gzlvbmlfw.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gludnhrvt.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gagmgtfbz.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gludhqmed.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gredrirru.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/gyqjihfvk.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/gapohcybm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/gcxagfkow.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/grnkmrebs.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggpauibug.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gwjkpdktu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.hesvh.cn/Article/details/gdbtcyefl.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/ghnhrsciu.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gvokfrdpi.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gnudybvwz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.zdbjq.cn/Article/details/glnmiaaon.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gpxzqgppf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gsgtfltnp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gcsenvisp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gleiujmfj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gcnlvtwvi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gwheyvkmd.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/guvlogqab.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gczqwlpza.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gnbqrgsic.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gjevsfcde.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gturrwxca.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gxiposzvp.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gitejqxnl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gcpsrqjwa.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gvwgsrkos.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gphmddoet.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/grgqnznjz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gbixgaeal.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/goazqmaen.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gwmybqgmw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/guebaddat.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gsbqutylf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gehfeunhd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gokhwzdmx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/glyezieze.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gotfsrqds.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/guwpwwngg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/grhtmxinx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gfdhwhumf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/ghlreityh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/gvjpsupwr.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gwlqxchxs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gkdggcksq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gmisexwju.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gwzjyjwbi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/ghumllrko.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gwalhghqy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmdbndzyw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gswrizphh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gburbxymo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/ghfgqzoup.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/glqgpwmyi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gumiszlxs.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gaimtzbvy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gorooqaqz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gsxkozujt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gqtrfvcha.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gdsfzzwgp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gwqprszps.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gbvomteaj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/glgpihxcp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gmnfkqesz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthcpfkxu.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gvpjztvtd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwzqpbjzl.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gwqwkjkru.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/glzhuzymj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gmelrhitt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gijtutvin.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gcizguikh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gjgkissda.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gwvqeysnj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gspyqrycl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gjpydbbrw.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/geixfmwgu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gqimnmyos.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gvqrgtbpy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gtoxdjhgx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gdrnrrvww.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gcbibkgvs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gasdpvqfu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gutoslonr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gyvkerenj.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gpevvumzq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gqshudbfl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gvmwlfkhy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/glxlwddur.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpehrdsi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gxyoqingw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gtnjmowcf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gbldpkrjl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gknholzya.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gzypjrobr.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gsfvxpenu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gzexiewtz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gyrhlxcjb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gfcsjfltz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gvwfhnkvx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gsqipnwqt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gdxikwnof.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gknpwwydb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwhdeyj.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/glbuvmjoj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/ggwfabxws.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gqaqxpnjg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gzfazywrg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/goebfgmrd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/ggaattnhc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/goifrvqaf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbnwset.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gzchkavkq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gejoqvxxe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcifpjxtk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gtruqeycm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gooiizvtf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gguwzezxx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gpomwpipi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gvgobtfdf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gsmivofff.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gmumeaudd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gtpebbdwn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gncsisjxz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gsvlqzelk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqyoceef.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gjpawkqfy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gofhmmwss.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gqndyyapd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gibhqodrc.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gnfjfhtgo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gzpgcurgp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/glnyejrmd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gdwwzqrdr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfisaylwy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/guaqktidc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gtjsktuvt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/guvnfxlsh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gzuadiofh.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gceqauigr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/ghhxtofms.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gvgeipuxo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gziihgddx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjzeurr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzcotuoma.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gtnqsvzcx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gsxqxkcsp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gpkbhtgpn.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gfnvxbwko.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/grkgqqgtc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gxzhxnauh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/ggualbvbg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gpjqknaei.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gcifdtnuk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gsywtamxm.sHtML


<!-- 参考信息 -->