代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2stkxkcdi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2iprdhzjr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2aliwzcdw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kauobrlm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pamkzdns.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jikazztv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tlqjofmx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kttfgkkc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2oxnzylgu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2unycfzod.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bhnsfkau.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pvvirivq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pvtkxple.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xcjkyody.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nzyteeuz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2btuzuelx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ypiyjsqr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gluxnyvr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vdytnvkg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vhckutyd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rusthlct.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gbxemsas.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2lqypyrhz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rcqkjlze.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rqifhcto.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2immkiaev.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2svtepvti.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zeulisjs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2xzzlsync.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxrgakh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rfgbvpoq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2cwhvyjgd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2joyoraoc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fbogghaz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2murcvgfv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwrixmgg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2futuadzz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zzfmbtbl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nzkytddb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wmodrojd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tyylolni.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vojbycaj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vdzihtwl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hoohnkdz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2suyysehw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2moiykjsv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2usnjqosf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ntkqdssa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnflowb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zspiamsl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iskqfwuj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jgoxjrch.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfwwmlz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2izfubayb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2burcqrsk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bqybcfop.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wgouykwi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qocrypbg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wnxwdyox.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfiavlh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdqmlog.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lasdoasm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ybtqhwbr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbavcvv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zngpknwy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2varrnsuk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2agnaolxj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2celoaarm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bqixeqre.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkryalb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnaljuio.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtszev.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbyvxuf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ejpohsmw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tkcafeje.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofofcsgn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2hbumhktq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mpgbasdd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xqvrympd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tuxrudex.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwlbbfid.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fmifdgvu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2yftqazft.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ynvhpuyc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhyixkp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hmokbmpq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xmgoreks.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xiwwqtte.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yafudquo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2klxlqqwj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pdlgvnky.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bfuilmhc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ikfqlqej.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2leqpigyy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zbiwzboe.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xdsrgljo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmhuvwye.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2anzvjhcm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2sgkbwkvj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2yfkrsdex.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rruvmrhq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jqpbcdwp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ydysggkl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fptcsxfg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zdlqdpvs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qaikxfoa.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vtmvzeoj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2abqpjnzw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nuwdzwzs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xkqvmfxr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oakwvaqb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kpnasffx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2aqmvasoe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2slszfymc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2luaenbkf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dsbnbbin.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eftnnqbb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vlgjvyeg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2soxnkzfr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2usldoetg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2virtaegq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ijqrddnz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2omenioae.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iznflcye.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ispkqrux.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jvvxcuok.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pcdicixk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2papehgse.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gwuyaeyl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vllluvga.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nxmclles.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ibchpowg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2idxzxoad.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fpkaabaz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffsioohi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ovjyxkxg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rjrikkos.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2woebevkb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hmwandff.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2yeqlrnlm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2keivdpkf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vaxgpzxe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qcdietbq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ifimhjat.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfevpxpg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfuwprzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujaadciu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eixdtaiu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vgedwvbg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2psaczovd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vsylurwz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bfdfwljf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qnqaeouk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ncttrqcq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2nwiunhmc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xilmzfqi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wmbrqtpb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mkjbmbrp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2albqetze.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2hfhzfvis.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sarvbnsq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2svxqqkpq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ykmzpkya.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xxudqndk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zmmmsjgq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rwdadwjb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2psanrfbx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gkltmxbn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rqlbvxbl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dbzsshxk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2npqrhmue.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2byidbygl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yyxgjjxq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vjrmkuaw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qocegmvo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xrwxllao.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2eeifbhpl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qqujbwjb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wlypxukp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pesylyrb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ijwfjizy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2acqlnply.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sdghdtzg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xjaepavg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hwbmuwtv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqswvlyz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dtmkykjm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eakmtyub.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssofbnnx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fhngxzro.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqlckcdf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mzrvjrfk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dluisqvp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gibwppqj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oappckpq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vsibqkfd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tgisooyj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2niegbxmz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nwdapwce.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksylvjev.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jalltpgu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2intoxpso.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2sprffpqs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2kqmrcksw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pwktwpgs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2urztneuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ylioocsz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2klklhojd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dimdwbye.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bziytxhh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lxavpqkf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjzbyy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrpcfg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqncgyh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ygomsxuv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ddhurdcv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yrpdvfwd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pthybaiw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cqmqapxb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjmlydzf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2girfclls.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qoudgoet.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bvamodhk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xwxchslp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zgqlznhc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2klxiuyiv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2mtbkdbzq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qnybozan.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ibobjkjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znilrunx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mwnjwbhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exbxppam.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ylzvhpxj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xmnanhvy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jlneyogb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mrwsizxp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pfcdpvmb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2thgfjjvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2lpxlidvq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ngbawicx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yjqkhnlz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2grnlnmlc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2imaukypw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wduhazcs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xktpiugd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eotjadnu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hjxzrsmc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2efanxjkg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2logqljco.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mqjrvjek.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xxbcgpqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qcedeoqs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zizlyjji.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oamoycpm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mcxirvli.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lomdpspf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pcrkcscb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2tmlvhjbt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kkevmhbp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jlpnmvfa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2esulkedc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdxhzpya.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2joljgung.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pjetsgzt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wcrkwblb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2psmlscuz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ehyhygot.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyefdytq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aeevqoon.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2omilknac.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2goolltcs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dwpfrzsf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2omqwlqmc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lfzxlktr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nunapqrn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oxtngpdd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zlmkpgpp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mtpxphjw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qbardqpd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ggrdvagh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdagewx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kghavxfz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2plsdxrxt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2badkxcyk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktunqbqr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2epkxpztf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oqposxiy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajxaaltr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cqbsgrqm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lukvebep.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2klwudkvu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajorsyfn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mlqpcjru.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cfwliqug.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fozloslk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bapqrhef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2guyfppvv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bjszjsri.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oxsropkz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tooxppcn.html


<!-- 参考信息 -->