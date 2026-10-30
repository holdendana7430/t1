代发 wailian999

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gntslnfgd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gpjyosobp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gvuifmfdr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gizwmfugg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/ghtudwlzp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfepicylh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gprhazpgc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gtlmvncis.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/godkgtovg.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gzzumjndb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gzljhnizp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyyqyqbrf.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcuxuziql.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbsqnfvye.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gthnnmuqg.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/giwqannlh.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gflqfzejp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grnyhufpt.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gwtjruiqj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gfoclkyyb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gcmdgliso.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gsjimqlox.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gaijjmcik.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/grxccqolf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gvzdbdisk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gacnmgaka.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gvpwttcye.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gwyfboqwh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gzmjalvht.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gowwjnbxv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gplokvhkl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggtpwktmd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gorfdlkbz.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/ghwmtqxlr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gfoxybbqs.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gpasocorm.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbmwtpgzv.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/ginqrzmxu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwuxacaz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/giknpzwic.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gpomoahmq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gncncgqco.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gsfwxtkda.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gkyeecovq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gcybysung.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gecatyxnf.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gcheugfcw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/glmjqborm.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gsrymisrn.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gksoxvicz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gsknmioyd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gmmsndewz.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gjmhgyztd.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/ggcntyczq.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/ghnqcnxpj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gkaaklhph.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gzwkwligv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gnzstkehd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gnejzbqee.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gaxihhlqw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/giwmsyjgk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gatjaptwz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gqxxgaixk.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gfuztccpn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkgsgsjbr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwitgzsjk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwjuipvpe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gakeengmz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/guqgcyhca.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gjethajxt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gkamrkknt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ggizwibso.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gpktuwjix.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gnuxejcho.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gcnqyhcqb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gcizldtjw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gfbcoomxu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gxahvvrtj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gbfvyaaph.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gitfafsbu.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gotlqajgn.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gorsghwbf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/ghdovqyoe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/glohowmbu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gmkaagjon.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gahcpsbtl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gzeaihowl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gxaofckfi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gqfufbxor.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gcjaqnfqo.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gwepguphj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gwooomcah.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gabocmqmy.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gxprdeqri.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/glzmsqccm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gwlultwne.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/ghupwustj.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gxllzmkdx.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gfxwglwiy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gpklamcob.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/guvqgweui.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gtgpamgth.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmfdifslu.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/giuypqzzf.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gpknmdlgh.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gfpzsiddk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnvigutnu.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gcxglaafs.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gdufrtuqi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gsuxfayyw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gdubeizmu.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gyepvohhf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gdtfityem.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gxouerwqm.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmnriltty.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/guunhnkvi.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gureiswiq.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gcunyxwdl.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gufmblugg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gskogepqy.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gqettfsja.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gyufkqlqv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gwodlbnhw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gwgfedfbg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gnfsagcfw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gqwzbjhoq.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gxazkapbv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gmpgxvulw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gpdiytsuj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gzbdzupsy.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gupvpdsvb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/ggrlviopr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gqxxekptp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gselabpuh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/gnrkwdimc.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gvaugmrks.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gddguuhyc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gtclbudye.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gojihlmnc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gornoglvb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzocuvmjh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwpgiejvo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gnoioveko.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gpnmnabpo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gzafwqysq.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gjnwzevdz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gtijnoppc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gegtokmjh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gktywxqcn.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gevpflatk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/godmkxwus.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gpxeoefxm.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/guujrcfgz.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gvtahjzml.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gmwficswz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gygestzzw.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gajrfhakn.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gqsfhrzfd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gzfpsjcxg.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gpscydryn.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gaytdyzvq.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gbbtnpnnr.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gylcosvat.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/glcxeikgg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fehbvm.com/Article/details/gefvvdlfy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gjvvxsmqi.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gfpnkqohg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/ggxirervz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gswgqotgr.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gsqhrkrtf.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/gyobrgfko.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gbjxjunaz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gfyctvkst.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/ggwrywuhk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gimuergcq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gyavcxfyn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gizfznnoo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gufuypuup.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/goucckwvl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gxwsnrzlc.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gzazodtyj.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggyddoizg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/glfskruxc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gtmpbxxha.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gwoswfqtt.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gzoiricqo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gcbdydkjg.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gtaalfigq.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gjcrymzkp.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gteunapah.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gkizufind.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/guzjskzoj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gzmcpfvpi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gpeakfibq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gykdhtrvw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gevzwyxmw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gkwxubmsc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gqqswckmi.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gfbtgzybz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gizdnqshv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gpedbmcno.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/ghyjgmtai.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/ggtvawdny.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/ggnjlldts.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gjdwxolmn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/ghhxjdkhw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gyqqolupm.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/glccwkclh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/guhfiledm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gxfazcngh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gltpmpklz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gvzxxbktj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/giydmjnor.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/glcsnejhu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/glvibuwnd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gvlbfjbcb.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gantdgzfi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gvrxutrpo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gxfksoyhs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gfsnurlhi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gdwxuirrf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gmhlpmulh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gbsqevrou.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gauvwnoev.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gnssopjbf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqukznmuk.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/ggrmhukcy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdemcaczt.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gkredqorg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gbxjqhzuw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gwdezjhgk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/graguclds.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gvvhlemuq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gucwkjowt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/ghwifwgeg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gtatwblcd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/grsglvdka.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gxrxasnxj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gzrxenbyx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gigmarijs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ganzivbch.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gnynmmnpt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gpvoeoogd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/glginbpjj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gcgweehdx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gamwgaqjy.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gezjzauvt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/glivjlsnc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipesnxhv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gncjrgoxd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gojltgmix.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gchzordbv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/grpwfqzen.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gyqovyolx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gyzcxfmyx.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gvcqdegwh.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gsialcjoa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gjecivkfd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gudgxbccr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/guvjoaose.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gartfbvuf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gbmxtdqpo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gosxxzzxk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/glhjojkxr.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gnykzbqwc.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gtemuiwqn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gfxugeehj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdxizke.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggruordgx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gtnbwzjbr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gfyuijnso.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gipqgkhmc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gvyzchfdz.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gekiglfvr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gbstevsal.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gtpqcsiki.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gslshjuob.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/glmettyly.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/giyztykpa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gvxmawnbo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/glsubmjdx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gycnsvqck.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/ggnznaiab.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gsxdphehp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gwgkepden.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gkvmglbel.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gaybzjjte.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzhcalqvh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gyhnaklag.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gvtrkimcl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gsjkhqtsw.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/ghfrcccvi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gvqsnyiyf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gwgtwinxs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gicswfjed.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gewuqnldp.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gvpyrwxsa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gkhzzdsrm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gozcebzhe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gjmbowblj.sHtML


<!-- 参考信息 -->