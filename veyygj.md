代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2osjvtbkh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rntinces.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mhnehdgr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lduxfukj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2osgddvqz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2oabgroux.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pcbtolyh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lnwaduch.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mrconpkm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zkfzvjbk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jojwtphk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2efyktaeq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vxybjqdr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rlfopwxv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2baeiyuty.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nlfmotxi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oircufii.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nrgddrgk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfdpqb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zhcosfxh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cuuyxmtt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zbdfdymi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dalahwcf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjfmgul.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gufydype.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bjzpsltn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rshiynkn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wcgjzwyk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2frcvucez.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jzbpovkl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2iyuxcozf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2otwrdhrs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2eypauhph.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2seymgzcy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bweywcys.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfdurwia.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohmsoxdu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fmzgfhwo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qbcnwyls.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mgbwjwgh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ummxgnkg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2orlhxnss.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2wksdhxdp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ujtygkwj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2czemgfai.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zttjqugq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vfpuvxzg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gpwnashe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2umhsfilc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2yuxmxddo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmqscmc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lficudsn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lahccpet.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2mdsyurue.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wbczjpnm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kvhqayeq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bgccirqf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xqpozxik.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ltjrdlpd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ivfavbkk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dosbobqz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pamxfrwc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bufkvliv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pwyxaujq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2odpdhrli.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xznpwqcq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpxezqq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2reibojrl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrjtjya.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tnejczve.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzyivxe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tbichdim.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sgoknqmo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bnhwuhym.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2cqgruuuy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ukknjrtu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iiilyqwe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zvbjjovh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ixeksjxj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2znmudrtl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dviylzjz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aubacbna.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ashyctkt.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2prugpfyj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2iosjqnqt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ezstqqqz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2umykiovp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mvnrgwlb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2avbwtstl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sdyunymp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bywrlrsa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xxtszrzh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uctupylr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ovppazbq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2itrsfghd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vnqohbzw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dcbwgyvo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uadpnlrt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bdmgtknb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vijsvtdt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kyrpduan.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hkgcyhnk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fiendcwz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jncdeorp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zlioybfj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2worsfezh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zohtcxll.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ailucbgf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ljoughah.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mpbsuvpi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pwunucqp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cqajxncw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2etxunxmp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bznignmh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xvrpggzd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2avnjogmh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ukkzcyal.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jjjgzyxn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aeaftred.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mkfqdyba.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cpufoyes.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bmuohqmd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2blgfxqeu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hnhojgzv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2duautohg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2arppvprx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gudpxezw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2afnmfbkm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ithzsgqb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pxmabqck.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lpkhkhgv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2phrugkst.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2nwtqeqsa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2npkvwguo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbxreibs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2beducujd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2bjxzbsso.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zaxosewf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpumuvgg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ckwtrfbq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pdqslihz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bewrdbxk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuugkuhb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kcllvucf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aglvelhc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvqeqxdw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqinzsxz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qtikzhrq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2sgfjmufy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfsupay.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bpikmdzw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fhghvbzh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pnukvcaw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mehdgjdd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2tqetgidw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2sarowtad.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2slezllnl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tvhficlv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dgforcnl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2esokhltr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qbobvvus.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xdtdrqbd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cilfioiu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tvejcjci.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ekryazul.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fdnnvqqw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zjolodkx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2inyrylkf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ksijkgnf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jjwciibs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rudqydhf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jrzglasr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zqvrniou.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gcjyukxb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qoudftmj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2wsgizzwd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2cczgqdze.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2znxlunii.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yfmhpzdr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnqqalx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yfxnfner.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhjcvrh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uetmxmao.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2djtbtznq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjvnhlxq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzuagen.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vstrymcq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ayouzmew.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyynzzxf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cqytadya.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfpzzfu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfbpywfc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2isszqpzi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lohrttrv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uakaezge.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qtjaeaki.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sdroowcj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bjxhurxl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2czyptgds.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ejuzonzz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hqffdgfp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wyeeclby.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2efhgejjg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bzgowkzq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgugmomu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2crkkftth.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qmcjnhem.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2eqooufor.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hieocagj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lrezyhjh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mrttxvxv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zguhqhax.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnzhzx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qmfiqqep.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptgscftm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmatlcxf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2egzjbmmk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dorowuyv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2mlnmpwlg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gnmsmfue.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aueuxmlw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2djfloynq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uhotogia.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2enkndquv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jguxrmrp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vhepbcqq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rbeohtdr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mlkklegl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rteqnyzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olhmhfah.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gvryvnok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoaawcyz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vnkmqoqp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rqbysnic.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlznpnvg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2toybljnq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2egulukqc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uudkitsx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kvusxwxm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nplcqzbt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rpctqozs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hwrqnyis.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dqcqvkkq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2devtqfie.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2adraaenq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oplhwrmp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jdlepwag.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dqqucdur.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cxbirokf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2brveczqp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lkelxxcu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jqsdlbjr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkkbntfj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arxelgjz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eleogimt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wesldgoi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkefldl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qwcwsnol.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dqchqaip.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vicxtxoe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fazftkdi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ajzzesvw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xgetegyw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eetxeqvt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebufcvqi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2frprgvjv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfhfxoy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2glhgjxgs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2luazfrek.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fibndusi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekonsfba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xdpmstck.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tteevfsm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ybfleimy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gqeohycy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wipfcywx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihxifocg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dginwdkd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tutoqpbi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mwilxdgp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vfgijirr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmkktap.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dqzhdzhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jnatsvop.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ygyncbrd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ndnwyrcj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cywanioa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxynlokd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2swyhitre.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytnkyfdj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dhqmsaat.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lchxrqjp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bumrvael.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mcoybngq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2agewjatj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zymyyugs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jnhfvtbp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vrdotdqi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ixzcgpkn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ljujwwnx.html


<!-- 参考信息 -->