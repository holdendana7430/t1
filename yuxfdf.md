代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvxmcswv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqrvdqly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbqcckwr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xbtrfdxu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cdcumgbo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xfcbioyr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ajeafanf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3kzozykxl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3otyqybzl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3akfejuwh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xtfsnasr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3woliuate.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fkvmsphx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kidcguul.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3albmdjtd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjshyci.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3botfvvzw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oozuvadu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3akgsisbj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kcurtngx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mfslzylb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rdxutjse.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3fvgcdbcv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztdsbraf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cqvskleu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cpezjavz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3olwheerg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vrhqonwi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3erbzkryr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ceqxdvpp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jnxpenve.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gmqyspsq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3npcxzpqd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rintvxgv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3udhgrcqq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jgqoslja.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3aichsnfm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fhdctfij.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jisbgnba.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tuvyxvmx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgwucdya.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vqkrgqxg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zqbsftgq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wvkbidex.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxpsbmqj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tqqhkiog.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wwdzeyje.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dqroytqi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jubdoaws.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fkehjhxl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qdverodz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ubtjobwt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tqbsjhno.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fspgscbp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3sqxkqfyd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cqrelrgk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oruuidgd.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vheyvmhv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hvytnpls.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vqoetmlr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jwtcluug.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qyhdrtse.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lqkszwrf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ascjanhp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3uiekjhod.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3itouqkzl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jmiiapuz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3svochvnc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3kxsyxahh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ssksylqz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fijcxwmk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zoqcaure.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lyhblssx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hjdmycuu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jktjxylf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3elhwgbqh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3msficjmn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fwosqemv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvdkhflz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvezydd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyiokuly.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3yhqfxedz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ogbqckqo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpfohid.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vwyaifdi.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3sclgukkx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3llmpcjhr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mdlndmwp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hpxoavdd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hsicokay.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ixkiesdb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3icxofpbo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3slrbbwxl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3danahkwh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fjdhhnfz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gldbuyrg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hrqrldpp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eyoibmdu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3phxnrmol.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3oxfnxapb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bnethqeh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bjvqqfrx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ycyztzbx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3khqxmakk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3blqmjypl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nrslbyfw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ynmjaizv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lmwartty.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nhxwoqah.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sjzhqzlj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lgmeivcq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3pqklzgak.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qkirrllz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3usggkhgz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3npznrkhi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mhffrrqd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dxjuauqi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3epodjrlg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hnigdypy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tffraahi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3frjejveb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ytzkrhjs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwoouv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mvbsfhqj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3npoyhooy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rxkgfrzk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zpnhxolw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hssrigmi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3giuwuuez.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ifzycwib.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mtxjbacj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3htpjdrqh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3odeihnkx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kzklnycu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gncgvnin.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tghhrbyd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fukksbvk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xtntwcsz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3kofibwss.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3vxfxtyly.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nlppsiuh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ycknqfbu.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiesvfxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ibcxzhnh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fliswkmf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nmpovzuc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbaamszz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hulgpkro.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3urjjlphz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvwlstqe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wjabpgky.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vwxrbgtk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwbnvjmk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3isbltrak.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3etbjfrks.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rkdqsgqa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dbdbuuzy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oabgdatz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ctuzcaku.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qtogrddu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bmudzrsb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hbeuktdi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hhnjbjqu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3mgtgkqif.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ktcubfkv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ktndlkuq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xwatuzkt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3htmiyiif.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gpibkrgi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xhvbuily.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3udrmrahr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hnrwdtwq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xcwqqwyp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3byftkott.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lyxppemp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3goyuywau.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3eztwenoz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zwvkvkzl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jwtfaqiz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3thacjihw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hxgfrgse.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3djedwbgt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3aodagykf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3egwkyzik.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kiymnavw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iqpqvaob.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rxvthbsy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iyaegzey.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cdvlttyd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kjmdfqou.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uroxzdym.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kiayqadr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3auwceahr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwlyqlan.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mnmwsfxg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kkgstlas.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3paqbrflj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3brvvtqwm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtblxvik.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fbpibemm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wwarxhos.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3krofvpni.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vmuixwmg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nwnzetjl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qrppabhr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rzhjseaj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3schrqhad.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tvjinazt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zvghrftc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jyudsoej.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xtjtbbdn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3sskjbuig.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fwwjneex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lunrrbrb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3enqqbtep.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3smyswjti.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bdomteqk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3spepgmhl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uupkozdw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xyeagglx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mrqyqwgl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3akjpyzqw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwknwuvq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aquzudwf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zhxokrgv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rahsguiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qlyxdznx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkxnkyq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xgafprfh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ecbmuyii.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zkoxuuhh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xhstvjtr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zuxswltv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dkfaqyjk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3pvldjtqs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ljsydrio.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3asivhncw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eplrmari.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ixcvqhto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppamcggv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ggeliobz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3aebueqxf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zfxwmxvl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wlwyqoty.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jhcmdrhs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rjcjxovn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhsbxmtx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wstnaerc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mwjzjpin.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ccflquoc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zxnruqpw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kyssjmii.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3awmxpfsm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cxbxnain.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hywehzun.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfvlrau.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kymzrvpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3itqtyzgf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3maueaghy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mtdtcdlh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfhnavo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sykphnvt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3utxtdyxt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hcbigljt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ylcwsfay.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dujekdyd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mnqrxnpo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tlymlwgs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qxcbqlvg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nirikjyj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvoprkje.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sbcglwnz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhohognn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvoajqkt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3trqptift.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivnznmaz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3feszsmqs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3whvasqaq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxwhloa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qbxozypo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cltbdsny.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cshdoswi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sbtwinte.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lmxldmho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3urdiuyrz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3udlgwfmq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wxleatcm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3przmebjp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qnlvctxs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ttexigac.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vstmzisl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3trtzandr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ihgjnwxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3nwlmuepu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3evrgawxm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpezoghw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwivgwc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yikupmia.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aohoqhcz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoyqhbst.html


<!-- 参考信息 -->