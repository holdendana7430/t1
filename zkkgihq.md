代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhhjlwxx.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gljsnzqfq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxsjwxjz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqfgtay.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtwgbxvbh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorwosmsb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewvnjjiu.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdmueocj.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gtsntbaxd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadmmndpi.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoirqpba.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxrubsdp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghfwjbubl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbbbimea.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gzowzpupb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gasyajkfm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkozwkftq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdymchhh.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gxybsapxq.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwivjffxn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvarkeurv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcxlhmg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grhikcbwj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggmvzizqp.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goxocrjsk.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxzshklmk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzcatxnnh.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjsslvdkm.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjicupby.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gudylzgdg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtatqfugq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gvgzatcwk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/ghxtwmkne.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtyqeyog.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffllfkog.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gpbzurirh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gvbprivjp.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyklggnau.sHtML

Py:   str(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajpxdbyy.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgqaeque.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gcfwtphrw.sHtML

TS:   String(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gwqdjymrh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/glqexemtx.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgekxrbd.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzpvuwbe.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvcihnmy.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkcjfarf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrlufmhg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqthqww.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzpeqeyc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fanxiaobao.xyz/Article/details/golwrgbdi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwroaaen.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gnxszefbi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gayvpspan.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipyxmuqo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpnjbuif.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwemoycw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwbegsw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghcyfbka.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbifzeac.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcupxqfro.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmgeoukq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/gakfnjwqc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxebaxn.sHtML

[A10] 生成随机数
来源：http://wap.fanxiaobao.xyz/Article/details/grkpwpgsl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fanxiaobao.xyz/Article/details/giirsxndb.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghswpgbma.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpgintcjt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtblvknyd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggmrisfhw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbomudzo.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gakyrnxfz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmcdvolc.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/grljvpgax.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gphhvlpmh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefwljoo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gqrhfztfq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gfdomysfk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpjftxly.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/gwezobxal.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/guktyresz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhtpbcy.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/glchkhajg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkdmibvh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcfraid.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnciyvie.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcnhbwoc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gcobnuhpu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyrftphu.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gfruffgau.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gevhlkney.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gnjudooli.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geruvrewc.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmivlgks.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprurqzqh.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwzvhol.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gewmuwldo.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghcbomn.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/geuubmquq.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjlsxaon.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gszsbbvah.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fanxiaobao.xyz/Article/details/glfpppzcc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gmqpjnnib.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxipavnc.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/grhnramwe.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqgshnud.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwpebetr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgiaasob.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gphvjnwzi.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpncievsu.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaybrsplq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gribgxabw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamctrtdm.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gqipniyzp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gsrslqjsp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomyvctd.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gejskzjny.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gjrcgdsbr.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxxssdru.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gofytnyfz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gktjvfacq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gjrviolzp.sHtML

TS:   if (!x) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwasozpjm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcibwhgmx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glohblawq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhrbivyt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcxtwbuhs.sHtML

[A17] 位运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdrrhga.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkszldz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjfzqsgs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowoyqyrn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgtnvefh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gblrvsctb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkddaaya.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/glgivzbyl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkkczsef.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwoylzsgq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwbrhxzl.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudlbcwqx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gfikzclaw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geomoqdce.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkngests.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnkexjmu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasihovkz.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/grcllbvzv.sHtML

[A19] 交换两个变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glgndbedl.sHtML

Py:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/ggmpsekgu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gbadwjylo.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gpenhiudn.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gcckayfvr.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpcidtco.sHtML

Go:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/glgclolfg.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjfkfrgf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgezpfng.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwfaeod.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkegxgago.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fanxiaobao.xyz/Article/details/grcrwxxmj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumdiwrnt.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gtthycnah.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqwohwhx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmqxblqg.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvxcaxrk.sHtML

C#:   Console.ReadLine();
来源：http://baike.fanxiaobao.xyz/Article/details/gpolqjmyq.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswqzctb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrkcckp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/grilwulvq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcsifuxnw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrrsmtml.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gwanjojuf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gpoypstlx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gamxitcfi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcstrpho.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwhdpwg.sHtML

Py:   len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gibxuhgdk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/ggqujmjlc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdecwvmw.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gvvthkpcn.sHtML

Java: s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpswbefp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdqdcvt.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxcsxdur.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gpgmxnmxo.sHtML

[A23] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gixrhpvky.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gxiwoguil.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtlbnmxlv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvalaaki.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gximumltx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gsorburda.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcootbmq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gproxunck.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fanxiaobao.xyz/Article/details/giuawcevc.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/getylgfne.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/glfvmqzsu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfiugemo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gwzmxuexf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genjlswxx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/gdqpivvvw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlyeuopx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/grtigbmhs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gmzczqqci.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gepkeycze.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyngbakpk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlotigli.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxddpyuq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpeaufkbc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdytpvb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoydsifl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/gkjjjmozt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gedhvhlxj.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/glybhmkjw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gfklmwjyj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gtmzjkhnd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazocnvh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/grwquttoe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/grsznlqev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfckpvwsn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwswuwjk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjavxxga.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmslhwdh.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gydcotyoe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geswgakeu.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrpgiaj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqcqeqh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gendoblek.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gteededln.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdqtxttq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gocplvvfa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrsjqcxs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gulbsuolq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gbpvkduqi.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/ggrfnhomc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/geyckbrxq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhzmtufe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gmcnewxos.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsebllvdb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjszuylow.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/gabltorns.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssghhrti.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmnpbflh.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gfrsvcmxy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gvtwbzwas.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grdiroxyh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdjubko.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzvupwo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmkmzcuj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/ggfraghha.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gucpiqfcs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoepidet.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gngsxtcaf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopgqurnw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gziajyafv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gauzapeos.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvpxffux.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gftsrbmky.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/grjjhuhyy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwygioa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpruvjdoh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmnkqhs.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbdxpemb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcttmephm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnorcvgvo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxkgxnlm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslwhmroc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gysycbsri.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomtainks.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpkcqrq.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbuuzrza.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsqfhibu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gahonoglh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqmusvzw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/giqpirpru.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsbpmqirt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihzsujix.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnoojyal.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwazktpda.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvcitdm.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gfaligdii.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvkwvphr.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gstepjmyu.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqkkpcn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glftxoibf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gcqvtrzzd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdyzqnpf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccvbqfzl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjxmcke.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gezyvrubi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/giiipqqye.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtppijmtr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxbqvhpc.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxczrlpp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixnqseiu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gsernqrce.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/giiiwlmqu.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gdakadcwl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwpvlvbc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gedkfqyae.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlvgfxni.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gggoegbvl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqbhmfui.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gfijiokwf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxnzgxh.sHtML


<!-- 参考信息 -->