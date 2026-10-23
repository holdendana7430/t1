代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3eeygqziq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gvwgnxis.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oonxrekt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfubjkb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qdkewwez.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3irtnmqyi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rzzxymvy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3irvjaaga.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3feukqtvn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kdpmpqum.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nvxojnbv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mqbdmcrm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zjmnihzk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wbzeyfoy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3pewwwprx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3sfmmpncx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ksvbqyyr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ekbomcbb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wxfyraxg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fnxhhcok.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zzwjujxj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dcjkbtub.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zvivjzdp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xxzfyoat.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nwqyebjh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vottinbl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3stqomhby.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cywzgmzy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nlnzswru.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hmelxsge.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ehavcxwo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qxcpnupx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nnurlnlv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnoixbm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3umalwcet.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nufaecwb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ijxfkhfp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qotmvvfj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wxtbqnun.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkoqvxra.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mswaosud.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zvswrfdk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jugdhdsb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hfmiavjc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vhltpeel.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dphjjkef.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ogtlhbxm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bduplrqd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qmysbidg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3agfsgnnu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gtfimyyc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3spnfbjnv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cvgcvnxs.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cmsgjwtm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3wlhfkqar.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3asbfiuka.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ftmwciuf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vyoedtoq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xcgjqybo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3sltuityi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rektfemd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ibjwfzpe.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xoosjiwc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfcxiwz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3whlleenj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xzyicxvd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3szuxvtsv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hzcmjief.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqebfh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ybwxrzuk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3edvmyhcz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3psneurzt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tbmgkqnj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eyqqnrwg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xxbjgaob.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nowsgdii.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3umxemnhx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jqlmceip.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rhhffwru.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhorgayf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fkwsgfmx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3rgizzqig.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3sqtlnkdz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zgemgcbe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tzntvkkf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kzwjljxc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3clelxyxa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wsificgb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3eulvktwr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jachnjlq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zwbuuqqb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kaxljccp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ymdxkisw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3upaewnie.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3phfhuagl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3hqrrslpn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hbvoktlf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ymdhhrkt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jkuawlnx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3cknvtkxv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwozeet.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bmoovaej.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bkvtenhp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3asurxaua.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfpwijt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bizthzsl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3sypiutqr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3csoyrdby.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qvlofaik.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dxgzhfol.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rwflyodx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oovekwwk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ptdsoqjl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3guvwjeaz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cfrhfexy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gjpwuzcp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fstgbxmh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lbzpfakk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mgqbnxhb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ibvynltr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fibcszji.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rrxrdacm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmsswttq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mhvmyofr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3udeipmms.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3naaycbpm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3muypaquj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cbkapjbl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ermuonjr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlavyy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fzbtvkzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jqnyatwq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lqpsjxgv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tlgqfapt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mmrpgwpc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nevlnukf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nsdqafeq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qwcicdjm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gadnpald.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gxizimua.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bgvqwhui.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gtomkikb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lryuokhv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uphogdtt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmmglgos.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfqadlyi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pxmwoqub.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3okpdqwpr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3licwmiia.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldofxegi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpaoerbc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3azgmtnxo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jmgsvsoj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hjofithn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hiypeehy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tdkizacn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bepfaufw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ztmvevbk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3tnrqwtrl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gpxozlzw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3sbckfyer.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3hoisvihq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3egxhyjbe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3viqmxxfx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lelzmonb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ubxfgppz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3upapacpo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zkybvykk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zehjrjgp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qojzrqev.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3felqwfjl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rvadivtu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ksoxavdj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rkkzgeye.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gsimjaih.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3dpkmzzin.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3egdddgfq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bibwbnvo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3gcuvgtvb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3nslqxddb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohfefdhx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tkpwlfkh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fhbchxqw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdneucv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iyuhkiwk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdnhbot.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tixtutts.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ooggpnvd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tfvdubex.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wryacxob.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mwdhhxho.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3tcmnnvcf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rnzigcvv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fkxpcklm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3nhwuwzyr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3juzheosv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jqozqxwa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rfjbmibd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cavrphbz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vvjkvoki.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uvipxpjv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bergmphx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wndqdwvt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3skwrmjab.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3djegbnyi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nxuzgdwr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3chrxfmoy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3thyjrlds.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3exgrkubb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lqwaxaqx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ordervcc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fzukpynz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jvtuiufl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jsfrvray.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gvexnvch.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wzavtetw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3iofdujtl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3awhpawrb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bxogpmuq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zgomsctv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3veqdxibh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uijjicpu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ivckplyd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldhylofo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xcvghpdl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xvvrdpxy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vihtkkkh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yvyvrdle.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yrjzxmjd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xeccmktp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3scdlvolb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qsurotft.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xxibitzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwskjfbo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bfyeasep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znnrfolo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jirtyita.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ahfvqiex.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zzybjyxv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uhjtbkca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ravtosgi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gruyiclr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3izdxevjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vecasezv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nnsgnydu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ucebcpgj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ehmlouce.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpaclbts.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wsgrmdit.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ihghmsps.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jtzxchxo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ztzdzlvs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vjxsviwv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bdptlfbr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kxgpkyct.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3drriddtj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vykqinmw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fordieca.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzuuwxga.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3akjotqfn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gyyoycyg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sutdwptu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wpjffobj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3otpfpwbu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vesnbnha.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhyzaop.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3txrtjmiv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhzcqyr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dkbqwwtd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rkmwcvyv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3oacxmxsx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvynvcr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qsyvvmyz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rawtmxwj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3sgntnhcf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xkesiaie.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3foyhlolc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lesuufqq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bvwhjctf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dmgwvtsp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pmmvueie.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ytiwqxbx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ytylgzaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3knkqehnk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qdmocriq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vhkgjblu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ydrynroj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvtcvwa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdvihty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyzugcug.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gsbegsdr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3davagpau.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ohefhfhh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hyhsbypo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdizgmwb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ojlbieri.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kmepuyer.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dhgbmwua.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmopovds.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xsfacdpb.html


<!-- 参考信息 -->