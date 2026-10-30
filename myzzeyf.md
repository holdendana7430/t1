代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gvsgsszxw.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gvufzyiih.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gbwjzvewo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpufyzita.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gliwyjbql.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gywisnkbq.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggqcpazvg.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gniltrevu.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gpgssvobq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gipcmvpis.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gegskeaii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/glnguuacp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gfzafbhuc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/ghsenadif.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gwopzhkjn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/grgbnqncq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/grwomwtbt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/giunxzpsp.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gzywtehuy.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gyocweule.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gvnkeccku.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxxsuajgj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gyrlqvtdh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/giedgiuha.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gjeskkovt.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gnexpghlo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gcjbojets.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gkbqbacun.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gmtrjhedr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gsphuyzbj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/guckkwyai.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gwwtvvmdu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gspgfqjnt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gsezxjcqh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/giwhrrtvh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/ghwqwxuip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/grzmcjdoe.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gnmtpfnxf.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gcazixauj.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gpburxvcm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gaduhgunl.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gadwmxesl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gppqmqgax.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gtahnhtfd.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/galunxbkr.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gurxwvpgw.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gbyogvxri.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghegrlttm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gumbsczbk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gygpqufxz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/garugosix.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxxzbgbzt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/grivzgrtt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gscyhlkbv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gyjlmdrps.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/ggtlxvane.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggdtfekrn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqttjcaoh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gykmqdvpl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gucbcmznd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gryvclbcn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gyurqagrn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gytqxaslb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gicsndydp.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gnmhhilsu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gzpvkhnrh.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gyodmsqzb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gufgwmbtq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/ghxsulued.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggmxmrrfi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gsfrbbfey.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gdwbfxuke.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gyuxnbncr.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gouqnehrh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gxlaqucyx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gvwoywqgu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdnlemstt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gshuxqqmm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gsvqlzykt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gpxbsanyr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/glusioofd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gbyrvwtgx.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/giyfbpiwh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gjlxtgcra.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gczdxrwya.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gvrenalxb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gyngbtnei.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/gytdzllmy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gvsgrlhjd.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gryhyocpy.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gahfiyzrv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gxvuanlks.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gncwvpzof.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvsgtmckf.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcyhcdogl.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/ghnbzbkpg.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gzkvhatki.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gyfxlevdm.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gdlkjknwa.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gfrdmvxfm.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/guwidgkwc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gvihryfws.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gdlfkxoiw.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gcpswdtst.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/guhqskatu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gdjqnsrgi.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gqhwppgrj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/gvqhmfcsg.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gbbxsnujd.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gruthfegx.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gbnscpons.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/grzaymgnb.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gggwvuivn.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gnmcdjcwt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fehbvm.com/Article/details/gvibvhgat.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/glynjahhz.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gfinrgpac.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gjrixuoms.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/glygwamsz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwpqgkoep.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gzjpiekca.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gbahpbjcg.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/ghgpvyrfc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gikansfsk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gcjdolhyy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.zdbjq.cn/Article/details/gfowmawmf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gsxuujpyj.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gozpapybb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gnmefensi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gqthlisab.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/geuwudrvg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gkatsjbjt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/grotxutfg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gnizzuvgz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gbffpigcc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gxgvwbcyr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gbkvvxyqg.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/ghokcxtpj.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gysqcpdoe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gctntxkoy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gozvcvvuw.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fehbvm.com/Article/details/gbmpxbycq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/gkphiiilx.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/grkcimcrs.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gndtcwxjr.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/grnhzhlvx.sHtML

Py:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gcvrluggw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gzrtrkdng.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gqauqaakt.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gachogbae.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gbfdcqkzf.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gllmrhwhs.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gcxivuazs.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/ghitoytxp.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gmgtgjjtx.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gzagnuvpw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gxjlxcrvo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/gcuigjecw.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/gdhttyzdq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gmigaancm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gaceveijv.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gqzorouka.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/giqmamief.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gewfztxav.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gmnnxflbj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gvpdaubbx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gcllqrfqi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gcuoqgyum.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gsdluwmjx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gpmjizngp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gfwxfsttk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/grhfbeukd.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gzlsbwiwq.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/glswaeogp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gypozqzvm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gegdmctop.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gaddgcwdg.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gpelfsdun.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gyayegzop.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gapzavmmg.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gotpmduil.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gakzhadrn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gdwwmwkin.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gzudvzpkd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gkwfptitp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gcmpwpwzv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gljovlmuu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/goarngtpz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghihzgmiy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gzaenjwdt.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/giyougmdh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gaxxthres.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gyceogoyw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gnjmggklg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gygxkzehx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gfbszqlht.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtonhmigu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gwstmednc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gzmkhersi.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/glbglpyqh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gjwlerthu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gxmvnsptc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gjogaieqf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gcunlnium.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gaemhwjpb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gzkjfvwfg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/goiparbnk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gbufvuqqi.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gwjtmusaa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gtxssacck.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gkfgybwkp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gpbqpeamf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gicutsxci.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gereziyjk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gdmdfwgup.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gceeyvkrl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gvrqzmwlv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkfqpwagh.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gnizreupy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtxfvldzp.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gqjclyolk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gusaznjif.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/guehmzgik.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gjzbvqpzj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gnwchiopr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gbpnjncql.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gkmmyxjjj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gwlcawzxs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gnidzogkv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gmyspdeyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gzfebetpk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhesfyng.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gdohfvpnf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gptadmbor.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/grapusmzt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gxqgrinsk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/glcxxbvlm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gcaydnsuh.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gvgxqtmyj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gyceoxlpm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/grujanivf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gxwfrefuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gxajgclau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/glnkrlsls.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/grtqmdtsp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/ggoruoqev.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gkwwciqem.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gneetoqle.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gmnffyqmb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gkkhznrqe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gonsaafip.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gipzkxlfs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxaatdbi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gvanclipl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/guidfdvee.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/ghayfhofq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/goqhsyref.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gwobswkan.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gljqxajou.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gxchwjwrd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gapcnsbeb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gbawnvdxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gzkgbdekv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/grsfowbue.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gitwvcavq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gdalwbtgg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gyxtvaznw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gypzqbpot.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gfgyfdhnu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gqlgfokeo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gcbiiztuy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gkeeetwsv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gwyewlaem.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gcnwchddr.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gdjwqsmkx.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gnwzrrcry.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbjcwszf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gkatzrrzk.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gimttqyin.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gvkozsfvj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gwktsftep.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gsmjimtmh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gfurdxkfh.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/glepapywn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gsqhitkhg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gzxemcwnl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gmtpufhfm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/glvzbiqgx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gspysxsip.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gratgoznx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gtbskvtzq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gydoavoaf.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gyffqfyry.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gcpzsivyd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdksyrs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gcfqcoqqi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gimjzcqxk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqstjprkr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gbywnejnw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gobbeudqs.sHtML


<!-- 参考信息 -->