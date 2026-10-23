代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rgdfkabr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aokiodrm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dxazlphx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vcfqovfr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yiqgdfnr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qfpncswd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hdnrbgja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ofipaaiz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zxnknksg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cespewmm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3odgeygmm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uojtbtro.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vczzaonm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3epuqhamr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xmuizjiw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tqzdyqez.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3johgsuau.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ncfravil.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qumqqrao.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vvkcrxwr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ecteysny.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3apwfkkeb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3heleoafn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3fktxnhjk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvykwrnc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gufgfxtj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qyovpfvq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bxgxonaq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lyzrxcdh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3iioenqbc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ojascrfs.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rogdppbs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dbnwwpnb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzhblzhb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qoikeyhb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xqucreyo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3huxhqaqa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rdecuswr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aavnkqwa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3domentmw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3duxhkiwc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wqljfbbd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qivxjlqy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tfkdadxx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pbysjwjn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kpwrctoa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3iiziatfa.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3htaidtfy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zhgjklbr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fxhpczzj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3eaocskda.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhzhgbm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nviyhqsb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bihzqrpk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wtivmxny.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ackhqqlf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gpwemoje.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gtfxdsud.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3isdhoxwa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxmwmna.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3omzvsxwj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3keeripad.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mekgamyu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nxwfjwjh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hxygxeje.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xtoenooj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hechtejm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3owpelpjd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxeywxg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfjbijn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ddflddyn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3smrssxtz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnunzmlk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cgggjere.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pmxrbtav.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnhrzpku.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3utcitfzv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tjthcdkb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3btdowdyh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cjhjiuue.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mxoyyaky.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkruieid.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qfxupchz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3cajzzdnz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hbauyrtn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dcdcxzwg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3phdojnkl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gavyjxpy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ydcloedr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emlipjnn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3krmrvrtj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3stoajfpm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olnxekze.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qjtyyndq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3yuisbdzl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3woihnmex.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hcchukyj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vxvrdleh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3quoevnuk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhzfqrs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ldoiifmm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pcnjtpgn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3enptrkgi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ctyvvclm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ysppfwkv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bfliqavq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3erscyubj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndhnvjlm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bcgdnqdr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hkochtti.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ogtmolnw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qmrzzqou.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3bgdmjela.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3jjgzeqfs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ercxjccs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bvdblthe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rhhjezpi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3nmgykkvh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3izqivvps.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nrtcazbo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sotvwfho.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rfmdbykk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3oytaaway.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hcbbwqmj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3boafebbl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wznksoyq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3okcyghsn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbyexrie.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zgbbxpwr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gfnagmpa.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3cumtlied.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hepscbkc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pojfxfsh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3nvmmftuy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3itptofwv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3lzlrlzes.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3didhixrg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xfwbcrkf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncdxyxzl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yenzwbwd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kkvvscas.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dwkwrgqb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yzusndno.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fuxrjhos.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfaewzxg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hstmimbv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pksqptmu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3scyepfbt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3fewherkb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pztmtido.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qdzscuzm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmoqxzs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vunujlnr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fkwvdepk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wuterzja.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tjxmgnjv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dcbslfhu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qxwhysmu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3loobmtto.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rdtvexpk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uayvuqfi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jgwkcktw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rolziwrv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kwsijjuw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zlpbddci.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vhlocjiy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wmaxslse.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vkyfbhkj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3chmdnfdu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zuxggyfa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ypykiqqe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3nmhobpul.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bmlgzuzu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dcxopcgr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3pkidesgr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3elknswiu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tyzntycy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fowxufbs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xffadqix.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pojfptoz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kvjhcteu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pcbagyey.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbtikng.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3lckkhhzf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmgewecp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbnjckn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3aqjijwjl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pwkqxbay.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lzouonzi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pikkubzt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uaokrlwh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mfhmtmuu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3crqozjcz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cwwdsiqx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nvgteglc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3okeynljk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ekbyrlln.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ccivjerv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eftczwps.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3srdtsmal.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qbnyggxh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gpdgaxfc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bodfjtey.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fyqtlnwz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmlhdln.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3varipqms.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uzwatjue.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tudcrncj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvfppfa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ftmjygyw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dxbwagma.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bjvcplew.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gtjgamai.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nfxwgpjb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fhdgnees.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hgforbpt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmdeyun.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lbwfaspf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qywqxnwi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3okdxnvfh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lpjekkyn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ijtidxre.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hhifkabi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lzjzyciu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xkfydrxc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zajejjbc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dudlqxvn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xarcrked.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fogogoeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hycybjya.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lwdkwlne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hplojlqg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ocqejejp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pfnimqgp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfbcggr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3truzlfze.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qyeltfmo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3azulxvwf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxmpawcc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bbqpdtln.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rlbxymno.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ieebwnzx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ozounmtv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mvqmftmj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tbpvbpmh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dvfnhbjm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iasfkgea.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvrsvmep.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3owmmchta.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oiisogfi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rwsmfnqp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3eblcngpb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbcwbvps.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ornbjprv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rcshmyce.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yxkfxvwl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jmshnlkg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3eowsfwlw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hppwyhxz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fbqmjyxo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fkozhkxu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkstrjh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3flgnkoyz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojavwibw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uokrziwe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cxpmbewi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3aefusagp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdmhxoyf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wettasuq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jwglteye.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvaknbts.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3drhgosme.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pmcualfx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vzsrcebf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vkmfgktu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ayqeupnk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mzboghou.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ryiazdzj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jxckoklq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rglyrnes.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdcricqx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fzgcgnnn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cmttdnqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hferzysa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxrdiddu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzyxbad.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pphaxcri.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ukqjozaf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjqkbhra.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvbijwfw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcymgjbf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zspqhgpf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xnrdduau.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3amngyinb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlbvtdk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ycmcytuj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xaefoiuv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mcqlgepj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kafvixls.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hrdeypnb.html


<!-- 参考信息 -->