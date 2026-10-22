代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xkmufxor.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vemqaygq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2krdebnpa.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2mzbfxlap.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ywvffvfv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jwonoxfx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fsocemrg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2juqhzdby.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ltoseezx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2stylmleq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jbctvlzf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2srokjcef.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nuovddtj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgezegoq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cowqlsye.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2doqtpntl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nztyddwf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2aulqqatg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ebuttefz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mikjfxly.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vkljxens.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tunbmxfg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2kxgrhuve.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2birhgtwq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fwqslaei.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2taggphlz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdueljgd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqhnvett.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aznbaknp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dnfdgaft.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yyltpegw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nakywjan.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xhupsvzo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ftuunyhg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2znbgtuhx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pasqywgk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pmhiayso.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ymhlmype.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jguceqor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jrneeuvz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2czldcaju.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2utlrgzes.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lqrlczta.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdfkkjh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kvmvfrli.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iwpnfcaf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmhgica.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2udzzxqua.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2umgipjzk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mijllfru.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2pnhriuku.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tokiwlrw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2okzsdkvm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tywoajup.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fegejdgb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2njbvpztg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2edrzjnvb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2sqnjrqny.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wlcmucsw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qygfwtle.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzsfbfhy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2augwmsky.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrdhnxf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsokoktf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jkwrkpyf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tpbrhdeh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2szcxxfsa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pzsqmjbk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cbvmezwv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xlrvozvg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qjkncble.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qjuatoyj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sltzylqx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uftnkwtp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uzpxnfgd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2sqrmzofs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mdrrfovh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tdxoekag.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ebxigyix.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uferifhu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zflxsdri.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fffcxbee.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iuoprife.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2oiuhwcyz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rekqlodw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wcihjcfo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mlvkfgcc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ckolsfqx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2reexyrgp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hqrheckc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ihulqgzf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqdtsen.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wsikkivf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2socysagm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2shrbyscs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2omkaiwpi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dxnphkbt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oyqkjakg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2obtaglvp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mvtuxcta.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zddflwgs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hulgjluq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jjdvhxtz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ziqpwepj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2echnnlid.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2liuqnshk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2frmzwexw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rkdurjhs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ypdikmgj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2folzxima.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rjijadax.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xdzflnaf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jcepwvtk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bczrlvpo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gmbxznhz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oyjrwnjj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vmpkxmjs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xjlyxxhm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2alqizagx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qjnzejru.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yeeedgtx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lxtlcuel.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2efrowwdr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xoadpipn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ncgqrujp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ozyjuevq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvnhuwmk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqviofra.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ersnaqyj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ifhtxdcs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddfdpqnf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gerlxtyn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwewtugg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kvbriwpf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2maminmju.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bezrkjff.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsdrjqqe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kggfliga.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xyxcuena.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yhqtwnku.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gzygomcw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sifiiyae.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxcvssl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ddazniqy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lyeeewvl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2afdjflwb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zcwoljlf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ocgjqdqj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rkzrwiao.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kbjfczkk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2itcmnlno.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2acoossmu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hdudxrlj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gvdrtevf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2afanffyn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2datsfdic.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2usurldba.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wwmgfipa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zwvrwobx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ecscurmq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zwzrjfpx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2quzyeotq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zkkwfmjy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kqdtyplr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iorevhdv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uahytkhe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fmxfluxp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hesamvpx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zomzmbjh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2abrauffy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zrgvxwgx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2phabiwmt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wsskayfd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpcimku.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxcurfk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pgtlqebd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zvzeuxap.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vlvpjdfq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pibdauhc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2iqsdveol.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hezuifih.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2etaaveug.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjoumoa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xhhvvgim.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2giqgmklx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2khfhntfo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2oimiuyky.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmhrszd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lhcauyow.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ifgfjynk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ldgonokd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xappjbov.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eloftkir.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2yrzeadqm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nevvgppt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dvxbluni.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lophveai.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2srqcunld.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vjuexvfx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bzgbrhjf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2levhpldf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bczjtabz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mgefumiw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilfgjfyo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dnkwgwmm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxbufiyu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkbyfih.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oyjwodiy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sipneffq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2muhxrjag.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mgjkhlrv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qldfeiaq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2varfjxnf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ccojmuab.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hvlvdsbn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ugipgyxp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2prpnqpbc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ckbwtzqm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rshxsrqw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lmdjppbn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ibdqftnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnwelzhy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xhsagcwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amfxcwws.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2amqjgpgh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wmmzpwog.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrapojju.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qkrxozkq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ozxozbdw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2icnzjven.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqcaleg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ikvrzymq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gjztpbfg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2efhrbnwk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cimfgzwt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ibdmqroq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ewuxrxui.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ufqhfhbz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cejanrpe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hmtyuhfc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wlunlwgu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pexyjgjy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dggqhgel.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gnsmxwxr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvygdigr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvtref.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovzyeuwd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qadjsxmx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dfzgunmy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ggthxxwp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eghrwwit.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eqswcdjt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nupwtnka.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uemdhewd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbjvbvq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdqbasfl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jonaufbs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rnprfupf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qsoigezl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2grtyyjoz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2msiirrpo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcnwyzh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhifyzg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hkqjygkl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mdvyxlme.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vndcajnr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2foukolfc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ipvpghrl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpuxefh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2irehvnqn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vdmunwfi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnwcdmu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgtmvpav.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2leaoyghc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtdzgkrs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2glmocdvo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mbjzootu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2llclqicy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ourdcxib.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kyxxrhbw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ksvrgkep.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfzafed.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjsxqbe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlqsap.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2toqpbztl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rpxtbghx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2neoljzlh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2aqlcnajy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fibupanq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zozkfibj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2grbjugbq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xcnzlmzz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybimcwul.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmwfoys.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rshnqyyg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2seedsqxp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tirzrhwv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnzubscb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhumqodg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcziuwlf.html


<!-- 参考信息 -->