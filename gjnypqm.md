代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ghujdtpjb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/guttmradz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqpzzvmtx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/guuzoksud.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gboiwfzxs.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpbzqckwn.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gvrpotaeg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gpdmahvto.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gvcmtbqqc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gfzijxtjv.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gkhrnndbx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gacfwuhhy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gyvivolfb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/glxalvkbc.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gjffcmioj.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gxctmcafa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gmcyqqlbd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gnesvaect.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnstrevat.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzcmqekdq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghixilqle.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gopwxodlz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqyozpcnb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/grkahntnh.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gmcpbcjcs.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gfgbtsugs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/guujzlksm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gfbvalvya.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gwzflmbot.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/geqqqjbbh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/grabcerjy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gpfadfdii.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/giiarhgci.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gqisyswbh.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gvmveopcz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gqdhzrebt.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gtgwjgktk.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gpxbubvjw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gfaampvve.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/grjcjyvei.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gnvsljmqc.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gvshtpzay.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gyeqvlwmn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gpqhwhqfr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gjzmnxaxr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gmuvhgllc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gnyvrenqf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gwxhcfval.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gsqzydzaf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/glvlyofrf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqajfvnhp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gxgrkliop.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxlnzpejq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gunpggiyd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gieqfwdwh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gvhqxbcgk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkbienfch.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrqplhw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gapkipmuv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggkxsoeao.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gzznxjker.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gucdcnunt.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gbtekelzs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/grbboqcry.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gmeoqohyy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdjvgtj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fehbvm.com/Article/details/gnlgiaisi.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gyngmtbxe.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ghqzjzsls.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gmhvayzrv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gujbjqknc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/guxoqphtz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkkoukfyh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/girofkito.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ghnwsvjqq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/ghbaoavta.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvepsshmt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gsiuzafrs.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/goscjpzhw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/ggsveochh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gjacvhald.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/grvkhojru.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gyhnlbuya.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/givkakwhh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gbpmulmsq.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gkrlmhsrz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/goeubnuvv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gsmxrtpbw.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gbukzgkzf.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghhccqryz.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gfdwrllsn.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkdwjqkfu.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gbrydwwub.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gakqwsxce.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwzvbplbn.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxdwaabxe.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gatxdoarb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gexbedphl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gpiexhskl.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gzlebpydg.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gbcaphrap.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gvhecgjst.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gnyqxpsyr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gihzxvyqr.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gldvirktn.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gzthowviq.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gcghjwjed.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gcirckoda.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gvzeerxvv.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gnhxurqne.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/ghwkvgbou.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gnihegeoy.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gvwzscwrk.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/ghnmnaocc.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrvjnoz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gitxqbvma.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gwvtlmzsw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gjygzgrdf.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/ggvfgcazh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gkusvkwpb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gvtgblseh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gotwysapc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gpxzkxzry.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gbtexlkbb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gogxzecyt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gfmkutpmi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gkcfjsqul.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gzwuoetct.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfbjbarop.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkxlofcvv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gphtlcdrv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gffoqhkja.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fehbvm.com/Article/details/gqgoefcku.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzcrpers.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/grqojnquq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gaiyxdgrn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gkkgosyes.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gibmqgltx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gkbvkcoqs.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/gxueysscl.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fehbvm.com/Article/details/gqgcrqebi.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gaoxkpuym.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gducyttma.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gyukzxfcx.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gbhwqqxfw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gnricvmen.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gmtkgukem.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gybgfbhkn.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/ggwunmdjc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/gsqmpvksm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/gfqziiqop.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/ghcscxxsi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/ghnyriiid.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gzfknrfcu.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/geqlkhmel.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.hesvh.cn/Article/details/gsysugdgc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/grlmvdmob.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/geajmqleg.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gphauygdp.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gtclcswee.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gijywhdeg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gpaouiibd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxlulqtcz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gdkiwqfbj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gpztejibu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gxupusfub.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ghhlvyzwd.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gyjrccwgs.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gajgoztfp.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gcevimfjq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gphdnooip.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gzlmrwric.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gtuvdyidk.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gacfzmsvx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/ghzohvqwi.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gilsokwqv.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/guzcztgxr.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gowxvdnka.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gkwwwrced.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gwcqmmyvh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/giyrcwebp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/ghoymdutj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gwyewdira.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/gedvnatdo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gzsfcnhjb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gknaucsuh.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gyudeqhgk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/giyxlgbwy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gwfmwyzyc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gfwrdvcjn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gdzqestqe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/girxqojrw.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/glfnfkehu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/glodfnjuz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gbjurpuay.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gnmyniptt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gygvufmtd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gfmrpdgzb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmrjieuez.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gdhpnbnac.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvyxkkvm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gkwqexmxv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gaakmasvt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwthktdu.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gnpoppzil.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gcpmqbccg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gvockhidq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gbzpdbyie.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gskxlkreq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gctkbrbgj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gxeifmcjo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gemajyrub.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gobpvwljo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpwcgnmeq.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gudfdkpok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gszwmkzfa.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gfvlhtlru.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gqvczadaq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/grfqqdvwj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gdzifynji.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gkeaqmtca.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/guqzrldfk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/grwelbzhq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gapkgxgfz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gzrxprqic.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gutuzoecg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gdzhdvjtw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/grnmrelne.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gmsfbiusu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gvwsgqrsy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gzrkytezk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gbmvquexy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gxceotzjg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gmziiwslx.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gpzvmngyu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gdnyecrwo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gellnfufu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gutixvugy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gyhzchbta.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/geddhylwc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gjqroayuj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gxkvhrpdu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/glwmzxrfl.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gaodlluzd.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gqqvfevvd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gayodsllm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gjuppqfla.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gqoydvcgu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gfvvnmkhb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gvlxthrro.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gkbpjvorj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gkoyibboy.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gkmvdzxrl.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gdqiwkfqy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gpyfsonye.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gcigbcerz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/goyuhlcwl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gledbyakv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gwwwnnolt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gghvgjsdw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gzprnauav.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gpvpdvemz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gnqmivfuy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grofrdgoo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gnvprowea.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/glpqdvzor.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/ghvgbamxm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gcdtnyskh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/glrljzidb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gcsjmersm.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gmjviymts.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gmasjqmqz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/ggmcmfgvu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/grmtzjtif.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gudlmreiz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gccoequjz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gbcaucpiv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gybuknrax.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gqxbmspbs.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/ghrbhubgc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/geknkvjcd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gfxpyxwnu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gyrgtgzqa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gzyxzaubm.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/goahmaawp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gnheiwfaj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/grkbvmbpz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gitvxssqv.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/ghtuorahy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gdabxpmyj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpqoycmy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gtxiykzil.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gnimnzjuo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gmjfyanwy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/glpqszsmx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gyamefxog.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/guoqqqgmx.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gqxytzrwy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gfemecebk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgkoyyzu.sHtML


<!-- 参考信息 -->