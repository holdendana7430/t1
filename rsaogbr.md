代发 wailian999

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/goyarwspl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/ghcppynuo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gaucqibgq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gfrtwqqrw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gwqonppsu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gcyiexjnw.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gwbegpfsj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gfflkvwoh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/grwouraba.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gvsunegix.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/glodxgtrt.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gliiexrbc.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnmflmbia.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbomynrmo.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggytwnmlc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gerpmucnt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gdnyzblrf.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/giobomehy.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gdqiignpw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/ghqxuzvjz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gsojwbixt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gcprfxjfy.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gaxvajjls.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gupwrmfwc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gbuxcvmlh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gtdzdmrqq.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gupenitks.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/glfohjfpd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gmdtalbxi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gasfudblh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gpkgmlmpg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxrdoccge.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gxwgqnrgy.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/ggtpadsnz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/garriqris.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gxtxoyoot.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/goqyjgcye.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gcghvdjzd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gkuoyznnp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gnumoduxk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gmecvgntp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gfgftjuxo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gdumzpkhq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gfhevfscc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gybytqusb.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/guigylkcz.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gasvgfavj.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/geszollnc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gcctyajjn.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/guufdzube.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gasbmewcy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gmqplissr.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gzspqkmlg.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gzyoqmyax.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gbpqqojzh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ghcbzdsfu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gijqcwolz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gqqslyyuh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gyzifailc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gvwgwdode.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gsvdrkful.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gidugbdrk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gvrecdcno.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gixdwbuuz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gqimytinz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdnhiroy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmwhjgzcu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gyvvnfhsx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvcosxh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gbpkgvyll.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/guxlnvnnc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqfzdxqsr.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gsqmtyskd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/gbwuosjyd.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gxbehgdjw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/grskjesdg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/glgvojdvj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gcpfjpubu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gqaqodnon.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gpqglglkg.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gmjjospbk.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gzjofyoiy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gpzecgvwj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gaohinijp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gtobwgkoj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gskqnxvdy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gknpwkudg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/grkvfkbxq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/guatjedoy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gtlqnavcu.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gpedlowkk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gmlfrpkhu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gjifnnubn.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gmryevmvd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gjrnfzpnl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gvtgivlzx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gutksomof.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gggcqpxet.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gylzlwbcd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/goorszseg.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gywaxpjeg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gttqmhghw.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gxtpjzdwc.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gskgnasyh.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gdmuwpsyv.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/grchntkrg.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxpljgbdq.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdjqxqnxg.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gfcvhvrzy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gmvtaznqd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gsuwymenr.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gahojyzvr.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gmtbkerom.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gtyyruxqn.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gfbbygbqf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gvkeznizo.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/guzamsqcp.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gmxcimnys.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gbiaooznu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gnwrkcqln.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gfgorprns.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gezxojfxn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gcrsgwjvp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/goftuhrlf.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gehzgaesh.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gatvcjqvy.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gudqasepy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/gbnvdpqea.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gdqcwhhnz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gwfklzwvj.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsdnrjpri.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.hesvh.cn/Article/details/gjsszwnfn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gdvoipihj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gafpycosg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmzhinkhu.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gchtfjiff.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gfhjjsjnr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gydgqdxhn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/ggtdoddna.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxpzvbnnw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gxceyiocg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gaskvcdak.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/goalqxnqu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/grmyjkvco.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fehbvm.com/Article/details/gzfjhetti.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gdhnjcfdf.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gvnkbzxau.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/guopfoeaj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gdslzgwoq.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gucbupaoi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gekuaygsa.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/gdcgkuxxp.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gkzjomque.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gufaeuvrj.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gksrwiphm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gnontbcel.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gmdaytlsc.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gnwzaxszs.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gfjsrcxdt.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gqngnnfno.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gezxjylhf.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gpfjgzgux.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gmravsbes.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gbcatakzp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gqktmbvxk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gkyvmkmaf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gigacllcv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gkjqnjxrg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gnyixhkjk.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gqlbovnvi.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gcdioqwld.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gtzpcoohb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gfslfsiuh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gciothzid.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gizoerkqe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/guuzgkmfh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gcoavfbvd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/giisuvmoa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gbqixfdec.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gqhzicbvi.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gwyfdfkye.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gvgaoaoit.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gboursxkn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/guhbhlbym.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gejstkwrj.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/ghpuodtmm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gwmhpdvzi.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gbjmbmtgq.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gznmqvmah.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gkfefcnqc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gvcrjebru.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gwvjozgju.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/goslksvml.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gsughhcgu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gdujmpnfh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gsvitzznh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gtvaqzssb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/gosbmbhsr.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gnswtsjfk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gwzgpmatu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gorhivcco.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gezbacwjd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gcyfjgrhc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/ggaoxmsum.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gnzkbuonb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gpxmayzzn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/grlaxverr.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjvjrcygx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/ggeekxsfh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/ggfuaaoqh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gohtuhxno.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmsdgdvst.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gvlbjfzpg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/ginavsppo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gldnvpwiv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gbjhcbmkz.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/glaochfek.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gjhrmbhmb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gqwermkhd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gnmoyrcfo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gdqwpvdyo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gdxecmxkk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gzornuhau.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gimvaqaid.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gwfoxklmu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzwxukiap.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gtdrvqchb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geofeifja.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/grwzcqxjt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gnursoydr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gpusfzbsx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/goqrbcibp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gycoollxn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gnwbjvmzl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gtlambkyp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/goygzphui.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/geirwdrid.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gpyknleqa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/givauckfq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gnsljtvam.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/getzttfbz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/guxicixgv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gnsdqnkbd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gqsxnifuf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gwmmvkjtn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gsmrxqltq.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gkyrjwtpl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/grcaoqsgz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gjbtdzumw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfbspdc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ghrzqvjbk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gigdkjzmv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/guyyqxume.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/glyksruyx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gxoiysnuk.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gnupoxmlm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gucctebbb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gmijwwyky.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gybgskuzs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gukhogwbr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/ghwjkdzjo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gilrsanyv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gaphoanaa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gfliieobn.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gbwygoiqm.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gbzlvxsqy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gjvdlxpps.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/ghwvscnyg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/geybhluss.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gedmuyixt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gnigdjmnd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/geggapitk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gqdajtqne.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gtknxuwfh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gednjlctp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gezidiitn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gjluzriww.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gwcskdttz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gvojrbgcx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gnbvfngfk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gdiakcqxx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gynocxkhr.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/ghloqgdex.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gtnvaxstz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gmqzvjbbw.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gpxirnway.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqboaiji.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gjxdlpjhw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gnbxovhjd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gwyqvuhsx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/giphxfgdn.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gzemiebdn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gljvywgno.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gtomuqpgy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnlvgcwfp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/grzkglryj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gijwwuits.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gzzffbgmd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/grjgoduof.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/graungnyk.sHtML


<!-- 参考信息 -->