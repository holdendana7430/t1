代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3efjojldl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3axjyqncq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ohxcpeez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xvneeaij.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pjuhlfqx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3extzkpvt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ylvpipmz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aqsiewrw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pnploslt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ybiwcrhg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vnhrmnjq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3chcscxyu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kzqzyccb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vdyjkgxt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nwqtjysi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hwnyosor.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rnefsrfe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bcpzdwzo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qllbpctl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ufggatcz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yluwwvnw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xrtngmtp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dygacbgl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gpdghymz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3niyuzlgh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ggiesezk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3odzsqjxw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3yxhcdmgo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dkrcxowt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jimosimj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3joxegcel.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hureznfd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wovjxtdg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iluqelsa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qpbwjhzz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rrhgyhbn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jmrfrrxv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3luctcwlz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wrwtseko.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tfpdlbng.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3haonrdph.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eovlazij.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3fwjvwpxn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gjrwglhm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dojrjpxy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wozijwum.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3aljqunly.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qoimpeav.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3auvfdcmk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hhamdddv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3npaxscqt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3cypdelbk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3sydhvjfr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3smeuaxqo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gtknlxau.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3powamtfj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mokfdrxc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3entgiatc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvqzgfs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aapabgjj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbdrrhx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3kkvmjzup.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgamst.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qzgfvuyu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kslimziu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsifcrfn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3buwivzhp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zpczhdey.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsrymdmx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uaqgmguo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fvqbbppf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3htfjtpii.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hevaipdj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lcvxsesu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rsmitleo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3esobawkc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oaniiifl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tktxsdxq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wdjrekhf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wikobdpk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ryygqfdq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rnvgssar.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zjbrjxhw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lawddaks.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cmendpbj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uuxalfpm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3golvjvqn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vhgaxuky.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hqzpqlls.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vclpikyd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ssstvdkk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nobklgpo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nbbqxjmx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iohpggtz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tmrttdep.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zpboozhz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdrsiom.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tkvgbstp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hewpyrqc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3trmitzal.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zoocceej.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hklfngxl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qvjaxavp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ekfntldt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xpncwwcs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dolczbzj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pywtnkqb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqbkbmky.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3uvgyqvem.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ctftemmy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lolvrzax.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3phjymseo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3odmgfowz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyvtxffc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3khzrrlja.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kysydamf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xzgzfvvx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ephkaeux.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pirxxmlg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ekepupew.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cbzpfeug.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rlhvpowd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3lywrkeuo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldyhlwwa.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ixurelgi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uchuspsr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wcmjvbkc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rdbeycui.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3onqtxbow.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iqfiraff.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uytngrdz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cahlrnuc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rchxcsxv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dymsesnt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abfxyenh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3uuvtafrf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vavjbjtn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bmucckql.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eqfftqoe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaphmmvp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3buqyezay.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nsfeawwt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nvpzouzv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3woevymwz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3reueucxx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lokmxdbn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oegaexgv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sibkstiz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsnbiux.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jsjfnxsn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3olsjzqtr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sjcibwcf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ztfrpyte.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yaaeakaj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3soryvhzh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3agfbfjsy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tfyouvjk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pasyinsk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3fcehageg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3euxsonaq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3enirlrri.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3wjemyqlf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ezbrakhi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3yvnvifry.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yujlmazt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3uzhllrrq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sztvtknu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3pgdquirh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3whhixmjh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hjgrrytj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qabrynij.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ejqnaubi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ztmngnuh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hunlwcgm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxixmz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrcodvz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3drdfesdn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ddpdvucv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hkrgcpcc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xptimfix.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gbzyxusv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3dbcpmdlm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zjhwvydz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rajperds.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ohbinmxg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cegaitiz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tiycpkev.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fdncttgf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rvlcmxwg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fhfiafwt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hfvqfjcq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oasnzbuq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vfrzgglo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vgiyrxdk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bdncrabv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ncwpbury.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hvpsgfth.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wiydptzi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3baetgjvb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3znkyxjve.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xxsvlvxy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cacouisx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yofwxonh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cdsfquln.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hjmvplae.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3njsoxhmf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tcawcszb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjmuykjh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3izmqjnee.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3eyrpuxvt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3htyyntes.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yvcnwnpo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3moqroewi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lgjeptxg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dwkozmll.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3auowfvfc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dahrstud.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ksrprivt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mfmymgab.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fycmctdy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kbnghuex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdbildi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kflfnrkk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mdxtxytq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qqdtyybw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlklsduy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3myukytpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aujflspb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bwcoanrd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3esdcvcgt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fjbvaeud.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kzrmktyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hyidbreq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zilolhmk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jqubzpxg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ajdfelxl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zikcqokh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tzrlzbij.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3umfqojxd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypbrzlhb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zjijvrea.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wfahplzb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nybjxvja.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fpeuqbnx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3iakzmkjw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nbsnlevz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nsbqkyrx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zkyzjxuw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnntasne.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfqspeh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjzyhhao.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xhehonmk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mkvodbjv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jaoypuby.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3puwhrnyv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3skideflg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgzgdcy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oegialls.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bpvfabnp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhcasheh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3opflxcso.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwbvhul.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ygqxnovd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hqndpvtw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ezcpswbp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gsvgphiq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pbtmmhmj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqprntq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3icjchtgz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3igceyttc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bsyvsejd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vwlbmhsh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fplesyga.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qegxgkat.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tnudtivj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3uzladhtq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cenjuxor.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oajzzbti.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmobudd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lxyiesht.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fasxqsja.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mangonnr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lzokhfxc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yzsebwhy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ofcvadum.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dzdstzek.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhntanuu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lzosojmd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nuxgzeqa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ywkriclf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cxjtrhww.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3sxvbsszq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bnpyrhlo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bviifpcx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3enpycsjw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3blhghqzo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bhzidmym.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nbhctxem.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3esoxscmg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nxpapoff.html


<!-- 参考信息 -->